# Github guide

## First Setup
### CLI
- `git config --global user.email calumlindsay.434c@gmail.com`
- `git config --global user.name "Calum Lindsay"`
### Repository
- Create the new repository on github.com
- Open local folder where repo will be downloaded
- Enter `git init`
- Enter `git remote add origin https://github.com/username/repositoryname.git`
- Run command `git config --global credential.helper store`
- Go to github and generate a new PAT
- When you first push or pull you will be asked to log in or use your PAT
- If you chose to create a default README.md
	- Enter git pull origin main
- Your repository is now ready to be used!
---
## How To Regenerate PAT
- Github sends an email with a link close to the token running out
- Go to github and generate a new PAT
- Enter `echo url=https://cogilv25@github.com | git credential reject` into the console
- Next time you push you will be asked to log in or use your PAT
---
## Updating submodules to upstream version
- git submodule update --remote --merge `[path to submodule]`
- To do all submodules at once use:
	- git submodule update --remote --merge --recursive