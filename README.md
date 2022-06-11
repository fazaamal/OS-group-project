**KULLIYYAH OF INFORMATION &amp; COMMUNICATION TECHNOLOGY**

**OPERATING SYSTEM**

**SEMESTER 2, 2021/2022**

**SECTION 1**

## **DOCKER AND DATABASE SETUP**

**PREPARED BY:**

| **NAME** | **MATRIC NO.** |
| --- | --- |
| MUHAMMAD YUSOFF BIN JAMALUDDIN | 2016799 |
| HAFSA BINTE MAHBUB | 2024364 |
| FAZA AMAL SOPHIAN | 2027009 |
| | |

**LECTURER**

Dr. Rizal

## TABLE OF CONTENT

[DOCKER DESKTOP INSTALLATION](#docker-desktop-installation) 

[WSL 2 INSTALLATION](#wsl-2-installation) 

[STARTING DOCKER AND CONTAINER](#starting-docker-and-container) 

[INSTALLING MONGODB DOCKER CONTAINER](#installing-mongodb-docker-container) 

[CREATING DATABASE IN MONGODB (CLI)](#creating-database-in-mongodb-%29cli%29) 

[CREATING DATABASE IN MONGODB (MONGODB COMPASS)](#creating-database-in-mongodb-(mongodb-compass))

## DOCKER DESKTOP INSTALLATION

![](RackMultipart20220611-1-pg5ly8_html_f5434f295b977383.png)

1) Go to docs [https://docs.docker.com/desktop/windows/install/](https://docs.docker.com/desktop/windows/install/) (for windows).

2) Click on &quot;Docker Desktop for Windows&quot;.

![](RackMultipart20220611-1-pg5ly8_html_79528e4751a14402.png)

3) Open Docker installer.

![](RackMultipart20220611-1-pg5ly8_html_376307c73cfeac99.png)

4) Choose your file destination for the installer. Docker desktop will start being installed.

![](RackMultipart20220611-1-pg5ly8_html_4f6b69e5dbbf74d2.png)

5) Configure your docker desktop and Click &quot;OK&quot; to start installation

![](RackMultipart20220611-1-pg5ly8_html_3357e9da5a372562.png)

5.1) Docker will start installation by unpacking files

Wait for Docker to finish unpacking files.

![](RackMultipart20220611-1-pg5ly8_html_5bb15f59beb6cc3f.png)

6) Once installation is complete, restart your computer.

![](RackMultipart20220611-1-pg5ly8_html_d30675c63655c5c0.png)

7) After restarting your computer, docker will start. Once it does so, accept the Service Agreement

## WSL 2 INSTALLATION

![](RackMultipart20220611-1-pg5ly8_html_efc029388816abc2.png)

8) In order to proceed with Docker, your computer must have a Linux kernel.

Docker will show a pop up that provides a link for WSL 2 installation, and click on the link ([https://aka.ms/wsl2kernel](https://aka.ms/wsl2kernel))

![](RackMultipart20220611-1-pg5ly8_html_1e5e15189f309cde.png)

![](RackMultipart20220611-1-pg5ly8_html_829e18a5c64eaa5f.png)

9) Once the website opens, scroll down to step 4, and click on the link under &quot;Download the latest package&quot;.

![](RackMultipart20220611-1-pg5ly8_html_5030230ec7a87dfd.png)

10) Choose the file destination for the installer package and click save.

![](RackMultipart20220611-1-pg5ly8_html_926c087bb05de725.png)

11) Wait for the installation, once the installation is complete, click on the .exe file.

![](RackMultipart20220611-1-pg5ly8_html_1af3084fa6c1ab99.png)

12) Click &quot;Next&quot; on the Linux Setup Wizard.

![](RackMultipart20220611-1-pg5ly8_html_9584b20bd2af7f58.png)

12.1) Wait for the setup wizard to finish the installation.

![](RackMultipart20220611-1-pg5ly8_html_f5217b0cee9baab8.png)

13) Once installation is completed, click on the &quot;Finish&quot; button.

## STARTING DOCKER AND CONTAINER

![](RackMultipart20220611-1-pg5ly8_html_b69ca59fce682c40.png)

After you Restart your computer, Docker Desktop will open.

