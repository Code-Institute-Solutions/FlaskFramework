### To log into the Heroku toolbelt CLI:

1. Log in to your Heroku account and go to _Account Settings_ in the menu under your avatar.
2. Scroll down to the _API Key_ and click _Reveal_
3. Copy the key
4. In your IDE, from the terminal, run `heroku_config`
5. Paste in your API key when asked

You can now use the `heroku` CLI program - try running `heroku apps` to confirm it works. This API key is unique and private to you so do not share it. If you accidentally make it public then you can create a new one with _Regenerate API Key_.


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


### Remove Heroku Git Remote:
- `git remote rm heroku`


### Push Code to Heroku Remote:
- `git push -u heroku master`


### Create a requirements.txt File:
- `pip3 freeze --local > requirements.txt`


### Create a Heroku Procfile:
- `echo web: python run.py > Procfile`


### View Heroku Application Logs:
- `heroku logs --tail --app YOUR-APP-NAME`


### Add Environment Variables to Heroku:
- go to Heroku Settings Tab
- click **Reveal Config Vars**
- **key**: `IP` | **value**: `0.0.0.0`
- **key**: `PORT` | **value**: `5000`
- **key**: `SECRET_KEY` | **value**: `your_secret_key`


### Setup Automatic Deployments from GitHub:
- go to the Heroku Deploy Tab
- click **GitHub** for *Deployment Method*
- click **Connect to GitHub**
- provide your *GitHub repository* name, then click **Search**
- ensure all code is pushed to your GitHub repo
- click **Enable Automatic Deploys**
- click **Deploy Branch** on Heroku
