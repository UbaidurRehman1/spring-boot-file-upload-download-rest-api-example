## Spring Boot File Upload / Download Rest API Example

**Tutorial**: [Uploading an Downloading files with Spring Boot](https://www.callicoder.com/spring-boot-file-upload-download-rest-api-example/)

## Steps to Setup

**1. Clone the repository** 

```bash
git clone https://github.com/UbaidurRehman1/spring-boot-file-upload-download-rest-api-example.git
```

**2. Specify the file uploads directory**

Open `src/main/resources/application.properties` file and change the property `file.upload-dir` to the path where you want the uploaded files to be stored.

```
file.upload-dir=/tmp
```

**2. Run the app using maven**

```bash
cd spring-boot-file-upload-download-rest-api-example
mvn spring-boot:run
```

That's it! The application can be accessed at `http://localhost:8909`.