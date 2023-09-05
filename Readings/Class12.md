## Spring boot JPA

- Spring Data JPA allows you to define repository interfaces, such as CustomerRepository, which extends CrudRepository. It provides methods for common operations like saving, deleting, and querying entities. You can also define custom query methods, like findByLastName and findById.Query methods in Spring Data JPA are defined in a repository interface by declaring method signatures with a specific naming convention. The naming convention is based on the properties of the entity you want to query.

- To complete the Spring guide mentioned, you will need the following dependencies:
Java 17 or later.
Gradle 7.5+ or Maven 3.5+.
Spring Data JPA: This is typically included when you use Spring Boot, but you can explicitly add it as a dependency.
H2 Database: This is an in-memory database used for demonstration purposes in the guide.

- The annotations used to specify an auto-generated identification number (ID) for an entity in Spring Data JPA are:
`@Id`: This annotation marks a field as the primary key of the entity.
`@GeneratedValue`: This annotation, when applied to an @Id-annotated field, specifies how the ID should be generated. Common strategies include GenerationType.AUTO, which allows the JPA provider to choose the appropriate strategy, and GenerationType.IDENTITY, which typically corresponds to an auto-incremented database column.

## Spring Data repository interfaces

- The **JpaRepository** has the most methods available among the Spring Data Repositories. It includes methods for CRUD operations, pagination, sorting, flushing the persistence context, and batch deletes.

- One downside of a Spring Data Repository is that it can lead to tight coupling of your code to the library and its specific abstractions. Additionally, when you extend a repository interface like CrudRepository, you expose a complete set of persistence methods, which might not always be desired if you want more fine-grained control over which methods are available in your repository.

- To define an operation to find a student based on their name in a repository named StudentRepository that extends JpaRepository, you can declare a method in the StudentRepository interface with a specific naming convention. Here's an example:
`public interface StudentRepository extends JpaRepository<Student, Long> {
    Student findByName(String name);
}`
