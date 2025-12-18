git config --global user.name "a5tro"
git config --global user.email "mathieua@gmail.com"

# install gh if needed, then:
gh auth login --hostname github.com --web
# or run interactively:
gh auth login

git config --global credential.helper manager-core
# then perform an authenticated action (push/pull) and follow the browser prompt:
git push -u origin main