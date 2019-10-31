# flask
Flask session handled on 30/10/2019 and 31/10/2019

Pre Requisties
--Python3
--Pip3
--Flask

Installation :
step1: Go to https://www.python.org/ftp/python/3.8.0/python-3.8.0-amd64.exe # It will download python3 in your machine.
step2: Run the installer, dont forget to check the path below
step3: select custom installtion (advised) -> next -> install to all users -> install # This will install python on all user account on a machine
step4: Go to command prompt by pressing "super key(windows key) + r" a prompt will pop up -> type cmd -> ok # Command prompt will popup
step5: python --version # If a value is returned "python 3.6" we have python
step6: go to https://bootstrap.pypa.io/get-pip.py -> copy the content by pressing "control+a" -> paste it in new notepad file -> save the file as "get-pip.py" and saveas type should be "all files" and save the file in a directory you know say desktop(use drop down)
step7: go to cmd prompt -> since our file is in desktop type "cd Desktop" -> python get-pip.py # This will install pip
step8: pip install flask
step9: go to desktop -> create a new folder -> in the folder create a new file -> save the file as run.py (dont forget to check saveas type as "all files" ).
step10: In the file run.py type the below code
from flask import Flask

app = Flask(__name__)

@app.route('/')
def index():
  return "PESCians !!!"

if __name__ == "__main__":
  app.run(debug=True)

step11: python3 webapp.py # starts webserver in localhost at port 5000

step12: Now lets add html file instead of a string, update the code
run.py file
from flask import Flask, render_template

app = Flask(__name__)

@app.route('/')
def home():
  return render_template('home.html')

if __name__ == "__main__":
  app.run(debug=True)

create a new notepad file save as home.html and change the savas type to "all file"

home.html file
<!DOCKTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Home Page</title>
</head>
<body>
  Hello PESCians!!!, how's the josh !!!!
</body>
</html>

Them lets have fun in html for a while.
