# Pi-WRF Setup

These instructions assume your [Raspberry Pi](https://www.raspberrypi.org "Raspberry Pi Homepage") is already up and running.

## Section 1. Download and install Docker on your Raspberry Pi 

The WRF application is run through a program called [Docker](https://www.docker.com "Docker Homepage"). It is too complicated for this lesson on how Docker works, but a good description can be found here. Once you have Docker installed onto your computer, it will be very easy to launch the application on your Raspberry Pi.

### 1.1 Install Docker by opening a terminal and typing

```bash
curl -sSL https://get.docker.com | sh
``` 

### 1.2 Launch the application by copying and pasting the following command

```bash
sudo docker run -it --rm --net=host -e DISPLAY -v $HOME/.Xauthority:/root/.Xauthority ncar/pi-wrf
```
When you enter the following command and execute it, Docker downloads the file for you and then launches it. If you close the program, Docker will save the “file” so you do not have to download it the next time you run the application.


## Section 2.  

Once you have launched the appliction, it is time to run it. The app allows you to configure when you want the model to run and for how long. Follow the steps below to make your first forecast.

### 2.1 Click the Run Forecast Button.

### 2.2 Select a start and end date, and confirm your selection.

### 2.3 Click and drag the domain you would like to select. The map automatically zooms to your domain. If you accidentally choose a domain that is too small, then you may either zoom out or reset the domain. Once you are done, click the run model tab.

### 2.4 Press the run model button when you are ready to run the model. After the model finishes, a button will appear to view the output. Click it to see the results of the model.

## Verify Your Results:

Websites like these are great for determining the observations of your domain: 

[National Weather Service](https://w2.weather.gov/climate/index.php?wfo=bou "National Weather Service Forecast Office: Denver-Boulder, CO")

