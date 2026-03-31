## Task 1: The Problem

Think about a team of 5 developers all pushing code to the same repo manually deploying to production.



What can go wrong?

     - code conflict means two developer changing the same code and pushing it to production then client can face problem
     - Finds lot of bugs because there is no checking
     - The systematic workflow will break .
     
What does "it works on my machine" mean and why is it a real problem?

       - it work on my machine ,this cause the main issue that when you are doing code in your laptop you install and set-up all the things accordingly 
         ,but when it comes to production it fails because every machine has different settings , libraries or enviroment
       - so this is the real problem because code need to be work everywhere .
       
How many times a day can a team safely deploy manually?

      - Manual deployments are slow and risky.  
      - At best, a team might safely deploy **once a day** if they’re very careful.  
      - More frequent manual deployments increase the chance of errors and downtime.

For this we need to know CI/CD automation so it can check the code , run it and if get errors it will reflect that and after all the correction 
,it automatically deploy the code and here developer can change code anytime if they feel and after all the changes the process will repeat once
again ,no manual deploying easy and safe.


## Task 2: CI vs CD

Continuous Integration — what happens, how often, what it catches

     - Continuous Integration means developers regularly (daily or many times a day) add their code to a shared project.
       Each time code is added, it is automatically tested and checked.
       It helps to catch bugs early before they become big problems.
          
       What it catches:
          - Code errors
          - Integration issues (when different parts don’t work together)
          
       Real-world example:
          - A team pushes code to GitHub → GitHub Actions automatically runs tests → if something breaks, developer knows immediately.

Continuous Delivery — how it's different from CI, what "delivery" means

       - Continuous Delivery means after CI, the code is always kept ready to release.
         The system automatically builds and tests the app, but deployment is done manually.
         “Delivery” means the software is prepared and ready for production anytime.

       - Real-world example:
            After testing, the app is ready and waiting → team clicks a button to deploy on AWS or server. 

Continuous Deployment — how it differs from Delivery, when teams use it

       - After testing, the code is automatically deployed to users without manual approval.
         Every change goes live quickly.

       - Real-world example:
         You push code → tests pass → website updates automatically (like updates on Netflix or Facebook).  


## Task 3: Pipeline Anatomy

A pipeline has these parts — write what each one does:

Trigger — what starts the pipeline

      - Trigger is what starts the pipeline.

        Example:
          
          When you push code to GitHub
          When you create a pull request

Stage — a logical phase (build, test, deploy)

     - Stage is a big step or phase in the pipeline.

       Common stages:
          
          Build
          Test
          Deploy
          
Job — a unit of work inside a stage

    - Job is a task inside a stage.
    
Step — a single command or action inside a job

     - Smallest action (one command)
     
Runner — the machine that executes the job

    - it means each machine has runner to know in which server it will run like ubuntu server or self-hosted server
    
Artifact — output produced by a job

Trigger → Stage → Job → Step → Runner → Artifact


## Task 4: Draw a Pipeline

Draw a CI/CD pipeline for this scenario:

A developer pushes code to GitHub. The app is tested, built into a Docker image, and deployed to a staging server.

      - Go to the .github/workflow/scenario.yml



