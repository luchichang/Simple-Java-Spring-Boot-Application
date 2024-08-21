# Simple-Java-Spring-Boot-Application

This application is designed for practicing the deployment process for Java Spring Boot-based applications.

## Instructions

1. **Clone the Repository:**

   Clone this repository using:
   ```bash
   git clone https://github.com/luchichang/Simple-Java-Spring-Boot-Application.git

2. **Install Apache Maven:**
       Apache Maven is used as the build automation tool for this application. If Maven is not already installed, follow the official installation guide.

       Maven is a build automation tool primarily for Java projects.
3. **Build the Application:**

    Navigate to the project directory and run:

```bash
    mvn clean package
```
   This command performs the following actions:
       * clean: Removes previously compiled code and build artifacts to ensure a fresh build.
       * package: Compiles the code, runs tests, and packages the application into a JAR or WAR file as specified in the pom.xml file.

4. **Run the Application:**
 ### Locally
     After the build process completes, the generated .jar file will be located in the target directory. To run the application, use:

```bash
java -jar target/spring-boot-web.jar
```
 The application will start and be accessible at http://localhost:8080.

 ### Through Containerization Approach

       build the Image in the docker file

```docker
       docker build -t basicspringbootapp:v1 .
```
      run the container and forward the application to  port  8010

      ```docker
      docker run -d --name container1 -p "8010:8080" basicspringbootapp:v1
      ```


5. **Optional:**

   For a visual reference, you can view the attached image:
     <a>![image](https://github.com/user-attachments/assets/53aef5f0-5569-49ba-9bd9-498dc9d55a59)
     <a/>

     Project Credits: https://github.com/iam-veeramalla
