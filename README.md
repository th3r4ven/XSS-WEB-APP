# XSS vulnerable WEB Application
<img src="https://img.shields.io/badge/python-3.8.6-blueviolet">

This web application simulates a vulnerable Blog that allow XSS scripting when posting comments and searching function.

in this simple application we have 2 common examples of XSS, stored and reflected

### XSS Stored

Basically this vulnerability store a JS script on its database or other data storage used by the application, and this script is delivered to every user that visit a page or post on this website.

### XSS reflected

This type of XSS is present commonly on URL, when doing some search on a website or submitting forms *(it does not limit just to those 2 cases)*, as this script is on URL, everyone that click on this infected URL will run its script and can be infected by other malicious user

---

## Running

Install required libs `pip install -r requirements.txt`

### Env vars
`FLASK_APP=app/__init__.py`

`FLASK_ENV=development`

`SAFE=False` to fix XSS scripting set this var to `SAFE=True`



