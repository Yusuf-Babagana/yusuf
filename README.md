from flask import Flask, render_template,request,redirect,url_for
from flask_sqlalchemy import SQLAlchemy

app= Flask(__name__)
app.config['SQLALCHEMY_DATABASE_URI'] = 'sqlite:///sign.sqlite3'
app.config['SQALALCHEMY_TRACK_MODIFICATION'] =False

db = SQLAlchemy(app)
