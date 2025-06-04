## Introduction

Hello and welcome to our project. This project was a school project for our database course and we built it to take our first step in web development tool.
We hope that this project would help new developer to understand what software development is like.

## deployment

If you are looking to running this project, you can go to each README file in the submodule and work on it. You will be able to run it without a problem.

We had also deploy this project and it was our first time using google cloud. If you are interested in deploying please follow down the instruction


# Don't forget to install google cloud and login 

 Go to each submodule, you will find a dockerfile, build it using this command

## API

```bash
docker build -t <your-api-image> .
docker tag <your-api-image> ${your desired location}/${project name}/${repo}/{your repo folder}
docker push ${your desired location}/${project name}/${repo}/{your repo folder}
```
`
    Before deploying, set the env value and connect it a desired database. 
``
 
   *Note: We uses gcloud instance database in deploying this project. We had set it up and down below before deployment, it will asks to connect to a databsae on gcloud instance. If you like to uses it, create a database on it and add your socketPath on sequelize.config.ts file on config folder and replace the url socket.*

`
    After deployment you will get a url and replace the string to build to your web deployment

    WEB
```
    docker build --build-arg VITE_API_BASE_URL=${String} <your-web-image> .
    docker tag <your-web-image> ${your desired location}/${project name}/${repo}/{your repo folder}
    docker push ${your desired location}/${project name}/${repo}/{your repo folder}


HAPPY DEPLOYMENT

    ############################################################################################
    #THANK YOU FOR YOUR VISIT. PLEASE COME AND TAKE A LOOK ONCE IN A WHILE TO FIND NEW PROJECT.# 
    #                                   HAVE A NICE DAY                                        #
    ############################################################################################
