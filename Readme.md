## Spring Boot File Upload

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

## Uploading file

1. trigger ngrok with your subdomain by `ngrok http -subdomain=${subdomain} 8909`
2. cURL command to upload file: `curl --location --request POST 'http://${subdomain}.ngrok.io/uploadFile' --form 'file=@"path/to/file"'`
3. You can download file by: `curl ${fileDownloadUri} -o ${fileName}` where we can get `fileDownloadUri` and `fileName` from #2 command response

