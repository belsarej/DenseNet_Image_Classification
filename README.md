# DenseNet_Image_Classification
Implementation of DenseNet image classification

### Orignal training file for densenet Final_DenseNet_Implementation.ipynb

### Step 1 Clone the file from git using command 

git clone https://github.com/belsarej/DenseNet_Image_Classification.git

### Step 2 Open CMD on computer and go to root directory using command cd DenseNet_Image_Classification

![](https://github.com/belsarej/DenseNet_Image_Classification/blob/main/data/de%201%20screenshot.PNG)

Additional step (If your env not ready then run requirements.txt after entering in folder command (pip install -r requirements.txt )

# Step 3 Run command Python app.py

![](https://github.com/belsarej/DenseNet_Image_Classification/blob/main/data/ds%202.PNG)

# Step4 Click on link http://127.0.0.1:5000


![](https://github.com/belsarej/DenseNet_Image_Classification/blob/main/data/ds2.PNG)


# Step6  Click on choose file and choose image for classififcation


![](https://github.com/belsarej/DenseNet_Image_Classification/blob/main/data/ds3.PNG)



# Step7  Click on upload and see result 


![](https://github.com/belsarej/DenseNet_Image_Classification/blob/main/data/Capture.PNG)

##Deployment

We chose Heroku for deployement. Preparing the Repo for Heroku Deployment.

Heroku looks for 2 things

Procfile - Intital file to run during deployment

#Creates Procfile without any extensions

touch Procfile

#Open in notepad and write the following

web: gunicorn app:app

requirements.txt - To install dependencies


flask==1.1.1

gunicorn==20.0.4

torch==1.4.0+cpu 

torchvision==0.5.0+cpu 

-f https://download.pytorch.org/whl/torch_stable.html

Pillow==7.0.0

numpy==1.15.4

pandas==1.0.1

matplotlib==3.1.3

scikit-learn==0.22.2.post1

Jinja2==2.11.1

tqdm==4.42.1

Following are the steps followed to deploy the model on to heroku

Sign up for a free account at Heroku

Create a New app

Name the app (Will be part of the deployed URL)

Click Create app

Connect to Github

Choose the Repo that we need to deploy

Choose the Branch from which to deploy

Click on Deploy Branch

Turn on Automatic Deployment if needed

Heroku in the background runs all the dependencies and installs them. For free version of heroku hosting the bundle size is limited to 500MB.

Once everything goes well our model will be deployed and we can view our link beloy it
