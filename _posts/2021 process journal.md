---
title: "hello github blog"
date: 2021-04-11 19:05:00 +0900
categories: test1 test2
---
$ Process Journal (first person perspective)
- ## **Day 1**
Through the class session I have reviewed familiar and unprecedented topics simultaneously: HTTP, Client-Server, RESTful and git. Initially, I downloaded required applications to puruse my tasks, including intellij, java, git, iterm, etc... To review, *HTTP* is the abbreviation for Hypertext Transfer Protocol, which is used for the communication for browsing web. Moreover, HTTPS significantly correlates to the "client-sever" concept because the client forms an HTTP request according to a web server, that a server responds. 

Also, the URL is a ubiquitously conecept as it is well known. URL stands for Uniform Resource Locator whcih is used to identify resources on a web. There are 4 factors incorporated in the URL, the protocol, domain, path and parameter, and they are crucial because they determine the allocation of the server. In order to operate the HTTP, the request needs a method where the four methods are
- GET (read)
- PUT (update)
- POST (create)
- DELETE (delete)

The HTTP request is divided in to 3 correlated parts in conjuction with the 4 factors, they get, request and use a HTTP version to operate a server. Furthermore, there are status Codes from 1xx-5xx informing the requester the status of the requsted HTTP.

The *Representational state transfer* (REST) contained the instantaneous stat of a system resource through the use of requests and responses. Like the HTTP, the REST has 4 contributing factors: Create, Read, Update and Delete. 

*Client-Server* is a model that describes how a sever provides resources and services to several clients. Each distinct servers provide resources to requested devices; therefore, the majority of servers have more than one relationships with the client.

- ## **Day 2**
"*Git* is a free and open source distributed version control system." Moreover, the git is capable of storing projects and files as they change over time with the contribution of diverse users. Therefore, the git progressively alters the updates on a repository, and a repository has commites to the project or references called heads. 

I have created a new repository to record our data sets and work. In order to create a repository, I used iterm with the commaneds stated on the slides.

Additionally, the Git has 5 vital codes used form branches:
- CLONE: download
- PUSH: upload and sync
- PULL: download with sync
- FETCH: refresh the state of remote repository
- COMMIT: save local changes

Consequently, I have formed, merged, altered a branch/repository according to the class session.

- ## **Day 3**

*Github blog:* on day 3 I created a reposity for a potential blog, and it was intriguing that github noticed my intention of creating a blog. Therefore, the fundementals of a blog was automatically updated by github. In order to create a blog I used the 5 factors of the git, especially "commit" because I was commiting a new repository. 

To continue the process I had to confirm if "ruby" and "gem" was installed, then I attempted to install "jekyll" and "bundler" as they are crucial resources. However, there was an inevitable error, but the potential trouble was anticipated by the teacher; therefore, we were able to pursue our tasks without squandering time. Moreover, the problem was exacerbated after another error was induced, the CLT error. After fixing all errors, we browsed for Jekyll themes, and installed the most eligible theme. 

Then, I transfered the "index.html" to my personal repository. After initialising a blog I commited and pushed the file to create a blog. Furthermore, I created a post in order to blog my process journal. 

*Spring Boot:*
I have setup spring boot according to the instructions, unzipping the folder to open it on IntelliJ. Then I learned about the packages, and added them to begin our API session.
- ## **Day 4**

On Day 4 I learned about the significance of the Bean Container, Inversion of Control, Get Beans, and about the most frequently used Spring Bean annotations. 

*Bean Container*
Beans are a crucial factor of a Spring Framework, but in order to utilise this concept I had to comprehend the fundamentals of how the Bean operates. 
Spring Beans:
is an object that forms the backbone of an application that is managed by the Spring IoC container. Moreover, the bean is formed and managed by the Spring IoC container, and the bean is like an component of a application.

*Inversion of Control*
The Inversion of Control occures when a bean exploits its feature when an object defines the dependencies of the bean (Inside a Spring)
Moreover, the Inversion of Control designates the job of constructing and developing dependancies to a IoC container.
e.g.)
A person has a property of an animal, but suppose that animal has two distinct properties: name and age. Then, to instantiate a person (an object), we will have to follow the procedures listed below:

