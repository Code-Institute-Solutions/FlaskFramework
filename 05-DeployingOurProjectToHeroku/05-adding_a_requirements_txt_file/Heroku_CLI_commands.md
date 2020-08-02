### Install Heroku within Gitpod:
- `npm install -g Heroku`


### Log In to Heroku:
- `heroku login -i`


### View your Heroku Apps:
- `heroku apps`


### Rename a Heroku App:
- `heroku apps:rename NEW-NAME --app CURRENT-APP-NAME`


### Deployed Heroku App URL:
- `https://YOUR-APP-NAME.herokuapp.com`


### View Verbose Git Remotes:
- `git remote -v`


### Creating Heroku Git Remote:
- go to Heroku Settings Tab
- copy **Heroku Git URL** link
- `git remote add heroku https://git.heroku.com/YOUR-APP-NAME.git`


### Push Code to Heroku Remote:
- `git push -u heroku master`


### Create a requirements.txt File:
- `pip3 freeze --local > requirements.txt`
