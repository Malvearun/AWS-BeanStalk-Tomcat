# AWS-BeanStalk-Tomcat

•	Browse the link for generating Spring Boot war file creation, in order to deploy inside the container.  

Link: https://start.spring.io/

•	Please select the project(Maven/Gradle), language(Java/Kotlin/Groovy) and Spring Boot version.

Group: com.tomcat
Artifact: AWS-BeanStalk-Tomcat
Search for dependencies: web, actuator
Name: AWS-BeanStalk-Tomcat
Description: Demo project for Spring Boot
Package Name: com.tomcat.AWS-BeanStalk-Tomcat
Packaging: War
Java Version: 8/11/14

•	Click on `Generate` to generate the Spring Boot application of type war file. You may open in the Intellij or visual studio.

•	Creating the WAR file in Spring Boot may add another file with exampleController.java under Java folder with `public class`.

•	Configure package to war format.

### Creating and deploying Elastic Beanstalk with Tomcat:

•	Login to AWS Console  Service  Elastic BeanStalk  Create Application   Get Started 

•	Create environment  Select Web server environment 

•	Environment / Application Name: `Hello-Tomcat`

•	Domain: will replace with same `Environment Name`

•	Base Configuration: 
1.	Platform: PreConfigured platform – EC2 instance will be create and tomcat will be added to the container.
2.	Select `Tomcat`, Platform branch and Platform version can be selected has per the project requirement.
3.	Application Code:
o	Select `upload you code`  browse the source file `S3 URL` or locally  under `target` folder  .war file  upload 
o	Reference files for the project are injected in GitHub repository: https://github.com/Malvearun/AWS-BeanStalk-Tomcat.git
o	Should see it will be tagged with the name.
o	Click on `Create application /environment`.