<img width="605" alt="Screen Shot 2021-04-25 at 11 52 33 AM" src="https://user-images.githubusercontent.com/73371470/115978749-b9870380-a5bc-11eb-87f6-b57fae51f639.png">

This shows that the two classes are coagulated and if the animal's property changes, the person's property will change proportionally. Therefore, the use of the Inversion of Control is convenient because an object can retrieve its own dependencies from an LoC container, instead of constructing them again.

In order to pursue that particular task I would need to provide the container with an appropriate configuration (metadata)

<img width="635" alt="Screen Shot 2021-04-25 at 11 57 02 AM" src="https://user-images.githubusercontent.com/73371470/115978848-5ba6eb80-a5bd-11eb-8511-30fda1822b13.png">



e.g.)


<img width="547" alt="Screen Shot 2021-04-25 at 11 58 00 AM" src="https://user-images.githubusercontent.com/73371470/115978884-7d07d780-a5bd-11eb-94f2-4342ecaac96a.png">
<img width="581" alt="Screen Shot 2021-04-25 at 11 58 12 AM" src="https://user-images.githubusercontent.com/73371470/115978892-84c77c00-a5bd-11eb-8a35-b56fd6c3dd0e.png">

*Get Bean*
In a Spring container there are several implementaions you can use by the use of different signatures.
- By name: the name returns an object if a bean with the identical name exist
<img width="573" alt="Screen Shot 2021-04-25 at 12 00 30 PM" src="https://user-images.githubusercontent.com/73371470/115978950-d5d77000-a5bd-11eb-8991-1012b045a144.png">

- By name and type: the name and a type returns a bean of a specific type if it does exists. Moreover, this may be useful to aviod to cast the object when returned
<img width="573" alt="Screen Shot 2021-04-25 at 12 02 09 PM" src="https://user-images.githubusercontent.com/73371470/115978985-10d9a380-a5be-11eb-93af-847740f3330a.png">

- By type: with the use of this I can find more beans with the same type

<img width="573" alt="Screen Shot 2021-04-25 at 12 02 55 PM" src="https://user-images.githubusercontent.com/73371470/115978995-2c44ae80-a5be-11eb-8533-fc8197e61436.png">

- By name with constructor parameter: with the use of this I can pass the bean's name and its constructor paremeters:

<img width="587" alt="Screen Shot 2021-04-25 at 12 03 57 PM" src="https://user-images.githubusercontent.com/73371470/115979010-51392180-a5be-11eb-8ccc-8028866b7d9f.png">

Then, we will get an animal named Fuffy with an age of 5

- By type with constructor parameter: instead of the name the system will have to pass the ype and the bean can not be a singleton

<img width="569" alt="Screen Shot 2021-04-25 at 12 05 26 PM" src="https://user-images.githubusercontent.com/73371470/115979033-86457400-a5be-11eb-910b-c42445a3548c.png">

The 5 methods listed above are the most ubiquitously used algorithms because the BeanFactory interface gives the beans from the container.

*Most frequently used Spring Bean annotations:*

<img width="498" alt="Screen Shot 2021-04-25 at 12 07 06 PM" src="https://user-images.githubusercontent.com/73371470/115979087-c1e03e00-a5be-11eb-8c9a-81f1c823da58.png">


- ## **Day 5**

On Day 5 I learned about the relevance of the Controller, Service, Repository Pattern, H2 DB Setup, Entity Class, Repository Class, Entity Manager, and the ER Diagram. 


*Controller, Service, Repository Pattern*
- The Controllor has a layer which contains the application logic, and the logic maps the user's request to particular function. Then, passes the input to a service layer in order to apply to a business logic:

<img width="611" alt="Screen Shot 2021-05-02 at 2 42 37 PM" src="https://user-images.githubusercontent.com/73371470/116803649-a512b000-ab54-11eb-8925-2d5242ef52d4.png">


