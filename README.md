# flask
Flask session handled on 30/10/2019

Pre Requisties
--Python3
--Pip3
--Flask

sudo apt-install 
python3 --version
pip3 --version

mkdir firstFlask
cd firstFlask

pip3 install virtualenv 
Work with other people and not stick on with any local PC instead just install requirements

virtualenv VEnvironment
source VEnvironment/bin/activate

pip3 install Flask

gedit webapp.py

from flask import Flask
app = Flask(__name__)
@app.route('/')
def index():
  return "PESCians !!!"
if __name__ == "__main__":
  app.run(debug=True)

python3 webapp.py
starts webserver in localhost at port 5000

from flask import Flask, render_template
app = Flask(__name__)
@app.route('/')
def home():
  return render_template('home.html')
if __name__ == "__main__":
  app.run(debug=True)

gedit home.html

<!DOCKTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Home Page</title>
</head>
<body>
  Hello PESCians!!!
</body>
</html>

Them lets have fun in html for a while.
