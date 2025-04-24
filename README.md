# Market Peak Ecommerce Deployment with Git, Linux and AWS

### Initialize Git Repository

![](img/1.%20make%20MPE.PNG)

- create user and email on git

![](img/2.%20user_name_email.PNG)

```bash
git remote add origin https://github.com/eyibiogeorge/MarketPeak_Ecommerce.git
```

- create a Market Peak Ecommerce repo on github

![](img/3.%20github.PNG)

- launch an EC2 instance on AWS

![](img/4.%20ec2.PNG)

- ssh into the EC2 

![](img/5.%20ssh%20to%20ec2.PNG)

- generate public key

![](img/6.%20ssh-keygen.PNG)

- Link Github with EC2 using public key

![](img/7.%20public-ssh.PNG)

- ssh public key successfully link

![](img/8.%20add%20ssh%20to%20github.PNG)

- clone remote repo on EC2 using ssh.
you will have to `sudo yum install git` before you can clone git.

![](img/9.%20clone-ssh.PNG)

- clone to EC2

![](img/10.%20clone-repo.PNG)

```bash
sudo yum update -y
sudo yum install httpd -y
sudo systemctl start httpd
sudo systemctl enable httpd
```

- remove, copy and reload file in `/var/www/html`

![](img/12.%20rm-cp%20and%20reload.PNG)

- Display the deployed website

![](img/11.%20marketPeak-homepage.PNG)

- create and switch into a new branch

![](img/13.%20branch%20development.PNG)

- create pull request

![](img/14.%20pull%20request.PNG)

- successfully merge pull request to the main branch

![](img/15.%20merge%20request.PNG)

```bash
git commit -m "Add new features or fix bugs"
```

![](img/16.%20branch%20update.PNG)