- The Service layer is located between the controller and the repository which performs the business and validation logic, and we can see the connection between them because the controller passes the user input to the service layer, then passes it to the repository after applying the business layer.

<img width="611" alt="Screen Shot 2021-05-02 at 2 42 37 PM" src="https://user-images.githubusercontent.com/73371470/116803649-a512b000-ab54-11eb-8925-2d5242ef52d4.png">


- Difference of the Business and application logic

The Business logic addresses the logical manipulations relevant to the business domain; therefore, I can infer that the business logic is specific to the business layer.

Despite the function of the business logic, the application logics represents the application level operators, which is specific to the application.


- The Repository is the layer which interacts with the database (CRUD) operations aimd the data access objects (DAOs)


- THe model is the simple POJO class which acts as the DTA and DAO


<img width="686" alt="Screen Shot 2021-05-02 at 2 51 37 PM" src="https://user-images.githubusercontent.com/73371470/116803861-e6578f80-ab55-11eb-87a1-1995b1b021fe.png">

<img width="633" alt="Screen Shot 2021-05-02 at 2 52 02 PM" src="https://user-images.githubusercontent.com/73371470/116803875-f66f6f00-ab55-11eb-8e5d-d6a10120ffae.png">

<img width="685" alt="Screen Shot 2021-05-02 at 2 52 16 PM" src="https://user-images.githubusercontent.com/73371470/116803945-fec7aa00-ab55-11eb-907d-1d90e5f17140.png">

Today I learned about the Repository, Model and the database, as I have already covered up the topics before.


*H2 DB Setup*

After downloading the H2 DB I ran h2.sh in the terminal:

<img width="611" alt="Screen Shot 2021-05-02 at 2 54 12 PM" src="https://user-images.githubusercontent.com/73371470/116803984-42baaf00-ab56-11eb-8284-34dfaf1299ab.png">

Then, I had to setup the H2 DB

<img width="617" alt="Screen Shot 2021-05-02 at 2 54 45 PM" src="https://user-images.githubusercontent.com/73371470/116803996-582fd900-ab56-11eb-9e0f-efc68711c369.png">

<img width="647" alt="Screen Shot 2021-05-02 at 2 54 58 PM" src="https://user-images.githubusercontent.com/73371470/116804002-5ebe5080-ab56-11eb-948e-8c50784de31b.png">

<img width="644" alt="Screen Shot 2021-05-02 at 2 55 08 PM" src="https://user-images.githubusercontent.com/73371470/116804007-64b43180-ab56-11eb-84b7-5647a854e8d1.png">

<img width="631" alt="Screen Shot 2021-05-02 at 2 55 23 PM" src="https://user-images.githubusercontent.com/73371470/116804012-6d0c6c80-ab56-11eb-9a48-cb1f26cad4d6.png">

After completly preparing H2 DB, I have added a dependency to "build.gradle"

<img width="471" alt="Screen Shot 2021-05-02 at 2 56 24 PM" src="https://user-images.githubusercontent.com/73371470/116804031-9200df80-ab56-11eb-9e4e-8ee3e8b6d9f2.png">

Then, I have created a "application.yaml" in src/main/resources

<img width="458" alt="Screen Shot 2021-05-02 at 2 57 04 PM" src="https://user-images.githubusercontent.com/73371470/116804040-a9d86380-ab56-11eb-9fb1-d3af42ed965e.png">


*Lombok Setup*

As, Lombok was already installed and updated, I added a dependency to build.gradle

<img width="679" alt="Screen Shot 2021-05-02 at 2 58 20 PM" src="https://user-images.githubusercontent.com/73371470/116804067-d7251180-ab56-11eb-9346-bccbce6cfb51.png">

Then, I enabled the annotation process

<img width="522" alt="Screen Shot 2021-05-02 at 2 59 06 PM" src="https://user-images.githubusercontent.com/73371470/116804075-f1f78600-ab56-11eb-8132-40cbdfb4b45b.png">


*ER Diagram*

