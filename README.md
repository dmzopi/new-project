Git instruction:

1. In console create and enter project folder
mkdir new-project && cd new-project
2. Initialize local git repository, ensure basic config
git init
git config --global user.name "Your Name"
git config --global user.email "your_email@whatever.com"
git config --global init.defaultBranch main
3. Attach remote repository
git remote add origin https://github.com/dmzopi/new-project.git
4. Fetch recent code
git fetch origin
5. Switch to "main" branch, check recent code
git switch main
6. Create "development" branch from "main" branch
git switch -c development
7. Make code changes and commit them using Smart Commit format (https://support.atlassian.com/jira-software-cloud/docs/process-issues-with-smart-commits/#Smart-Commit-commands)
git add . && git commit -m "PROM-42164 #comment Instructions added to README.md"
8. Merge changes to "main"
git switch main && git merge development
9. Push changes to remote
git push -u origin main