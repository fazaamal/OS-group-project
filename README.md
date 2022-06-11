# **DOCKER AND DATABASE SETUP**

**PREPARED BY:**

| **NAME** | **MATRIC NO.** |
| --- | --- |
| MUHAMMAD YUSOFF BIN JAMALUDDIN | 2016799 |
| HAFSA BINTE MAHBUB | 2024364 |
| FAZA AMAL SOPHIAN | 2027009 |
| | |

**LECTURER**

Dr. Rizal, Section 1

## TABLE OF CONTENT

[DOCKER DESKTOP INSTALLATION](#docker-desktop-installation) 

[WSL 2 INSTALLATION](#wsl-2-installation) 

[STARTING DOCKER AND CONTAINER](#starting-docker-and-container) 

[INSTALLING MONGODB DOCKER CONTAINER](#installing-mongodb-docker-container) 

[CREATING DATABASE IN MONGODB (CLI)](#creating-database-in-mongodb-cli) 

[CREATING DATABASE IN MONGODB (MONGODB COMPASS)](#creating-database-in-mongodb-mongodb-compass)

## DOCKER DESKTOP INSTALLATION

![https://ibb.co/mqDy9NC](https://i.ibb.co/xjCg1FS/Step-1-Step-2-website-and-download.png)

1) Go to docs [https://docs.docker.com/desktop/windows/install/](https://docs.docker.com/desktop/windows/install/) (for windows).

2) Click on &quot;Docker Desktop for Windows&quot;.

![](https://i.ibb.co/30PHD9t/Step-3-installer.png)

3) Open Docker installer.

![](https://i.ibb.co/tzLNVfc/Step-4-save.png)

4) Choose your file destination for the installer. Docker desktop will start being installed.

![](https://i.ibb.co/4jfjmbk/Step-5-configure-and-start-installation.png)

5) Configure your docker desktop and Click &quot;OK&quot; to start installation

![](https://i.ibb.co/rZ9z9Z1/Step-5i-unpakcing-files.png)

5.1) Docker will start installation by unpacking files

Wait for Docker to finish unpacking files.

![](https://i.ibb.co/KKcXJqy/Step-6-restart.png)

6) Once installation is complete, restart your computer.

![](https://i.ibb.co/qnS9p42/Step-7-service-agreement.png)

7) After restarting your computer, docker will start. Once it does so, accept the Service Agreement

## WSL 2 INSTALLATION

![](https://i.ibb.co/TKWNF9x/Step-8-WSL-popup.png)

8) In order to proceed with Docker, your computer must have a Linux kernel.

Docker will show a pop up that provides a link for WSL 2 installation, and click on the link ([https://aka.ms/wsl2kernel](https://aka.ms/wsl2kernel))

![](https://i.ibb.co/YdxSNPr/Step-9-WSL-website.png)

![](https://i.ibb.co/ccddcnB/Step-9i-WSL-scroll-down.png)

9) Once the website opens, scroll down to step 4, and click on the link under &quot;Download the latest package&quot;.

![](https://i.ibb.co/7nL7YgW/Step-10-WSL-save.png)

10) Choose the file destination for the installer package and click save.

![](https://i.ibb.co/mB7ZVgr/Step-11-WSL-installer.png)

11) Wait for the installation, once the installation is complete, click on the .exe file.

![](https://i.ibb.co/w6XjZx5/Step-12-WSL-next.png)

12) Click &quot;Next&quot; on the Linux Setup Wizard.

![](https://i.ibb.co/qCh7cvR/Step-12-i-WSL-wait-for-installation.png)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;i) Wait for the setup wizard to finish the installation.

![](https://i.ibb.co/CsvtdF4/Step-13-WSL-finish.png)

13) Once installation is completed, click on the &quot;Finish&quot; button.

## STARTING DOCKER AND CONTAINER

![](https://i.ibb.co/mH0zk0D/Step-14-docker-startup.png)

After you Restart your computer, Docker Desktop will open.

![](https://i.ibb.co/6013K16/Step-14-i-getting-started.png)

14) Click on &quot;Start&quot; to get started with Docker.

![](https://i.ibb.co/2jQHbNF/Step-15-and-step-16-getting-started.png)

![](https://i.ibb.co/RQCzbFF/Step-17-and-step-18-getting-started.png)

15 -20) Complete the tutorial.

![](https://i.ibb.co/b5HVZMB/Step-19-and-Step-20-and-step-20-i.png)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;i) When you press &quot;Next Step&quot; you have instruction to Push your image to your Docker Hub (not shown for the 4th step)

![](https://i.ibb.co/10Lqmm4/Step-21-final.png)

21) When you completed Docker Tutorial (or skipped it), &quot;Home&quot; section will be your main menu with container options to download.

For us we selected MongoDB as our database and connected it to MongoDB Compass as our UI to view the content interactively.

## INSTALLING MONGODB DOCKER CONTAINER

![](https://i.ibb.co/TvsSb5T/Step-1.png)

1) Open your Windows PowerShell and type &quot;docker --version&quot; to ensure MongoDB is compatible.

![](https://i.ibb.co/C6t2h6Y/Step-2.png)

2) Type &quot;docker pull mongo&quot;. This will pull Mongo Image to your Docker storage

![](https://i.ibb.co/C8LC5GH/Step-3.png)

3) Type &quot;docker images&quot;. This will show you the images with it&#39;s version and related details.

![](https://i.ibb.co/M7hfFzw/Step-4.png)

4) Type &quot;docker run --name mongo\_example -d mongo&quot;.

This will create a Docker Container with below meaning:

- docker run: this command Docker to run a container
- (double dash)name : this will give name to the container
- mongo\_example: name of the container
- -d: detach, this means if we close the powershell/terminal the container will run on background
- mongo: the image name we want to use

![](https://i.ibb.co/RgtjMVT/Step-5.png)

5) Type &quot;docker ps&quot;.

This command checks the running container in Docker.

![](https://i.ibb.co/yBPLbNB/step-6-container.png)

6) We can also see the container is running in Docker with the name we gave and the details

## CREATING DATABASE IN MONGODB (CLI)

![](https://i.ibb.co/vLwJLFG/1.png)

1) Click on mongo CLI on Docker.

Make sure the container is running and this option is available

![](https://i.ibb.co/m0xcMWg/2.png)

2) Type the command &quot;mongosh&quot;.

This will access mongodb using the mongo shell.

![](https://i.ibb.co/JBWCRVq/3.png)

3) Type command &quot;use dbName&quot;, which in our scenario is &quot;food&quot;.

This will create a database name &quot;food&quot; and use it as our running database.

![](https://i.ibb.co/X3r4NBB/4.png)

4) Type command &quot;db.createCollection(&quot;collectionName&quot;), which in our scenario is &quot;fruits&quot;. This will create a collection named &quot;fruits&quot;.

MongoDB is a NoSQL, thus no table is created but a combination of Key-Value pair as it&#39;s database storage.

![](https://i.ibb.co/FXKbYBR/5.png)

5) Type command &quot;db.collectionName.insert(JSON object)&quot;, which in our scenario is &quot;db.fruits.insert({name: Apple})&quot;. (Make sure to use correct syntax)

You can insert many fruits at once by the command &quot;db.fruits.insertMany([{name: &quot;Apple&quot;, origin: &quot;USA&quot;, price: 5}, {name: &quot;orange&quot;, origin: &quot;Italy&quot;, price: 3}, {name: &quot;Mango&quot;, origin: &quot;Malaysia&quot;, price: 3}])&quot;.
 By executing this command you will be inserting 3 fruits (Apple, Orange, and Mango), each one has its own origin and price.

![](https://i.ibb.co/QfcjmkS/6.png)

6) We can later view the collection using find() function.

\*\*We are using the built-in JS functions provided by MongoDB itself, we can also use regular SQL Command but not shown here.

\*\*MongoDB mostly uses built-in JS functions, that&#39;s why it&#39;s widely used by JS Developers.

## MONGODB COMPASS INSTALLATION

![](RackMultipart20220611-1-pg5ly8_html_802d2a5175ffc54b.jpg)

1) Download MongoDB Compass from the link ([https://www.mongodb.com/try/download/compass](https://www.mongodb.com/try/download/compass))

2) Click on the dropdown to choose the package according to your operating system, for Windows MSI or EXE is recommended.

3) Click on Download.

4) Open the installer and click Next for the installation to start.

![](RackMultipart20220611-1-pg5ly8_html_b6ae2713c9d223f.jpg)

5) Click Next to begin the installation.

![](RackMultipart20220611-1-pg5ly8_html_9cd3c3d09ffd6837.jpg)

6) You can change the installation directory, but we leave it as the default here.

7) Click Next to confirm your directory installation.

![](RackMultipart20220611-1-pg5ly8_html_f3763bbc39069316.jpg)

8) Wait for the installation process to finish.

![](RackMultipart20220611-1-pg5ly8_html_d3b0bea32c9759f3.jpg)

9) Click Finish to close the installation window.

![](RackMultipart20220611-1-pg5ly8_html_d3d75d649df5c87d.jpg)

10) Open your MongoDB Compass, here is shown the main menu of the application. We skipped the Introduction part.

11) This is the configuration you will use to connect MongoDB Compass to the MongoDB you set up inside Docker (MongoDB Container).

## CREATING DATABASE IN MONGODB (MONGODB COMPASS)
