<h1 align="center">DOCKER AND DATABASE SETUP</h1>


### [Link to Google Docs (backup)](https://docs.google.com/document/d/1wzcsIiCowplbkTmHnPt6YmQ3Dpv_2DsILEakmBFyuW8/edit?usp=sharing)

**PREPARED BY:**

| **NAME** | **MATRIC NO.** |
| --- | --- |
| MUHAMMAD YUSOFF BIN JAMALUDDIN | 2016799 |
| HAFSA BINTE MAHBUB | 2024364 |
| FAZA AMAL SOPHIAN | 2027009 |
| FADWA RAMADAN ALI HASSAN| 2024334 |

**LECTURER**

Dr. Rizal, Section 1

<h2 align="center">TABLE OF CONTENT</h2>

[DOCKER DESKTOP INSTALLATION](#docker-desktop-installation) 

[WSL 2 INSTALLATION](#wsl-2-installation) 

[STARTING DOCKER AND CONTAINER](#starting-docker-and-container) 

[INSTALLING MONGODB DOCKER CONTAINER](#installing-mongodb-docker-container) 

[CREATING DATABASE IN MONGODB (CLI)](#creating-database-in-mongodb-cli) 

[CREATING DATABASE IN MONGODB (MONGODB COMPASS)](#creating-database-in-mongodb-mongodb-compass)

<h2 align="center">DOCKER DESKTOP INSTALLATION</h2>

<p align="center">
   <img src="https://i.ibb.co/xjCg1FS/Step-1-Step-2-website-and-download.png" alt="Material Bread logo"> 
</p>

1) Go to docs [https://docs.docker.com/desktop/windows/install/](https://docs.docker.com/desktop/windows/install/) (for windows).

2) Click on &quot;Docker Desktop for Windows&quot;.

<p align="center">
   <img src="https://i.ibb.co/30PHD9t/Step-3-installer.png" alt="Material Bread logo"> 
</p>


3) Open Docker installer.

<p align="center">
   <img width = "600" src="https://i.ibb.co/tzLNVfc/Step-4-save.png" alt="Material Bread logo"> 
</p>

4) Choose your file destination for the installer. Docker desktop will start being installed.

<p align="center">
   <img width = "600" src="https://i.ibb.co/4jfjmbk/Step-5-configure-and-start-installation.png" alt="Material Bread logo"> 
</p>

5) Configure your docker desktop and Click &quot;OK&quot; to start installation

<p align="center">
   <img width = "600" src="https://i.ibb.co/rZ9z9Z1/Step-5i-unpakcing-files.png" alt="Material Bread logo"> 
</p>

5.1) Docker will start installation by unpacking files

<p align="center">
   <img width = "600" src="https://i.ibb.co/KKcXJqy/Step-6-restart.png" alt="Material Bread logo"> 
</p>


6) Once installation is complete, restart your computer.

<p align="center">
   <img width = "600" src="https://i.ibb.co/qnS9p42/Step-7-service-agreement.png" alt="Material Bread logo"> 
</p>

7) After restarting your computer, docker will start. Once it does so, accept the Service Agreement

<h2 align="center">WSL 2 INSTALLATION</h2>

<p align="center">
    In order to proceed with Docker, your computer must have a Linux kernel.
</p>

<p align="center">
   <img width = "600" src="https://i.ibb.co/TKWNF9x/Step-8-WSL-popup.png" alt="Material Bread logo"> 
</p>


8) Docker will show a pop up that provides a link for WSL 2 installation, and click on the link ([https://aka.ms/wsl2kernel](https://aka.ms/wsl2kernel))

<p align="center">
   <img  width = "600" src="https://i.ibb.co/ccddcnB/Step-9i-WSL-scroll-down.png" alt="Material Bread logo"> 
</p>

9) Once the website opens, scroll down to step 4, and click on the link under &quot;Download the latest package&quot;.

<p align="center">
   <img  width = "600" src="https://i.ibb.co/7nL7YgW/Step-10-WSL-save.png"> 
</p>

10) Choose the file destination for the installer package and click save.