<img width="505" alt="Screen Shot 2021-05-02 at 3 00 06 PM" src="https://user-images.githubusercontent.com/73371470/116804090-16536280-ab57-11eb-935b-1f914aa7c3d1.png">

- One to One Relationship

A diagram has a one to one relationship when a row in a table is related to another row in another table

This relationship can be created by using the Primary key-unique foreign key constraints

<img width="334" alt="Screen Shot 2021-05-02 at 3 02 12 PM" src="https://user-images.githubusercontent.com/73371470/116804133-60d4df00-ab57-11eb-82d7-604e7a6d8eda.png">


- One to Many Relationship

This concept is similar to the one to one relationship, but this relationship is where a row from a table can have multiple relationships with rows in another table

This relationship can be created by using the Primary key-foreign key relationship.

<img width="372" alt="Screen Shot 2021-05-02 at 3 04 01 PM" src="https://user-images.githubusercontent.com/73371470/116804169-a1ccf380-ab57-11eb-9ddc-cdaff3c1a412.png">


- Many to Many Relationship

This is where a row from a table can have multiple matching rows with row in another table, and a row from another table can also have multiple matching row with the first table.

This relationship can be created by using a thrid table called the Juction table or the Bridging table

<img width="280" alt="Screen Shot 2021-05-02 at 3 06 27 PM" src="https://user-images.githubusercontent.com/73371470/116804205-f96b5f00-ab57-11eb-8846-22c7a3f96f30.png">


Bridging table for the Many to Many Relationship:

<img width="602" alt="Screen Shot 2021-05-02 at 3 07 11 PM" src="https://user-images.githubusercontent.com/73371470/116804218-130ca680-ab58-11eb-9ca9-b30cbc828839.png">



*Entity Class*
Member Class

- @Entity

The JPA specification required the @Entity annotation because it indentifies a class as a entity class:

<img width="370" alt="Screen Shot 2021-05-02 at 3 09 12 PM" src="https://user-images.githubusercontent.com/73371470/116804256-5bc45f80-ab58-11eb-8f94-5efa0bb6aabf.png">

- @Id

The JPA and Hibernate required me to specify a primary key attribute for each entity, and I did this by annotating an attribute with the @Id notation:

<img width="372" alt="Screen Shot 2021-05-02 at 3 11 10 PM" src="https://user-images.githubusercontent.com/73371470/116804287-a219be80-ab58-11eb-95b8-a9518dc46f17.png">

- @GeneratedValue

When a primary key is specified, the sequences and the auto-incremented database cloumns also has to be specified.

Also, the 2 most frequently used DB generates unique primary key values:

<img width="370" alt="Screen Shot 2021-05-02 at 3 13 00 PM" src="https://user-images.githubusercontent.com/73371470/116804334-e3aa6980-ab58-11eb-83cb-d528055431c4.png">


- @Getter and @Setter

A field is annotated with the @Getter and @Setter, which allows the lombok to automatically generate the default getter and setter:

<img width="365" alt="Screen Shot 2021-05-02 at 3 14 30 PM" src="https://user-images.githubusercontent.com/73371470/116804361-194f5280-ab59-11eb-8ea6-5e8443d0c8a7.png">



*Repository Class & Entity Manager*

<img width="605" alt="Screen Shot 2021-05-02 at 3 14 59 PM" src="https://user-images.githubusercontent.com/73371470/116804376-29ffc880-ab59-11eb-9c4a-28b0766d9019.png">

- @Persistence context

The transaction persistence context is bound to the transaction

Also, the entities contained in the persistence context are flushed into the persistent storage(DB) when the transaction finishes:

<img width="532" alt="Screen Shot 2021-05-02 at 3 16 42 PM" src="https://user-images.githubusercontent.com/73371470/116804401-67645600-ab59-11eb-98ac-0a6457553f7b.png">


- @Repository

The @Repository is a Spring notation which indicates the decorated class of a repository

Moreover, a repository is a mechanism for encapsulating storage, retrieval and the search behavior which emulates a collection of a object 

