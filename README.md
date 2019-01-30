# Hello World Flask 2

### Initialize a git repository
```bash
git init
```

### Create a virtual environment
```bash
virtualenv app_env
```

### Activate the virtualenv
```bash
source app_env/bin/activate
```

### Install dependencies
```bash
pip install flask
```

### Install more dependencies gunicorn
* necessary for deployment to heroku
* Flask's default server is not suitable for Production
http://flask.pocoo.org/docs/0.12/deploying/
```bash
pip install gunicorn
```

### Create a Procfile

* with the following line

web: gunicorn app:app

### List dependencies in requirements.txt

```bash
pip freeze > requirements.txt
```

# Install herokucli

* using brew

```bash
brew install heroku/brew/heroku
heroku login
heroku create
```

### Commmit the history in the git repository

```bash
git add . 
git commit -m 'Deploy to heroku'
```

### Push to Heroku as the remote 
```bash
git push heroku master
```

