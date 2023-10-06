## ROR Acornfile

##### TL: DR  `acorn run -n ror .`
```
acorn run -n ror .
```

Hi, here we have the Simple Hello world `Ruby on Rails` framework Application and we are going to use Acornfile to deploy it on Kuberenetes.

###### Steps:

- If you want to just deploy the application with defaults use below command
```
acorn run -n ror .
```

- You can check all the available Args by running `acorn run -n ror . --help`
```
demo@demo:~/ror $ acorn run -n ror . --help

Volumes:   <none>
Secrets:   postgres-password
Containers: web, db
Ports:     db:5432/tcp, web:3000/http

      --postgres-host string     
      --postgres-passwd string   
      --postgres-user string     
```
- If you didn't pass the `--postgres-passwd` args a random token will be generated. 
- To cutomize the args 
```
$ acorn run -n ror . --postgres-host "db" --postgres-passwd "mysecretpassword" --postgres-user "postgres"
```

As this Application just include the simple Hello world Application which can be easily customized based on your requirement . You can follow all the Ruby on Rails docs.

- [Getting Started](https://guides.rubyonrails.org/getting_started.html)

Join the Acorn Community Slack

- [Slack](http://slack.acorn.io/)