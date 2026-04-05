## Task 1: Trigger on Pull Request

          -  Create .github/workflows/pr-check.yml
          -  Trigger it only when a pull request is opened or updated against main
          -  Add a step that prints: PR check running for branch: <branch name>

          = Here in PR check running for branch: <branch name> ,the place of branch name i write ${{github.head_ref}}
            because when the pull request will done by any other branch it show the logs will always say "PR check running for branch: main.

            And also during the debugging time we will face problem ,if bug occur we can't find the actual problem.

          = When if use github.head-ref then GitHub Actions acts like a template. When you open a PR from dev-branch, 
            GitHub replaces that variable with dev-branch. If your teammate opens a PR from cool-feature, it replaces it with cool-feature. 

Create a new branch, push a commit, and open a PR

Watch the workflow run automatically

## Task 2: Scheduled Trigger

Add a schedule: trigger to any workflow using cron syntax

           - Cron syntax consists of 5 fields:

                Minute  Hour  Day_of_Month  Month  Day_of_Week

                How 0 0 * * * works:
                0: At the 0th minute.

                0: At the 0th hour (Midnight).

                *** *** ***: Every day, every month, every day of the week

Set it to run every day at midnight UTC

            - Cron ' 0 0 * * * '

Write in your notes: What is the cron expression for every Monday at 9 AM?

            - Cron '0 9 * * 1'


## Task 3: Manual Trigger

Create .github/workflows/manual.yml with a workflow_dispatch: trigger
Add an input that asks for an environment name (staging/production)
Print the input value in a step

         - You can go to .github/workflows/manual.yml


         - Here I use the enviroment , this typically a placeholder that swap itself when user choose something or select option

           Like an example:-
              - you as a customer go to resturent and hold the tabelet to select menu maually
              - it contain some input like what you want with their specific options
              - when you choose the options or if you don't choose they set some default options too (if you confuse or you don't want to choose)
              - after all this you send the message to kitchen what they will see ex -{want medium baked food}in their ticket

              This is how enviroment work.
              
Go to the Actions tab → find the workflow → click Run workflow            




