## Week Two - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON - YOU are a web developer!!!). 

Note: When you're done, submit a PR. 

1. At a high level, what is ActiveRecord? What does it do/allow you to do?<br>
*Active record is an object relational mapping tool. It allows us to interact and manipulate databases. We do this by wrapping the database tables in a ruby object so we can create our own methods and interact with the information in these tables.*

2. What is a migration?<br>
*A migtration is the instructions for how we want our database to be created and/or altered.*

3. How does a table relate to a model?<br>
*A table is represented in the model class...* 

4. What kind of methods are `belongs_to`, and `has_many`? (i.e. class or instance) Give an example.<br>
*These are instance methods. We call them on the instance of the class, not the whole class.<br>
A teacher model(class) could has_many: students, while the students model class belongs_to: teacher. The student table would have the foreign key of the teacher.*

5. What do they allow you to do?<br>
*They allow you to associate ..*


6. What's the difference between agile workflow and waterfall method?<br>
*Agile workflow aims to break up a project into smaller parts that are tested and complete on their own. You could therefore have a very small working part of your project before your move on to starting the next part.   Waterfall method takes the whole project together, plans for it and impltements it.  This makes it much harder to make changes along the way and adapt to new problems, which would be much easier in the agile method.*

7. What is the difference between `#new` and `#create`?<br>
*Create combines '#new' and '#save', so it makes a new instance of your object and it saves it into your database. '#new' just creates a new instance without saving it.*


8. At a basic level, what does cURL allow you to do?<br>
*cURL allows you to transfer data to a server*

9. In a database that's holding students and teachers, what will be the relationship between students and teachers? Draw the schema diagram.<br>
*tables below
```Students table               
  id
  student name
  grad

```

10. Define foreign key, primary key, and schema.<br>
*A primary key is the unique identifier for the row of data in that table. A foreign key is a primary key in a different table, that is used to make an association in our current table. *

11. Describe the relationship between a foreign key on one table and a primary key on another table.

12. What are the parts of an HTTP response?

13. `Rack::Test` allows us to test our controllers in isolation. What are some of the methods it gives us to simulate the request/response cycle?
14. Describe some techniques to make our Sinatra views more DRY. Give an example of when you would use these techniques.


### Optional Questions

1. Name your five favorite ActiveRecord methods (i.e. methods your models inherit from ActiveRecord) and describe what they do.
2. Name your three favorite ActiveRecord rake tasks and describe what they do.
3. What's the difference between agile workflow and waterfall method?
4. What can you expect from a group as you begin working together? As you continue working together?
5. What two columns does `t.timestamps null: false` create in our database?
6. What cURL flag can you use to send a `POST` request?
7. What case does JSON (and JavaScript) use for multi-word variables?
8. What case does Ruby use for multi-word variables?
9. In a database that's holding schools and teachers, what will be the relationship between schools and teachers?
10. In the same database, what will you need to do to create this relationship (draw a schema diagram)?
11. Give an example of when you might want to store information besides ids on a join table.
12. Describe and diagram the relationship between patients and doctors.
13. Describe and diagram the relationship between museums and original_paintings.
14. What are some examples of acceptable values for the parts of an HTTP response?
15. What types of output do we want to test when we test our controllers?
16. What could you see in your code that would make you think you might want to create a partial?
17. Why might you use a helper method?
