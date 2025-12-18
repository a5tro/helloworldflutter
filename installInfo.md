installInfo.md
C:\dev\helloworldflutter\installInfo.md
git config --global user.name "a5tro"
git config --global user.email "mathieua@gmail.com"

# install gh if needed, then:
gh auth login --hostname github.com --web
# or run interactively:
gh auth login

git config --global credential.helper manager-core
# then perform an authenticated action (push/pull) and follow the browser prompt:
git push -u origin main

# Inspect current remotes
git remote -v

# If the URL is wrong, set the correct origin URL
git remote set-url origin https://github.com/a5tro/helloworldflutter.git

# If the repo doesn't exist, create it on GitHub, then push
git push -u origin main

git branch --set-upstream-to=origin/main main

git fetch origin
git merge origin/main --allow-unrelated-histories
