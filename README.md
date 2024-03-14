
# Logistic Regression — Breast Cancer Prediction

1)Project link: Part-1

https://srinipratapgiri.medium.com/logistic-regression-breast-cancer-prediction-935ecd990b2a

2)Deployment of Containerized Machine Learning Model Application on AWS Elastic Container Service(ECS) link: Part-2

https://srinipratapgiri.medium.com/deployment-of-containerized-machine-learning-model-application-on-aws-elastic-container-cbd1464643b3

Dataset links: 

https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic)

https://www.kaggle.com/uciml/breast-cancer-wisconsin-data?select=data.csv

#First we Create instance with ubuntu AMI with t2.medium instance type with 30GB storage. 


sudo apt-get update && sudo apt-get upgrade -y 

*   sudo apt install python3-venv -y

*   python3 -m venv MLPRO

*   source MLPRO/bin/activate                 (activate the environment)

*   deactivate                                (to deactivate the envirnoment)

*   mkdir mlproject                           (create one project directory)

*   cd mlproject                              (changed to project directory also check the permission of folder)

Create new repo in github and follow below steps:

*   echo "# End-to-end-ML-Project" >> README.md

*   git add README.md

*   git commit -m "First Commit"

*   git status

*   git branch -M main

*   git branch

*   git remote add origin https://github.com/vipulwarthe/mlproject.git

*   git push -u origin main

Create .gitignore file with python template in mlproject repo on github

16  git pull    # It will pull the .gitignore file in VScode mlproject repo

create and add setup.py, requirements.txt, .ipynb notebook file, dataset file, app.py and Dockerfile in mlproject repo and after run all the files push into github repo.
save the model in modle.pkl format in github repo

*   pip install -r requirements.txt 

*   git status

*   git add .

*   git status

*   git commit -m "setup file added"

*   git push -u origin main

after creating app.py file run with below command also push all the files in github repo as well.

*   nohup python app.py & 

After run above command go to the browser and paste below link

http://localhost:5000/predict?s1=-0.96666522&s2=0.32786912&s3=-0.93579507&s4=-0.91104225&s5=0.60962671&s6=0.36569592&s7=-0.10914833&s8=-0.62181482&s9=-0.63860111&s10=0.53651178&s11=-0.46379509&s12=0.5132434&s13=-0.45632075&s14=-0.59189989&s15=0.67370318&s16=1.26928541&s17=2.17185315&s18=1.12535098&s19=0.64821758&s20=1.09244461&s21=-0.96440581&s22=-0.08750638&s23=-0.94145109&s24=-0.84547739&s25=-0.07511418&s26=-0.01862761&s27=-0.10400188&s28=-0.47718048&s29=-0.5634723&s30=0.05526303

Just replace the localhost with you public IP address and you will see the result
