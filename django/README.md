## Django Acornfile

##### TL: DR 
```
acorn run -n django .
```

Hi, here we have the Simple Hello world `Django` framework Application and we are going to use Acornfile to deploy it on Kuberenetes.

###### Steps:

- If you want to just deploy the application with defaults use below command
```
acorn run -n django .
```

- You can check all the available Args by running `acorn run -n django . --help`
```
demo@demo:~/django $ acorn run -n django . --help

Volumes:   <none>
Secrets:   <none>
Containers: web
Ports:     web:8000/http      
  
```
- Currently there is no such args added as it is by default using sqlite database. Which can be easily customized following this [docs](https://docs.djangoproject.com/en/4.2/intro/install/#set-up-a-database). 

- This Acornfile provide the feature to run Django Application in debug mode. If you run the application with this command `acorn dev -n django .`
You can see all the changes reflected to your application.

As this Application just include the simple Hello world Application which can be easily customized based on your requirement . You can follow Django docs.

- [Getting Started](https://docs.djangoproject.com/en/4.2/intro/tutorial01/)

Join the Acorn Community Slack

- [Slack](http://slack.acorn.io/)