Also, the @Repository specializes the @Component notaion because it allows the @Component
to implement classes which is autodetected through a classpath scan:

<img width="605" alt="Screen Shot 2021-05-02 at 3 20 31 PM" src="https://user-images.githubusercontent.com/73371470/116804458-efe2f680-ab59-11eb-9028-cac7df045a3e.png">

- ## **Day 6**


Today, I have brain stormed for a significant amount of time on deciding a project to work on for the next semester. I listed out ubiquitous parts of humanity, like schools, jobs, tech, etc, then I research about the flaws of the prominate factors of life in order to create a service that can secure the flaws. However, several ideas were already innovated to secure any flaws or inconvenience. Therefore, I moved on to making a service which is approachable by all individuals in order to increase clients.

- Coding Idea

*Music:*

Emotion choosing (when the web or app is opened), then recommending a list of songs

Or

Weather API of location, then recommending songs relevant to the weather

But, the topic does not have to be limited to music, the emotion and weather values can output another topic, like videos, etc


- ## **Day 7**


- ### IOS
As, I finished brainstorming my topic/idea, I began to design and construct my client by using a application called sketch. First I download sketch, then began to adapt myself to the environment. Moreover, the UI of the application was explicit and coherent; therefore, I was able to accelerate my process of constructing my client. In order to display my plan I began by outlining specific pages for the client.
- sign up

When the user enters the application, the server directs them to the sign up page where they have to enter their name, emial, username and password. Then, if the user clicks the sign up button, the prototype directs the client to the login page

<img width="193" alt="Screen Shot 2021-05-16 at 11 49 30 AM" src="https://user-images.githubusercontent.com/73371470/118383869-ca1b1e80-b63c-11eb-8d94-6b9dcaf89f5c.png">

- longin

When the client enters the login page, they have to enter their username and password established on the signup page to continue. Then, if the client clicks the login button, the prototype directs the client to the main page

<img width="215" alt="Screen Shot 2021-05-16 at 11 50 09 AM" src="https://user-images.githubusercontent.com/73371470/118383878-e0c17580-b63c-11eb-9265-05eab0275bdb.png">

- main 

The main page contains the weather API and the mood checker, where the client chooses a specific mood, so that the server that recommend a playlist according to the mood. There are 3 different moods: happy, sad and angry, and when the client clicks on one of them the server directs them to the detail page.

<img width="197" alt="Screen Shot 2021-05-16 at 11 50 25 AM" src="https://user-images.githubusercontent.com/73371470/118383881-e919b080-b63c-11eb-8052-0a7cf640a583.png">

- details
The detail page displays the list of songs according to the mood, and provides a mini-player on the bottom of the page in order to allow the client to understand what song they are currently listening to.

<img width="205" alt="Screen Shot 2021-05-16 at 11 50 34 AM" src="https://user-images.githubusercontent.com/73371470/118383884-ef0f9180-b63c-11eb-89aa-8d131cd129af.png">

- IOS page:

<img width="811" alt="Screen Shot 2021-05-16 at 11 51 06 AM" src="https://user-images.githubusercontent.com/73371470/118383891-0189cb00-b63d-11eb-8eb1-5f9308eee62a.png">


- ### PC or Tablet

However, this design is only limited to IOS users, therefore, I formed another format for pc or ipad users.
The design contains all aspects, functions and pages stated above, but with some additional pages that enhance the convenience of the service. 
Additional pages:
- playlist choosing page

the choosing page is directed to the user depending on what mood they chose. The page recommends several playlists and allows the client to search for specific sons. Moreover, the page has a section on top and if the client clicks on that button the page directs the client to the mood page, so that the client can change their mood status. 

<img width="501" alt="Screen Shot 2021-05-16 at 11 51 22 AM" src="https://user-images.githubusercontent.com/73371470/118383897-0c446000-b63d-11eb-87a7-e8bd6704a6bc.png">

- mini player page

As said before the detail page includes a mini-player on the bottom, and this page extends the mini-player when clicked on. The page includes basic information on their mood status, song, and how much the song durated. Moreover, the bottom section allows the user to rewind, pause/start or skip the song.

