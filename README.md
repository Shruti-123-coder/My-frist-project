



create table if not exists books(barcode varchar(100) primary key, name varchar(100), author varchar(100), price int, quantity int);

create table if not exists users(username varchar(100) primary key,password varchar(100), firstname varchar(100), lastname varchar(100),address text, phone varchar(100),mailid varchar(100),usertype int);

insert into books values('9780134190563','The Go Programming Language','Alan A. A. Donovan and Brian W. Kernighan',400,8); insert into books values('9780133053036','C++ Primer','Stanley Lippman and Josée Lajoie and Barbara Moo',976,13); insert into books values('9781718500457','The Rust Programming Language','Steve Klabnik and Carol Nichols',560,12); insert into books values('9781491910740','Head First Java','Kathy Sierra and Bert Bates and Trisha Gee',754,23); insert into books values('9781492056300','Fluent Python','Luciano Ramalho',1014,5); insert into books values('9781720043997','The Road to Learn React','Robin Wieruch',239,18); insert into books values('9780132350884','Clean Code: A Handbook of Agile Software Craftsmanship','Robert C Martin',288,3); insert into books values('9780132181273','Domain-Driven Design','Eric Evans',560,28); insert into books values('9781951204006','A Programmers Guide to Computer Science','William Springer',188,4); insert into books values('9780316204552','The Soul of a New Machine','Tracy Kidder',293,30); insert into books values('9780132778046','Effective Java','Joshua Bloch',368,21); insert into books values('9781484255995','Practical Rust Projects','Shing Lyu',257,15); insert into users values('demo','demo','Demo','User','Demo Home','42502216225','demo@gmail.com',2); insert into users values('Admin','Admin','Mr.','Admin','Haldia WB','9584552224521','admin@gmail.com',1); insert into users values('shashi','shashi','Shashi','Raj','Bihar','1236547089','shashi@gmail.com',2);

commit;


### ========== Importing and Running The Project Through Eclipse EE ==========

Step 0: Open Eclipse Enterprise Edition. [Install, if not already installed.]

Step 1: Click On File > Import > Git > Projects From Git > Clone Uri > Paste The Repository Url as: ```https://github.com/shashirajraja/onlinebookstore.git```> Select master Branch > Next > Next > Finish.

Step 2. a: Go inside ```src/main/resources > application.properties``` and update the value of database details as per your usage, like db.driver, db.host, db.username and db.password according to your installed mysql/postgresql admin user credentials.

Step 2.b: Right Click on Project > Run as > Maven Build > In the goals field enter "clean install" > apply > run

Step 2.c: Right Click On Project > Build Path > Configure Build Path > Libraries > Remove and Update Any Libraries if Red Mark Exists > Finish.

Step 3: [Only If Tomcat Server is not configured in Eclipse] : Right Click On Project > Run As > Run On Server > Select Tomcat V8.0 > (Select Tomcat V8.0 Installation Location If Asked) Next > Add onlinebookstore > Finish.

Step 4: In The Server Tab > Double Click On Tomcat Server > Ports > Change The Port Number For Http/1.1 To 8083 > Close And Save.

Step 5: Right Click On Project > Run As > Run On Server > Select Tomcat v8.0 > Next > Add All> Done.

Step 6: Check Running The Site At  <a href="http://localhost:8083/onlinebookstore/">http://localhost:8083/onlinebookstore/</a>



## FAQ
**Question:1** Unable to Connect to Database?

**Answer:** Please check you have installed the mysql correctly and have updated the correct db details in application.properties file. Also you can try doing maven clean install and force update the project and restart.
<hr>

Note:- Considering this as a Sample Project, we have not much considered of web security.
#### Some Screenshots for the project:
<img width="941" alt="image" src="https://user-images.githubusercontent.com/34605595/224769637-37c34d4b-26e7-4d49-b990-4c09b260ec31.png">
<img width="954" alt="image" src="https://user-images.githubusercontent.com/34605595/224769990-f440f74d-41b2-4629-ba1c-a87267f225d9.png">
<img width="930" alt="image" src="https://user-images.githubusercontent.com/34605595/224770145-5902054f-5943-44ac-b02f-92097c8a6972.png">
<img width="934" alt="image" src="https://user-images.githubusercontent.com/34605595/224770257-e18a3810-0457-4b78-bf46-cf82746708ee.png">
<img width="946" alt="image" src="https://user-images.githubusercontent.com/34605595/224770392-5a5478d2-98cc-44ee-8689-132b6b16af80.png">


#### "Suggestions and project improvement ideas are welcomed!"

<bold>Thanks a lot,</bold><br/>
                                                                                                        Project Leader<br/>
                     
