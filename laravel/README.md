## Laravel Acornfile

##### TL: DR 
> Note : add the .env file inside the src dir . You can copy  .env.example and modify based on your requirement.
```
$ acorn run -n laravel .
```

Hi, we have developed a simple `TODO App` using Laravel framework and we have the AcornFile which can be used to deploy the Application on Kubernetes.

###### Steps:

- If you want to just deploy the application with defaults use below command
```
$ acorn run -n laravel .
```

- If you are developing your application an you don’t what to restart the pods everytime you make the changes you can simply use the acorn dev command which will run the Laravel Application in dev mode and all the changes will the reflected to the UI as soon as you save the file. 
```
$ acorn dev -n laravel .
```
As this Application just include the simple Hello world Application which can be easily customized based on your requirement . You can follow Laravel docs.

- [Getting Started](https://laravel.com/docs/10.x/installation)

Join the Acorn Community Slack

- [Slack](http://slack.acorn.io/)