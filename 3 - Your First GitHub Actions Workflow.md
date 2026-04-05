## Task 1: Set Up

Create a new public GitHub repository called github-actions-practice

Clone it locally
     - git clone repo url

     - Good way to clone is to use the ssh key

Create the folder structure: .github/workflows/


## Task 2: Hello Workflow

Create .github/workflows/hello.yml with a workflow that:

Triggers on every push
Has one job called greet
Runs on ubuntu-latest
Has two steps:
Step 1: Check out the code using actions/checkout
  
     - I uae this in my yml file after words i remove it because actions/checkout@v4 is used when you are using any code , not for 
       only writing commands.

Step 2: Print Hello from GitHub Actions!

You can go to .github/workflows/hello.yml to check the code


## Task 3: Understand the Anatomy

Look at your workflow file and write in your notes what each key does:

on: it use for trigger the things
    - Like when you use 
               on:
                path:
                  branches: [main]
      - here anything you put or do cahnges it automatically run the file

     - Another one is there
                on:
                 workflow-dispatch:
        - It start running when you go to action and go to your file path /name and then hit the    
           "run the workflow" then it will start.

jobs: these are the tasks which we going to follow to complete the pipeline

runs-on: it uses to machine know that in which server it going to run

steps: commands / actions to complete the task

uses: used to call pre-build actions

run: it execute the command

name: (on a step) : for display


