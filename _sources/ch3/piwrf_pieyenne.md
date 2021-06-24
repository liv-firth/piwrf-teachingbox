# Pieyenne

![title](piwrf_pieyenne.jpeg)

Build NCAR's Supercomputer with Raspberry Pis!

## Overview
With more and more digital data being collected every day. Although home computers are getting faster and are able to process more data than ever, there still exist large complex scientific problems that are too complex and produce too much data for any top-of-the-line computer anyone can purchase (as of 2019).

To tackle these difficult problems, supercomputers and clusters are used to. These machines are not necessarily a one-off expensive machine, but they are essentially high end desktop computers that are all networked together to allow for each individual computer to work on a portion of the problem in tandem.

The scale computers can scale and are only constrained by budgets. Supercomputers can cost tens of millions of dollars and consist of thousands of individual computers. 

## Goal
The goal of this project is to build a computing cluster with Raspberry Pis. HAving the cluster will allow for some applications to run whereas it will not be able to run on a single Raspberry Pi. To complete the project, users will need to download and upload file, create a local area network with a router, and run install scripts.

## Who this is for
This project is recommended for grades 9-12 (high school). The project will require typing skills, downloading and running scripts. 

## Equipment

### 1. [Raspberry Pi 4](https://www.raspberrypi.org/products/raspberry-pi-4-model-b/ "Raspberry Pi 4 Homepage") (minimum of 2) - There are three versions of the raspberry pi 4 that are available. Computing power and price increases with each version of the Raspberry Pi4 but the lowest level will suffice for this project. 

### 2. [Raspberry Pi Power Supply](https://www.raspberrypi.org/products/type-c-power-supply/ "Raspberry Pi Power Supply Homepage") - This is a special USB-C power adaptor that will power your Raspberry Pi.

### 3. Micro SD CARD for each Pi - The amount of storage varies widely for SD cards. A minimum of 32GB will suffice for this project. 

### 4. HDMI Cable.

### 5. [Network Switch](https://www.amazon.com/Computer-Networking-Switches/b?ie=UTF8&node=281414 "Amazon Network Switch") (not a router  and enough ports for each pi) - It is not recommended to use a router in place of a switch. The price of the switch increases with speed and performance. For this project, a basic switch is recommended to save costs (10/100) 

### 6. Ethernet cables for each Pi

### 7. USB Mouse/Keyboard

### 8. Monitor

### 9. Personal computer/laptop

### 10. Power strip

## Supercomputers Today

### Today's Supercomputers and Data Centers