<img width="550" alt="Screen Shot 2021-05-16 at 11 51 37 AM" src="https://user-images.githubusercontent.com/73371470/118383903-149c9b00-b63d-11eb-9841-35dd079b6993.png">


- PC page:

<img width="1076" alt="Screen Shot 2021-05-16 at 11 52 19 AM" src="https://user-images.githubusercontent.com/73371470/118383913-2ed67900-b63d-11eb-935e-f35f90f161c8.png">


- ## **Day 8**

As I finished creating an outline sketch of the client design, I installed the DB designer to outline the server side. 

<img width="840" alt="Screen Shot 2021-06-06 at 9 38 03 AM" src="https://user-images.githubusercontent.com/73371470/120908976-e72a9680-c6aa-11eb-9288-d7a72a45ddc5.png">

Then, I created the member and order table in conjunction with integrating a primary and Foreign Key because unique values are crucial to uniquely identify all table records. However, a table can only contain one primary key without a null value because the key organizes the sequence of the clustered index. Moreover, the primary key can interconnect with foreign keys.

The foreign key acts as a bridge that links data between two tables because it acts as a cross-reference. Foreign keys generate after the creation of primary keys.

<img width="595" alt="Screen Shot 2021-06-06 at 9 46 20 AM" src="https://user-images.githubusercontent.com/73371470/120909073-0d9d0180-c6ac-11eb-9b85-90646e79f17f.png">

- Member Table
- Order Table
- Item Table
- OrderItem Table (Join Table)
- OrderStatus Table

<img width="677" alt="Screen Shot 2021-06-06 at 9 47 52 AM" src="https://user-images.githubusercontent.com/73371470/120909086-43da8100-c6ac-11eb-9f40-c64a2e2a0e4d.png">

After finishing the outline I created the Memeber and Order Entity Class:

<img width="170" alt="Screen Shot 2021-06-06 at 9 49 48 AM" src="https://user-images.githubusercontent.com/73371470/120909110-88feb300-c6ac-11eb-90a7-f705575e0584.png">
<img width="661" alt="Screen Shot 2021-06-06 at 9 48 51 AM" src="https://user-images.githubusercontent.com/73371470/120909099-68365d80-c6ac-11eb-9264-17603003156a.png">

Then, the Modify Order and Creat OrderStatus Entity Class:

<img width="639" alt="Screen Shot 2021-06-06 at 9 49 37 AM" src="https://user-images.githubusercontent.com/73371470/120909107-83a16880-c6ac-11eb-9f2f-2daa252edaf5.png">



Item Entity Class:

<img width="615" alt="Screen Shot 2021-06-06 at 9 50 33 AM" src="https://user-images.githubusercontent.com/73371470/120909116-a3d12780-c6ac-11eb-901c-350b415c7ddf.png">


OrderItem (Join Table) and Modify Order Entity Class:

<img width="683" alt="Screen Shot 2021-06-06 at 9 51 11 AM" src="https://user-images.githubusercontent.com/73371470/120909124-bba8ab80-c6ac-11eb-92be-a596de8c78d2.png">



- ## **Day 9**

Today I advanced forward to repository and test case classes as they are curical to outline item entity classes. 

- Member Repository
- Item Repository
- OrderStatus Repository
- OrderItem Repository 
- Order Repository


As there are 5 item entity classes, it is the same for the repository case. 

- Item Repository

<img width="425" alt="Screen Shot 2021-06-13 at 1 05 05 PM" src="https://user-images.githubusercontent.com/73371470/121795049-fa5bda00-cc47-11eb-8f25-59256a6073a4.png">

- OrderStatus Repository

<img width="641" alt="Screen Shot 2021-06-13 at 1 12 13 PM" src="https://user-images.githubusercontent.com/73371470/121795149-f9777800-cc48-11eb-85b6-fd2bfa9dee1d.png">

- OrderItem Repository 

