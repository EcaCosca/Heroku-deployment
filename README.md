# Heroku-deployment
Heroku deployment for class. Here we have a step by step guide you can follow any time you want to deploy your full stack aplication using Heroku.


Guide

1. Set up.
    1. Let's go to https://devcenter.heroku.com/articles/heroku-cli#download-and-install.
    Here is where you will find your installer corresponding to your operating system, follow instructions acordingly.
    2. Let's check on our heroku version and login to our account in the terminal.
### `heroku --version`

### `heroku login`

2. Back end.
    1. Inside your server file we will make sure to set up the port variable to use any prt avilable.
<img width="336" alt="Screen Shot 1443-04-12 at 2 22 04 PM" src="https://user-images.githubusercontent.com/63668672/142191448-ed925bba-c6ea-4194-a7c2-29d40c34cb99.png">
    2. Now let's tell our server that we need it to do something in particular once we are in Heroku. We need to link it to a folder that we are going to have in our front end after we run the command on step 3.
<img width="420" alt="Screen Shot 1443-04-12 at 2 28 10 PM" src="https://user-images.githubusercontent.com/63668672/142192390-153df10b-311a-403e-a79b-7e1b82fb3f73.png">
    3. Inside of our package.json
<img width="594" alt="Screen Shot 1443-04-12 at 2 30 42 PM" src="https://user-images.githubusercontent.com/63668672/142192739-45c19c61-22bf-404e-9936-30ca6d1bd494.png">

3. Front end.
    1. Let's get the enviorement ready.
### `npm run build`

4. Root folder for the project.
    1. Create a file called ".gitignore" inside of your root folder.
    2. inside of the file we are going to add the name of the files we don't want git to track anymore. In this case we are going to add the "node_modules"
    3. Open your terminal in the root directory of your project and now let's create our Heroku app.
### `heroku create <NAME>`
### `git add .`
### `git commit -m"<message>"`
   4. Let's try to run our heroku app locally and see what happens.
### `heroku local`
   5. Push it to our repo.
### `git push heroku master`
   6. Let's open and see.
### `heroku open`

