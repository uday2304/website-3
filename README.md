# Import libraries 
import requests 
import pandas as pd 
import matplotlib.pyplot as plt 

# Read the data 
car_data = pd.read_csv('cars_data.csv') 

# Analyze the data 
plt.scatter(car_data['Model'], car_data['Price'], color='r') 

# Set the labels 
plt.xlabel('Models') 
plt.ylabel('Prices') 

# Create a website
from flask import Flask, render_template 

app = Flask(__name__) 

@app
