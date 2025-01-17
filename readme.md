Introduction: App uses JWT token based access only.
All endpoints need token except registering user.
CRUD operations checks user ownership before applying changes.
ANy user can see all blogs,comment on blogs,reply to comments however updation can be done by owner only.
Owner of the blog can delete any comment from the blog.
Java v17 is used.
Project Structure
com.blog -> contains main app class
com.blog.config -> contains security and other config
com.blog.controller -> contains all controllers (user,blog,comment,vote...)
com.blog.dto ->contains Data transfer object files.
com.blog.exception -> all exceptions and global exception handler
com.blog.filter -> filters 
com.blog.mapper -> custom mapper classes to map entity to dto and vice versa
com.blog.model -> all entity classes
com.blog.repository -> all repositories(user,blog,comment,vote...)
com.blog.service -> it has service interfaces (user,blog,comment,vote...)
com.blog.serviceImpl -> it has respective implementation for service interfaces (user,blog,comment,vote...)
com.blog.specification -> specifications for filtering blogs with pagination
com.blog.util -> Utility class 
=======================================================
Setup Instructions
------------------
1.Java 17
2.Postgresql recent LTS version will work
3.Change application.properties as per your local
spring.datasource.url=jdbc:postgresql://localhost:5432/blogapp    <--- your postgresql url(make sure db name is same "blogapp" or change the url accordingly)
spring.datasource.username=postgres     <---- your username for postgres
spring.datasource.password=postgres     <---- your password for postgress
server.port=8888 <--- port on which you want to run the app