![](RackMultipart20220611-1-pg5ly8_html_8e24c3d0281dcdf.png)

14) Click on &quot;Start&quot; to get started with Docker.

![](RackMultipart20220611-1-pg5ly8_html_57fc403c35923574.png)

15 -20) Complete the tutorial.

![](RackMultipart20220611-1-pg5ly8_html_3b6f41c01834276c.png)

![](RackMultipart20220611-1-pg5ly8_html_60b8278f73b4cac2.png)

20.1) When you press &quot;Next Step&quot; you have instruction to Push your image to your Docker Hub (not shown for the 4th step)

![](RackMultipart20220611-1-pg5ly8_html_fc947fc73f7f0dcd.png)

21) When you completed Docker Tutorial (or skipped it), &quot;Home&quot; section will be your main menu with container options to download.

For us we selected MongoDB as our database and connected it to [MongoDB Compass](#_4t61j2rohx8u) as our UI to view the content interactively.

## INSTALLING MONGODB DOCKER CONTAINER

![](RackMultipart20220611-1-pg5ly8_html_e7d2766896d09568.png)

1) Open your Windows PowerShell and type &quot;docker --version&quot; to ensure MongoDB is compatible.

![](RackMultipart20220611-1-pg5ly8_html_fe38da761dc68088.png)

2) Type &quot;docker pull mongo&quot;. This will pull Mongo Image to your Docker storage

![](RackMultipart20220611-1-pg5ly8_html_2c65e3903eec306f.png)

3) Type &quot;docker images&quot;. This will show you the images with it&#39;s version and related details.

![](RackMultipart20220611-1-pg5ly8_html_42aa0845b435d653.png)

4) Type &quot;docker run --name mongo\_example -d mongo&quot;.

This will create a Docker Container with below meaning:

- docker run: this command Docker to run a container
- (double dash)name : this will give name to the container
- mongo\_example: name of the container
- -d: detach, this means if we close the powershell/terminal the container will run on background
- mongo: the image name we want to use

![](RackMultipart20220611-1-pg5ly8_html_6694647d123a21f.png)

5) Type &quot;docker ps&quot;.

This command checks the running container in Docker.

![](RackMultipart20220611-1-pg5ly8_html_7ac817e33792f775.png)

6) We can also see the container is running in Docker with the name we gave and the details

## CREATING DATABASE IN MONGODB (CLI)

![](RackMultipart20220611-1-pg5ly8_html_f13616d46ed38315.png)

1) Click on mongo CLI on Docker.

Make sure the container is running and this option is available

![](RackMultipart20220611-1-pg5ly8_html_ed839744ea9226c5.png)

2) Type the command &quot;mongosh&quot;.

This will access mongodb using the mongo shell.

![](RackMultipart20220611-1-pg5ly8_html_47a3e538f7b3ce83.png)

3) Type command &quot;use \&lt;dbName\&gt;&quot;, which in our scenario is &quot;food&quot;.

This will create a database name &quot;food&quot; and use it as our running database.

![](RackMultipart20220611-1-pg5ly8_html_999a049f5d7d122d.png)

4) type command &quot;db.createCollection(&quot;\&lt;collectionName\&gt;&quot;), which in our scenario is &quot;fruits&quot;. This will create a collection named &quot;fruits&quot;.

MongoDB is a NoSQL, thus no table is created but a combination of Key-Value pair as it&#39;s database storage.

![](RackMultipart20220611-1-pg5ly8_html_2b2cf0031b0e3cbd.png)

6) Type command &quot;db.\&lt;collectionName\&gt;.insert &quot;\&lt;id\&gt;:\&lt;data\&gt;&quot;, which in our scenario is &quot;db.fruits.insert &quot;name: Apple&quot;. (Make sure to use correct syntax)

You can insert many fruits at once by the command &quot;db.fruits.insertMany([{name: &quot;Apple&quot;, origin: &quot;USA&quot;, price: 5}, {name: &quot;orange&quot;, origin: &quot;Italy&quot;, price: 3}, {name: &quot;Mango&quot;, origin: &quot;Malaysia&quot;, price: 3}])&quot;.
 By executing this command you will be inserting 3 fruits (Apple, Orange, and Mango), each one has its own origin and price.

We can later view the collection using find() function.

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
