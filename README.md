### Deploying (create-react-app) to Heroku

### App Preview (Deployed to Heroku)
https://lit-falls-80508.herokuapp.com/

### Why We Need Heroku At first Place
Heroku is the platform as a service (pass). It enables developers to build, run and operate there apps entirely in the cloud.[https://www.heroku.com/]. In other words we can describe as the online server where we can preview our developed app, and show it to concerned users. 

## Deploying Steps
We will create a simple app that displays helloworld. actually the main idea is to make you familier with steps to deploy project to heroku. I've refered https://blog.heroku.com/deploying-react-with-zero-configuration which provides the comprehensive guide. 

#Step1
install heroku cli, in this case we are using it for windows therefore download & install it from https://devcenter.heroku.com/articles/heroku-cli

#Step2
create account at www.heroku.com

#Step3
once installed open up the command prompt and run
heroku --version

this command will verify the installation by displaying the heroku version.

#Step4
once installation is verified then run
heroku login
provide your login account credentials

#Step5
run
create-react-app <projectname>

#Step6
in order to initialize it for github run
git init  
by doing this you can later upload your project to github

#Step7
then run following build pack
heroku create -b https://github.com/mars/create-react-app-buildpack.git
Above build will let heroku know that this is app generated by create-react-app generator.

#Step8
run 
git add .
this will ready your files to be added to heroku

#Step9
run 
git commit -m "V1"

#Step10
run
git push heroku master
This command will push your app files to heroku

#Step11
finally run
heroku open
to see the preview of your app.