<img width="664" alt="Screen Shot 2021-06-13 at 1 14 52 PM" src="https://user-images.githubusercontent.com/73371470/121795181-58d58800-cc49-11eb-905f-d801e4e6ecb7.png">

- Order Repository
<img width="433" alt="Screen Shot 2021-06-13 at 1 16 45 PM" src="https://user-images.githubusercontent.com/73371470/121795216-9afec980-cc49-11eb-9a20-75b4585bbe85.png">


- ### Test cases

As test cases are correlated to the repository it will be logical to include test cases for all repositories.

- Item Repository

<img width="493" alt="Screen Shot 2021-06-13 at 1 37 15 PM" src="https://user-images.githubusercontent.com/73371470/121795497-78ba7b00-cc4c-11eb-9ffc-2e0f481fb14b.png">

<img width="514" alt="Screen Shot 2021-06-13 at 1 37 22 PM" src="https://user-images.githubusercontent.com/73371470/121795503-7ce69880-cc4c-11eb-9b2f-0748f98ee3db.png">

<img width="513" alt="Screen Shot 2021-06-13 at 1 37 39 PM" src="https://user-images.githubusercontent.com/73371470/121795507-86700080-cc4c-11eb-9d0d-a472ff9800a1.png">

- OrderStatus Repository

<img width="552" alt="Screen Shot 2021-06-13 at 1 37 53 PM" src="https://user-images.githubusercontent.com/73371470/121795515-8ec83b80-cc4c-11eb-9963-8787ea1f3c1c.png">

<img width="608" alt="Screen Shot 2021-06-13 at 1 39 32 PM" src="https://user-images.githubusercontent.com/73371470/121795544-cafb9c00-cc4c-11eb-9218-ed0eb3c55a39.png">

<img width="569" alt="Screen Shot 2021-06-13 at 1 39 47 PM" src="https://user-images.githubusercontent.com/73371470/121795545-d2bb4080-cc4c-11eb-9658-c00f5d04a9bc.png">

- Order Repository


- ## **Day 10**

Today I touched upon the @Repository classes and JUnit Test cases (partially), in particular - the test cases - the JUnit, as it is crucial for a pre-emptive solution for potential faliures. Again, this applies to all five facets:

- Member Repository
- Item Repository
- OrderStatus Repository
- OrderItem Repository 
- Order Repository


Creating:

- Item Repository Class

<img width="426" alt="Screen Shot 2021-06-27 at 11 37 41 AM" src="https://user-images.githubusercontent.com/73371470/123531048-15e0dd80-d73c-11eb-8435-9eafea978502.png">

- OrderStatus Repository Class

<img width="642" alt="Screen Shot 2021-06-27 at 11 38 21 AM" src="https://user-images.githubusercontent.com/73371470/123531052-2e50f800-d73c-11eb-8af1-c2c33f295a5b.png">

- OrderItem Repository Class

<img width="663" alt="Screen Shot 2021-06-27 at 11 38 53 AM" src="https://user-images.githubusercontent.com/73371470/123531061-4163c800-d73c-11eb-89b1-2f044dd8ac86.png">

- Order Repository Class

<img width="434" alt="Screen Shot 2021-06-27 at 11 39 18 AM" src="https://user-images.githubusercontent.com/73371470/123531069-4fb1e400-d73c-11eb-8785-9fe6fbea8515.png">

- Item Repository Test Case

<img width="487" alt="Screen Shot 2021-06-27 at 11 40 24 AM" src="https://user-images.githubusercontent.com/73371470/123531085-7708b100-d73c-11eb-92bf-1ea8abb99339.png">


<img width="512" alt="Screen Shot 2021-06-27 at 11 40 32 AM" src="https://user-images.githubusercontent.com/73371470/123531088-7c65fb80-d73c-11eb-84c6-8ed2a0489103.png">


<img width="512" alt="Screen Shot 2021-06-27 at 11 40 40 AM" src="https://user-images.githubusercontent.com/73371470/123531090-825bdc80-d73c-11eb-9ca4-5d2db87cbd91.png">


hello


