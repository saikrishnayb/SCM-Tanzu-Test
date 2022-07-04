# SCM-Tanzu-Test

This repo provides a simple Hello World sample project for Spring Boot.

It can be deployed as a standalone web app, as a Cloud Foundy app or as a TAP workload, depending on the deployment option choosen when generating the project.

## Deployment

### Standalone app with embedded Tomcat server

You can build the project using Maven:

```bash
./mvnw clean package
```

To run the app using the embedded Tomcat server you can run this command:

```bash
./mvnw spring-boot:run
```

You can modify the default message "World" using an application property of `app.message`:

```bash
./mvnw package  
java -jar target/SCM-Tanzu-Test-0.0.1-SNAPSHOT.jar --app.message=Test
```

### Pushing to Cloud Foundry

You can deploy and use the `config/manifest.yml` file to set the initial message:

```bash
./mvnw package  
cf push SCM-Tanzu-Test -p target/SCM-Tanzu-Test-0.0.1-SNAPSHOT.jar -f config/manifest.yml --random-route
```

When deploying without the `manifest.yml` you can use the following commands:

```bash
./mvnw package  
cf push SCM-Tanzu-Test -p target/SCM-Tanzu-Test-0.0.1-SNAPSHOT.jar --random-route
```

Then, when you want to update the message you can set the env var `APP_MESSAGE` using:

```
cf set-env SCM-Tanzu-Test APP_MESSAGE 'Cloud Foundry'
cf restage SCM-Tanzu-Test
```

### Accessing the deployed app

Determine the route for the app by running:

```
cf app SCM-Tanzu-Test
```

Then, use `curl` or some other utility to access the route:

```
curl <route-for-SCM-Tanzu-Test>
```

### Deleting the Cloud Foundy app

You can delete the running app using:

```
cf delete SCM-Tanzu-Test
```
