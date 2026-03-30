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