<p align="center">
   <img width = "600"  src="https://i.ibb.co/mB7ZVgr/Step-11-WSL-installer.png"> 
</p>

11) Wait for the installation, once the installation is complete, click on the .exe file.

<p align="center">
   <img  width = "600" src="https://i.ibb.co/w6XjZx5/Step-12-WSL-next.png" alt="Material Bread logo"> 
</p>

12) Click &quot;Next&quot; on the Linux Setup Wizard.



<p align="center">
   <img width = "600"  src="https://i.ibb.co/CsvtdF4/Step-13-WSL-finish.png" alt="Material Bread logo"> 
</p>

13) Once installation is completed, click on the &quot;Finish&quot; button.

<h2 align="center">STARTING DOCKER AND CONTAINER</h2>

<p align="center">
   <img width = "600" src="https://i.ibb.co/mH0zk0D/Step-14-docker-startup.png" alt="Material Bread logo"> 
</p>

After you Restart your computer, Docker Desktop will open.

<p align="center">
   <img width = "600"  src="https://i.ibb.co/6013K16/Step-14-i-getting-started.png" alt="Material Bread logo"> 
</p>

14) Click on &quot;Start&quot; to get started with Docker.

<p align="center">
   <img width = "600" src="https://i.ibb.co/2jQHbNF/Step-15-and-step-16-getting-started.png" alt="Material Bread logo"> 
</p>

<p align="center">
   <img width = "600" src="https://i.ibb.co/RQCzbFF/Step-17-and-step-18-getting-started.png" alt="Material Bread logo"> 
</p>


<p align="center">
   <img width = "600" src="https://i.ibb.co/b5HVZMB/Step-19-and-Step-20-and-step-20-i.png" alt="Material Bread logo"> 
</p>

15 -20) Complete the tutorial.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;i) When you press &quot;Next Step&quot; you have instruction to Push your image to your Docker Hub (not shown for the 4th step)

<p align="center">
   <img width = "600" src="https://i.ibb.co/10Lqmm4/Step-21-final.png" alt="Material Bread logo"> 
</p>

21) When you completed Docker Tutorial (or skipped it), &quot;Home&quot; section will be your main menu with container options to download.

For us we selected MongoDB as our database and connected it to MongoDB Compass as our UI to view the content interactively.

<h2 align="center">INSTALLING MONGODB DOCKER CONTAINER</h2>

<p align="center">
   <img src="https://i.ibb.co/TvsSb5T/Step-1.png" alt="Material Bread logo"> 
</p>

1) Open your Windows PowerShell and type &quot;docker --version&quot; to ensure MongoDB is compatible.

<p align="center">
   <img src="https://i.ibb.co/C6t2h6Y/Step-2.png" alt="Material Bread logo"> 
</p>

2) Type &quot;docker pull mongo&quot;. This will pull Mongo Image to your Docker storage

<p align="center">
   <img src="https://i.ibb.co/C8LC5GH/Step-3.png" alt="Material Bread logo"> 
</p>

3) Type &quot;docker images&quot;. This will show you the images with it&#39;s version and related details.

<p align="center">
   <img src="https://i.ibb.co/M7hfFzw/Step-4.png" alt="Material Bread logo"> 
</p>

4) Type &quot;docker run --name mongo\_example -d mongo&quot;.

This will create a Docker Container with below meaning:

- docker run: this command Docker to run a container
- (double dash)name : this will give name to the container
- mongo\_example: name of the container
- -d: detach, this means if we close the powershell/terminal the container will run on background
- mongo: the image name we want to use

<p align="center">
   <img src="https://i.ibb.co/RgtjMVT/Step-5.png" alt="Material Bread logo"> 
</p>

