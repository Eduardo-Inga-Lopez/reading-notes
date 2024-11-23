# Cómo implementar una búsqueda con filtros usando Spring Boot y MongoDB

Implementar una búsqueda con filtros en Spring Boot y MongoDB puede ser eficiente al usar `Spring Data MongoDB`. Aquí te dejo una guía paso a paso:

## 1. Configura tu entidad
Define una entidad para mapear los documentos en MongoDB. Por ejemplo, para una colección de películas:

```java
@Document(collection = "movies")
public class Movie {
    @Id
    private String id;
    private String title;
    private Integer year;
    private String genre;
    private String director;
    // Getters and setters
}

```
## 2. Crea un repositorio con consultas personalizadas
Usa MongoRepository o implementa búsquedas dinámicas con @Query. Por ejemplo:

```java
public interface MovieRepository extends MongoRepository<Movie, String> {
    List<Movie> findByTitleContaining(String title);
    List<Movie> findByYearBetween(Integer startYear, Integer endYear);
    List<Movie> findByGenreIn(List<String> genres);
}

```

## 3. Desarrolla un servicio para manejar la lógica de negocio

```java
@Service
public class MovieService {
    private final MovieRepository movieRepository;

    @Autowired
    public MovieService(MovieRepository movieRepository) {
        this.movieRepository = movieRepository;
    }

    public List<Movie> searchMovies(String title, Integer startYear, Integer endYear, List<String> genres) {
        if (title != null && startYear != null && endYear != null && genres != null) {
            return movieRepository.findByTitleContainingAndYearBetweenAndGenreIn(title, startYear, endYear, genres);
        } else if (title != null) {
            return movieRepository.findByTitleContaining(title);
        } else if (startYear != null && endYear != null) {
            return movieRepository.findByYearBetween(startYear, endYear);
        } else if (genres != null) {
            return movieRepository.findByGenreIn(genres);
        }
        return movieRepository.findAll();
    }
}
```