NCAR’s has a long history of owning and using supercomputers that dates back to 1970's. Historically, these computers have been used to advance our knowledge of weather and climate. NCAR's current supercomputer “[Cheyenne](https://www2.cisl.ucar.edu/ncar-wyoming-supercomputing-center "NCAR-Wyoming Supercomputing Center")” is based in Cheyenne, Wyoming. Although the primary research done on Cheyenne is tailored to weather and climate research, it is also used in other fields such as renewable energy research, engineering, astrophysics, data science, and artificial intelligence.

![title](cray1.jpeg)

![title](cray2.jpeg)

The world’s most powerful supercompter is named Summit (as of 2019) and is located in Oak Ridge, Tennessee at Oak Ridge National Laboratory. There are internal components of Summit that differ from Cheyenne, but the concept is the same. The research done on Summit focuses on energy research include, nuclear fusion, cancer research, biology, chemistry, and material science.

![title](summit.jpeg)

Cloud Supercomputers: Since supercomputers require dedicated facilities (sometime their own power grid) it is not feasible for some organizations to build one. With this in mind, “cloud supercomputers” do exist. Several large tech companies offer cloud computing resources to individuals or organizations on a pay-as-you-go basis. 

![title](cloud.jpeg)

## Pieyenne Instructions

### 1. Download Cheyenne Image and Cloning Software

*Disclaimer*
The first section is optional but **Highly Recommended**! If you choose to forego the first section, the files may not install correctly and permissions on your Raspberry Pi will be changed. Fixing these problems is not time consuming but it will require technical expertise.

In the first section you will download the Cheyenne Image to your computer and then upload it to your micro SD card. The image file you will download is an .ISO image file that contains the entire Raspbian operating system and all of the necessary software combined into a single file. Since this is a unique type of file, you cannot simply copy and paste the file onto your micro SD card. You will need a program that will not only copy the file to the micro SD card, but will also format the .ISO image file so that it knows how to control your Raspberry Pi. Formatting the .ISO image file and copying it to a micro SD card is known as “flashing the image” to a micro SD card. Once you have flashed the image to your micro SD card, you can then use your Raspberry Pi.

#### 1.1 Download the Raspberry Pi image
The first step of this section is to download the .ISO image file to your personal computer or laptop ( this step will work for any operating system). Right click on the blue link and choose “save link as” [insert address for print version]. This will prompt you to save the link to the destination of your choice. Once you do this simply hit enter or select “OK” and the download will start.
*Depending on the speed of your network, this may take 5-20 minutes.*

#### 1.2 Download the software to flash the .ISO image to a micro SD card 
After downloading the image file, you will need special software to flash the .ISO image to a micro SD card. You may already have some software capable of this installed on your computer. If this is the case, you are welcome to use any software to flash the image. We recommend Etcher as the program of choice. The software is open-source, secure, and freely available. To download Etcher go to this website (link) and you will see a button to download the program based on your operating system. Select your operating system and choose install. You may install it in the location of your choosing. 

#### 1.3 Flash the micro SD card
Now you will need to insert you micro SD card either directly into you computer or through some sort of adapter. Once you micro SD card is recognized by your computer you are ready to flash it. Open Etcher or your program of choice, and you will be prompted with a menu. First you will click the button to select your image (in this case it is the Cheyenne .ISO image file you just downloaded). You will then be prompted to choose the image file you downloaded in the previous step. After that, you must select drive, which is your micro SD card. Once that is done, you may click "flash".

#### 1.4 Repeat the flash steps for each micro SD card you will use

### 2. Setup your hardware

Since you have your micro SD card formatted, it will act as your Raspberry Pi’s hard drive. Now, you simply need to set up the hardware for your cluster.

#### 2.1 Insert micro SD cards
The slot for the micro SD card is located at the bottom of the Pi (see diagram). Insert it into the slot and it should be a snug fit once it is in all the way. The chassis is designed such that the micro SD card will only fit one way so you will not have to worry about orientation.

#### 2.2 Insert ethernet cables
After the flashed micro SD have been inserted into each Raspberry Pi, you must insert your ethernet cables into each Pi. There is a square ethernet jack that is located at the front of each Pi. When you connect your ethernet jack you may hear an audible click and it will lock into place if done correctly. 

#### 2.3 Connect ethernet cables to router
After you have connected the ethernet cable into the Pi, you must do it again for the ports on your switch. Like the Raspberry Pi, you may hear an audible click and it will be a snug fit. 

#### 2.4 Connect peripherals (keyboard, mouse, and hdmi cable)
After these are done, you will need to connect your peripherals. Each Raspberry Pi needs a power source. In addition, you must designate one of your Pis to be a head node. You will connect your keyboard, mouse, and monitor to the head node. 

#### 2.5 Power up the system
Now you need to plug in your power sources and plug in your router. Once electricity is delivered to each Pi and the switch, they will turn on automatically.

If this is successful, you should see this desktop menu.

#### 2.6 Connect to the internet

### 3. Configure the Cluster

Assuming your Pis are up and running, you will need to configure it so that each Raspberry Pi can ‘communicate’ with each other. In order to do this you will use a script or automated program that finds the IP addresses of all the Raspberry Pis. This is how the system finds all the Pis. Once it does that, it open changes permissions and allows each Raspberry Pi to “talk to one another”

#### 3.1 Launch terminal
Once all of your Pis are turned on and connected to your switch, you can begin to configure your cluster. To this you will need to first open the terminal (see definition appendix). The terminal is a “bare-bones” interface for your Raspberry Pi. You can do some of the same commands as you normally can on your desktop, (create, copy or move files, open applications, logout, etc) but other commands are also accessible. Do this by clicking this tab in the upper left of your screen. (insert picture). After doing so a black window should appear with a cursor. If you see this text prompt or something similar, you have opened your terminal. Alternatively, you can open the terminal by pressing the following keys together Control+Alt+t

#### 3.2 Run configure script
f you used the Raspberry Pi image file, then the software will already be installed onto your Raspberry Pi. You simply need to type the following commands into your terminal:

```bash
wget https://github.com/wefoust/Build-a-Rpi-Cluster/archive/master.zip
```
```bash
unzip master.zip
``` 

```bash
.mv Build-a-Rpi-Cluster-master/* ..
``` 

```bash
rm master.zip & Build-a-Rpi-Cluster-master
``` 

Depending on the size of your cluster, the first phase of the script will take up to 15 minutes to complete depending on the size of you cluster. Throughout the script you will be asked for permission to continue and for passwords. 

Whenever you are asked to continue: type ‘yes’
Whenever you are asked for a password, type raspberry.

This will be done many times depending on your cluster.

#### 3.3 Set the date and time of your system
Once your Pi turns on you will need to configure a few settings based on your location and time. First, you will need to setup your timezone and time. To do this click the start menu and then click settings. From there go to date and time, and configure your timezone. Once that is done, connect to the internet by clicking the upper right and choosing network. You can test if you are successfully connected by launching a web browser by going to chromium and going to any website.

### 4. Monitor Your Cluster

With expensive high performance systems, it is important to monitor them to make sure they are always working at full capacity. NCAR has dedicated staff that monitors the system 24/7 to ensure the maximum amount of work is done on the system as possible. In this section you will configure a dashboard so that you can monitor exactly what your cluster is doing. 

#### 4.1 Run the monitor_cluster script
To run the script type the following commands:

```bash
cd /home/pi/cluster_monitor/
``` 

```bash
./monitor_configuration
``` 

```bash
./start_monitoring
``` 

After you type the final command, do not close the terminal window.

#### 4.2 Setup Grafana
Once the cluster has started the monitoring process, you may set up your dashboard. To do this, open the Chromium web browser that is preinstalled on all Raspberry Pis. To Launch Chromium, click the icon in the upper left of the toolbar. 

Once the browser has been launched, type the following command in the address bar
htt[://localhost:3000 

Once it has started you will be prompted with a sign-in menu. You DO NOT need to register. The default username and password is
username : admin
Password : admin

