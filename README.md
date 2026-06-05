# Host-Nginx-server-and-connect-it-with-Git-
**Hosting an app in an Nginx web server and connecting it to a Git version control system**

**1. Create a VM in the AWS platform**
   
**2. Update and upgrade the Instance**
   
        sudo apt update -y
   
        sudo apt upgrade -y

**3. Install the Nginx server on the virtual machine instance**

        apt install nginx -y

        systemctl start nginx

        systemctl enable nginx

        systemctl status nginx

**4. Test Nginx**

        http://3.15.171.16

**Public IP address of your instance. (Welcome to nginx page will appear)**

**5. Create your HTML application**

        cd /var/www/html

        ls

        index.nginx-debian.html

        rm index.nginx-debian.html

**6. Create an HTML file**

        vim index.html

**Some shortcuts that will be useful in the Vim text editor**

Esc + u              -> undo 
Esc + gg             -> move to 1st line in the code
Esc + gg + d + G     -> move to 1st line in the code, delete everything in the code
Esc + dd             -> removes the line where the cursor is placed 

i      -> Insert mode
Esc    -> Normal mode
dd     -> Cut line
yy     -> Copy line
p      -> Paste
u      -> Undo
Ctrl+r -> Redo
:wq    -> Save and quit
:q!    -> Quit without saving
o      -> insert new line 
gg     -> Go to the beginning of the file
G      -> Go to the end of the file
50G    -> Go to line 50
h      -> Move left
j      -> Move down 
k      -> Move up 
l      -> Move right 

**Code is there in to do app code.txt file. Paste it into the index.html file**

**7. Test your app**

**8. Install Git**

         apt install git -y

         git --version

         mkdir devops-webapp

         cd devops-webapp

         git init

         cp /var/www/html/index.html .

         ls

         git add .

         git config --global user.name "Dharshika Poopalan"

         git config --global user.email "dharshikasms@gmail.com"

         git commit -m "First DevOps Web App"

         git remote add origin URL/devops-webapp

         git remote -v

         git branch

         git branch -M main

         git push -u origin main

         git clone URL+Repo which need to be cloned

**Difference between Clone and Push** 



     

     
