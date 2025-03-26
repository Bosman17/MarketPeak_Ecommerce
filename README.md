# CAPSTONE PROJECT- INTRODUCTION TO CLOUD COMPUTING

## MarketPeak_Ecommerce

__Step 1:__ Initializing Git Repository by using command; mkdir
![](./images/1.1.png)

__Step 2:__ Local Website Development
![](./images/1.2.png)
![](./images/1.22.png)
![](./images/1.24.png)

__Step 3:__ Staging and Committing of the template to Git with:
git add .
git config --global user.name "YourUsername"
git config --global user.email "youremail@example.com"
git commit -m "Initial commit with basic e-commerce site structure"
![](./images/1.3.png)
![](./images/1.32.png)

__Step 4:__ The code was pushed to the Github repository using: git remote add origin https://github.com/your-git-username/MarketPeak_Ecommerce.git and git push -u origin main
![](./images/1.4.png)

__Step 5:__ AWS Deployment: I created an EC2 Intance on my AWS as seen below.
![](./images/EC2.png)
![](./images/2.1.png)

__Step 6:__ I then cloned the repository on the linux server using SSH.
![](./images/2.2.png)
I got my SSH key using ssh-keygen to get my public key
![](./images/SSH%20Key.png)
Which was later added to my Github account.
![](./images/2.23.png)

__Step 7:__ I installed a web server on my Ec2 instance using sudo yum update -y
sudo yum install httpd -y
sudo systemctl start httpd
sudo systemctl enable httpd

![](./images/2.24.png)
![](./images/2.25.png)
![](./images/2.26.png)

__Step 8:__ I Confirgured httpd for website using sudo rm -rf /var/www/html/*
sudo cp -r ~/MarketPeak_Ecommerce/* /var/www/html/
![](./images/2.4.png)

Our Website
![](./images/Website.png)

__Step 9:__ Continous Integration and Deployment Workflow
![](./images/3.1.png)
Version Control with Git: New Features was added using git add .
git commit -m "Add new features or fix bugs"
git push origin development

![](./images/3.2.png)
![](./images/3.3.png)
__Step 10:__ Pull Request and Merging to the same branch using git checkout main
git merge development
git push origin main
git pull origin main

![](./images/3.4.png)

Then We have our changes reflected.
![](./images/3.5.png)

THANK YOU