5) Type &quot;docker ps&quot;.

This command checks the running container in Docker.

<p align="center">
   <img src="https://i.ibb.co/yBPLbNB/step-6-container.png" alt="Material Bread logo"> 
</p>

6) We can also see the container is running in Docker with the name we gave and the details

<h2 align="center">CREATING DATABASE IN MONGODB (CLI)</h2>

<p align="center">
   <img src="https://i.ibb.co/vLwJLFG/1.png" alt="Material Bread logo"> 
</p>

1) Click on mongo CLI on Docker.

Make sure the container is running and this option is available

<p align="center">
   <img src="https://i.ibb.co/m0xcMWg/2.png" alt="Material Bread logo"> 
</p>

2) Type the command &quot;mongosh&quot;.

This will access mongodb using the mongo shell.

<p align="center">
   <img src="https://i.ibb.co/JBWCRVq/3.png" alt="Material Bread logo"> 
</p>

3) Type command &quot;use dbName&quot;, which in our scenario is &quot;food&quot;.

This will create a database name &quot;food&quot; and use it as our running database.

<p align="center">
   <img src="https://i.ibb.co/X3r4NBB/4.png" alt="Material Bread logo"> 
</p>

4) Type command &quot;db.createCollection(&quot;collectionName&quot;), which in our scenario is &quot;fruits&quot;. This will create a collection named &quot;fruits&quot;.

MongoDB is a NoSQL, thus no table is created but a combination of Key-Value pair as it&#39;s database storage.

<p align="center">
   <img src="https://i.ibb.co/FXKbYBR/5.png" alt="Material Bread logo"> 
</p>

5) Type command &quot;db.collectionName.insert(JSON object)&quot;, which in our scenario is &quot;db.fruits.insert({name: Apple})&quot;. (Make sure to use correct syntax)

You can insert many fruits at once by the command &quot;db.fruits.insertMany([{name: &quot;Apple&quot;, origin: &quot;USA&quot;, price: 5}, {name: &quot;orange&quot;, origin: &quot;Italy&quot;, price: 3}, {name: &quot;Mango&quot;, origin: &quot;Malaysia&quot;, price: 3}])&quot;.
 By executing this command you will be inserting 3 fruits (Apple, Orange, and Mango), each one has its own origin and price.

<p align="center">
   <img src="https://i.ibb.co/QfcjmkS/6.png" alt="Material Bread logo"> 
</p>

6) We can later view the collection using find() function.

\*\*We are using the built-in JS functions provided by MongoDB itself, we can also use regular SQL Command but not shown here.

\*\*MongoDB mostly uses built-in JS functions, that&#39;s why it&#39;s widely used by JS Developers.

<h2 align="center"> MONGODB COMPASS INSTALLATION</h2>

<p align="center">
   <img width = "700" src="https://i.ibb.co/Fq93FG0/1-Download-and-Start-Install.jpg" alt="Material Bread logo"> 
</p> width = "700"

1) Download MongoDB Compass from the link ([https://www.mongodb.com/try/download/compass](https://www.mongodb.com/try/download/compass))

2) Click on the dropdown to choose the package according to your operating system, for Windows MSI or EXE is recommended.

3) Click on Download.

4) Open the installer and click Next for the installation to start.

<p align="center">
   <img width = "700" src="https://i.ibb.co/XzYfYZL/2-Click-next-for-the-installation.jpg" alt="Material Bread logo"> 
</p>

5) Click Next to begin the installation.

<p align="center">
   <img width = "700" src="https://i.ibb.co/cJ8h38K/3-You-can-set-the-location-but-we-leave-it-default.jpg"> 
</p>

6) You can change the installation directory, but we leave it as the default here.

7) Click Next to confirm your directory installation.

<p align="center">
   <img width = "700" src="https://i.ibb.co/CQNvLNm/4-Installation-Progress.jpg" alt="Material Bread logo"> 
</p>

