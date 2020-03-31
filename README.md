# Your Project Name 

## Checklist
- [ ] Check your mail and accept Github Repository invitation for edit access.
- [ ] Clone your project github repository 
- [ ] Import Project in Eclipse
- [ ] Configure Tomcat Server in Eclipse
- [ ] Run Web Application
- [ ] Test Web Application


#### Step 1: Clone Repository

```code
git clone https://github.com/csy-fresher-batch-2019/{yourproject-reponame}/.git
```

#### Step 2: Import Maven Project
```
Eclipse => File -> Import -> Existing Maven Projects -> Select Project Folder
```
Note: It will take few minutes ~1-3 minutes to import maven projects and download project dependencies.

#### Step 3: Build the Project
```code
mvn install
```
(or)
```
Run As -> Maven Install 
```
Note: Test whether build is successful.

#### Step 3.1 JRE Error
* Eclipse => Window Preferences => Java => Installed JRE => Change JRE Path to JDK path

#### Step 4: Update pom.xml and commit the files and push to github

* Update groupId, artifactId and name based on your project.
```code
 <groupId>com.naresh</groupId>
  <artifactId>myapp-web</artifactId>
  <version>1.0-SNAPSHOT</version>
  <name>myapp-web</name>
  ```
  to
  ```
 <groupId>com.prabhu</groupId>
  <artifactId>bankapp-web</artifactId>
  <version>1.0-SNAPSHOT</version>
  <name>bankapp-web</name>
  ```
  
#### Step 5: Download Tomcat WebServer
* Apache Tomcat 
* http://apachemirror.wuchna.com/tomcat/tomcat-9/v9.0.33/bin/apache-tomcat-9.0.33.zip
* Download and Extract folder ( Move tomcat to some folder e.g: D:\Softwares\apache-tomcat-9.0.33 )

#### Step 6: Configure Tomcat Server in Eclipse

* Windows => Show View -> Servers => New Server => Choose Apache => Tomcat 9.0 => Enter Tomcat Path - D:\Softwares\apache-tomcat-9.0.33

#### Step 6.1 : Test Tomcat Server
*  Try Start/Stop/Restart Server

#### Step 6.2: Error - Port 8080 already used
*  Modify port to 8081 in server.xml

#### Step 7: Test your web application
* Run As => Web Server
* Test => Servlet (HelloworldServlet, WelcomeServlet )  and JSP ( index.jsp )

