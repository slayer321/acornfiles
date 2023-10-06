## Laravel Acornfile

##### TL: DR  `acorn run -n laravel .`
```
acorn run -n laravel .
```

Hi, here we have the Simple Hello world `Laravel` framework Application and we are going to use Acornfile to deploy it on Kuberenetes.

###### Steps:

- If you want to just deploy the application with defaults use below command
```
acorn run -n laravel .
```

- You can check all the available Args by running `acorn run -n laravel . --help`
```
demo@demo:~/laravel $ acorn run -n laravel . --help

Volumes:   <none>
Secrets:   mysql-root-password, mysql-password
Containers: app, db, nginx
Ports:     app:9000/tcp, nginx:8000:80/http

      --mysql-db string            
      --mysql-passwd string        
      --mysql-root-passwd string   
      --mysql-user string          
  
```
- If you didn't pass the `--mysql-root-passwd`  and `--mysql-passwd` args a random token will be generated. 
- To cutomize the args 
```
$ acorn run -n laravel . --mysql-db "db" --mysql-passwd "secretpasswd" --mysql-root-passwd "secretrootpasswd" --mysql-user "test"
```

As this Application just include the simple Hello world Application which can be easily customized based on your requirement . You can follow Laravel docs.

- [Getting Started](https://laravel.com/docs/10.x/installation)

Join the Acorn Community Slack

- [Slack](http://slack.acorn.io/)