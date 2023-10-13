## Django Acornfile

Here we have the Simple `Voting App` using Django framework and we have the Acornfile which can be used to deploy it on Acorn SaaS Platform.


##### Deploying the App on SaaS Platform.
- First you need to login to saas platform using your github username.Once the Account is setup you need to click on create and select `from acorn image` where you need to select `name`, `region` and `Acron Image`. For Django below is the latest image
```
ghcr.io/infracloudio/django-acorn:v0.0.5
```
Once you click on `Create` , Provisioning starts and in some time your app is in Running state and you can access it using the given URL.

##### Checking App logs
- You can click on 4 dots on the right side of your app on the UI and click on View Logs through which you can see your app Logs.

##### Removing the App
- If you simply want to remove the App . Click on the 4 dots and select `Remove` which will remove your app.

As this Application just include the simple `Voting Poll` App which can be easily customized based on your requirement . You can follow Django docs.

- [Getting Started](https://docs.djangoproject.com/en/4.2/intro/tutorial01/)

Join the Acorn Community Slack

- [Slack](http://slack.acorn.io/)