8) Wait for the installation process to finish.

<p align="center">
   <img width = "700" src="https://i.ibb.co/zGzckHL/5-Installation-Finished.jpg" alt="Material Bread logo"> 
</p>

9) Click Finish to close the installation window.

<p align="center">
   <img width = "700" src="https://i.ibb.co/VwQc9Zm/6-When-you-open-Mongo-DB-Compass-this-will-be-your-main-screen.jpg" alt="Material Bread logo"> 
</p>

10) Open your MongoDB Compass, here is shown the main menu of the application. We skipped the Introduction part.

11) This is the configuration you will use to connect MongoDB Compass to the MongoDB you set up inside Docker (MongoDB Container).


<h2 align="center">CREATING DATABASE IN MONGODB (MONGODB COMPASS)</h2>

<p align="center">
   <img src="https://i.ibb.co/2SVYK8V/1-Step-1-i-set-the-port-number-to-27017.png" alt="Material Bread logo"> 
</p>

1(i) Create a container with 271017 port number

<p align="center">
   <img width = "700" src="https://i.ibb.co/TgSjyHm/Step-1-ii-Click-on-Advanced-connection-options.png" alt="Material Bread logo"> 
</p>

1)(ii) Go to Mongo Compass Desktop and click on Advanced Conncection Options

<p align="center">
   <img width = "700" src="https://i.ibb.co/C8JJrWX/Step-2-and-Step-3-Authentication.png" alt="Material Bread logo"> 
</p>

2) Click on Authentication

3) Click on Username/Password

<p align="center">
   <img width = "700" src="https://i.ibb.co/qxYh1WP/Step-4-set-username-and-password.png" alt="Material Bread logo"> 
</p>

4) Set Username and Password

<p align="center">
   <img width = "700" src="https://i.ibb.co/BPZqDb0/Step-4i-connected.png" alt="Material Bread logo"> 
</p>

Step 4(i) Mongo Compass connected

<p align="center">
   <img width = "700" src="https://i.ibb.co/QJHyVML/Step-5-click-on-database-then-create-db.png" alt="Material Bread logo"> 
</p>

5) Click on Databases then create Database

<p align="center">
   <img width = "700" src="https://i.ibb.co/5jvFLz2/Step-6-name-db-and-collection.png" alt="Material Bread logo"> 
</p>

6) Name database and collection

<p align="center">
   <img width = "700" src="https://i.ibb.co/C6ycXTh/Step-6-i-db-created.png" alt="Material Bread logo"> 
</p>

6)(i) Database created

<p align="center">
   <img width = "700" src="https://i.ibb.co/wYwhzzJ/Step-7-click-on-db.png" alt="Material Bread logo"> 
</p>

7)Click on database

<p align="center">
   <img width = "700" src="https://i.ibb.co/FYh6M7m/Step-8-click-on-collection.png" alt="Material Bread logo"> 
</p>

8) Click on collection

<p align="center">
   <img width = "700" src="https://i.ibb.co/5TDtnMX/Step-9-click-on-add-data.png" alt="Material Bread logo"> 
</p>

9) Click on add data 

<p align="center">
   <img width = "700" src="https://i.ibb.co/2cJYfby/Step-10-click-on-insert-document.png" alt="Material Bread logo"> 
</p>

10) Click on insert document

<p align="center">
   <img width = "700" src="https://i.ibb.co/sPFCg33/Step-11-insert-data-using-JSON-format.png" alt="Material Bread logo"> 
</p>

11) Insert data

<p align="center">
   <img width = "700" src="https://i.ibb.co/LpXDwfS/Step-11i-data-successfully-added.png" alt="Material Bread logo"> 
</p>

11)(i) Data successfully added

<p align="center">
   <img width = "700" src="https://i.ibb.co/FYfwqpL/Step-12-searching-for-data-final.png" alt="Material Bread logo"> 
</p>

12) Search for data
