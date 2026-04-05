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




