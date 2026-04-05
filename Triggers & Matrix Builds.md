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