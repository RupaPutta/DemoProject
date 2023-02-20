# Spring React Annotations Cheat Sheet

## File: com/example/SpringReact/SpringReactApplication.java
* @SpringBootApplication: This annotation is used with main class of Spring Boot Application. One of the most basic and helpful annotations, is @SpringBootApplication. @SpringBootApplication is @Configuration, @EnableAutoConfiguration and @ComponentScan annotations combined, configured with their default attributes.


## File: com/example/SpringReact/controller/*
* @RestController: Controller Class annotated with `@RestController` has REST end points.
* @RequiredArgsConstructor: The `@RequiredArgsConstructor` annotation generates the constructors with one parameter for each field needing special handling.
* @CrossOrigin: This `@CrossOrigin` annotation enables cross-origin resource sharing only for this specific method. By default, its allows all origins, all headers, and the HTTP methods specified in the `@RequestMapping` annotation.
* @RequestMapping: `@RequestMapping` is the most common and widely used annotation in Spring MVC. It is used to map web requests onto specific handler classes and/or handler methods. `@RequestMapping` can be applied to the controller class as well as methods.
* @ResponseStatus: `@ResponseStatus` marks a method or exception class with the status code and reason message that should be returned. The status code is applied to the HTTP response when the handler method is invoked, or whenever the specified exception is thrown. It overrides status information set by other means, like ResponseEntity or redirect.

## File: com/example/SpringReact/service/*
* @Service: Components in Service Layer need to be annotated with `@Service`. Mark a specialization of a @Component. It tells Spring that it's safe to manage them with more freedom than regular components. Remember, services have no encapsulated state.
* @RequiredArgsConstructor: The `@RequiredArgsConstructor` annotation generates the constructors with one parameter for each field needing special handling.

## File: com/example/SpringReact/repository/*
* @Repository: Components in Repository Layer need to be annotated with `@Repository`. 

## File: com/example/SpringReact/domain/*
* @Data: The `@Data` annotation is equivalent to the combination of the following annotations: (@Getter, @Setter, @RequiredArgsConstructor, @ToString, @EqualsAndHashCode). We can replace annotating a class with the annotations that are listed and a single @Data annotation.
* @AllArgsConstructor: It generates a constructor requiring an argument for every field in the annotated class.
* @NoArgsConstructor: It generates a default constructor with no parameters.
* @Entity: A class which need to be mapped with underlying database table.
