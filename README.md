# Ex.06 Book Front Cover Page Design
# Date:
30/11/2024
# AIM:
To design a book front cover page using HTML and CSS.

# DESIGN STEPS:
## Step 1:
Create a Django Admin project.

## Step 2:
Create an app in the Django interface.

## Step 3:
Create a folder named 'static' in the app folder.

## Step 4:
Create a new HTML file in the static folder.

## Step 5:
Write the HTML code with relevant CSS properties.

## Step 6:
Choose the appropriate style and color scheme.

## Step 7:
Insert the images in their appropriate places.

## Step 8:
Publish the website in the LocalHost.

# PROGRAM:
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Book Cover</title>
    <style>
        body {
            margin: 0;
            font-family: 'Georgia', serif;
            background-color: #eae7dc;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }
        .book-cover {
            width: 400px;
            height: 600px;
            background: linear-gradient(145deg, #ffeadb, #f7d9c4);
            border-radius: 20px;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.25);
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            align-items: center;
            padding: 20px;
            position: relative;
            text-align: center;
            border: 4px solid #d9b08c;
        }
        .book-cover img {
            width: 80%;
            height: auto;
            border-radius: 15px;
            border: 3px solid #d9b08c;
            box-shadow: 0 8px 15px rgba(0, 0, 0, 0.2);
            margin-top: 10px;
        }
        .title {
            font-size: 2.2em;
            font-family: 'Times New Roman', serif;
            font-weight: bold;
            color: #4a3f35;
            margin: 20px 0 10px 0;
            text-shadow: 2px 2px #f4a261;
        }
        .subtitle {
            font-size: 1.4em;
            font-family: 'Palatino Linotype', serif;
            color: #3f2a21;
            margin-bottom: 20px;
            text-shadow: 1px 1px #e76f51;
        }
        .author {
            font-size: 1.2em;
            font-weight: bold;
            color: #1d3557;
            margin-bottom: 30px;
            font-family: 'Courier New', monospace;
        }
        .decorative-line {
            width: 50%;
            height: 3px;
            background-color: #8d99ae;
            margin: 10px auto;
            border-radius: 5px;
        }
        .footer {
            font-size: 0.9em;
            color: #7f5539;
            font-family: 'Verdana', sans-serif;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <div class="book-cover">
        <!-- Replace src with a valid image URL -->
        <img src="https://blackhattalent.com/wp-content/uploads/2023/08/robinslalalalharma.jpg" alt="Robin Sharma">
        <div class="title">The Leader Within</div>
        <div class="decorative-line"></div>
        <div class="subtitle">Unlock Your True Potential</div>
        <div class="author">By Robin Sharma</div>
        <div class="footer">© 2024, Leadership Publishing</div>
    </div>
</body>
</html>
~~~
views.py
~~~
from django.shortcuts import render
def htm(request):
    return render(request,"Time_Table.html")

def html(request):
    return render(request,"book.html")
   
# Create your views here.
~~~
urls.py
~~~
"""
URL configuration for sam project.

The `urlpatterns` list routes URLs to views. For more information please see:
    https://docs.djangoproject.com/en/5.1/topics/http/urls/
Examples:
Function views
    1. Add an import:  from my_app import views
    2. Add a URL to urlpatterns:  path('', views.home, name='home')
Class-based views
    1. Add an import:  from other_app.views import Home
    2. Add a URL to urlpatterns:  path('', Home.as_view(), name='home')
Including another URLconf
    1. Import the include() function: from django.urls import include, path
    2. Add a URL to urlpatterns:  path('blog/', include('blog.urls'))
"""
from django.contrib import admin
from django.urls import path
from myapp import views

urlpatterns = [
    path('admin/', admin.site.urls),
    path('new1/',views.htm),
    path('book/',views.html)

]
~~~
# OUTPUT:

![Screenshot 2024-12-07 132112](https://github.com/user-attachments/assets/2fab3822-cd5d-43bf-90ce-c96231ee6982)


# RESULT:
The program for designing book front cover page using HTML and CSS is completed successfully.
