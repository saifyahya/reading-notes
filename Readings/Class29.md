## Overview: Saving data with Room
- Database Engine Used by Room:
Room is wrapped around SQLite, which is a lightweight, embedded relational database engine. SQLite is a popular choice for mobile and embedded applications due to its simplicity, low resource requirements, and reliability. It is well-suited for Android apps because it provides structured storage with the advantages of a relational database.
- Is it a Good Choice?
SQLite is a good choice for many Android applications. It offers benefits such as data integrity, ACID compliance, and efficient storage. Room provides a higher-level abstraction over SQLite, making it easier to work with, and it handles many database-related tasks for you. For most Android apps, SQLite through Room is a suitable and efficient database choice.

- Similarities Between Room and JPA (Java Persistence API):
Room and JPA share some similarities in their purpose, as both are used to simplify database interactions in their respective ecosystems (Android for Room and Java EE/Java SE for JPA). However, they also have significant differences:
- **Annotations**: Both Room and JPA use annotations to define data models, relationships, and queries.
- **Object-Relational Mapping**: Both Room and JPA perform object-relational *mapping (ORM)* to bridge the gap between the object-oriented world and the relational database world.
- **Entity Management**: JPA, as part of Java EE and Java SE, offers more extensive entity management features, including features like caching and lazy loading, which are not present in Room.
- **Platform and Ecosystem**: Room is specific to Android and is optimized for mobile apps, while JPA is part of the broader Java ecosystem, including Java EE and Java SE.
So, while there are similarities in their use of annotations and ORM principles, Room is tailored for Android's needs and offers a more simplified and Android-specific approach to database operations.

- Description of a DAO (Data Access Object):
A DAO, or Data Access Object, is a design pattern that separates the database operations from the higher-level application logic. In the context of Room and Android, a DAO is an interface or abstract class annotated with @Dao that defines a set of methods for interacting with a specific database entity or table. These methods typically include operations like inserting, updating, deleting, and querying data.
A DAO provides a clean and abstract way for the application to interact with the database, abstracting away the underlying SQL queries and database management. It promotes separation of concerns by isolating the database-related code from the rest of the application, making it easier to maintain, test, and understand.
DAO methods can include convenience methods for simple database operations and query methods for more complex and customized data retrieval. Developers can define parameters in these methods to filter or manipulate data based on application needs. In summary, a DAO acts as a contract that specifies how the application can access and manipulate data in the database while promoting good architectural practices.