# Face-Detection-using-OpenCV

> **Archived.** This project and [FaceRecognition-OpenCV-RaspberryPi](https://github.com/pranavragji/FaceRecognition-OpenCV-RaspberryPi) were merged into [Facelog](https://github.com/pranavragji/facelog), a face recognition attendance and door log with a web dashboard. It swaps the Haar cascade and LBPH used here for YuNet and SFace, which name people correctly far more often. Facelog is private for now. The code below is left as it was in 2019.

For this project you require

1.Raspberry Pi

2.Pi Cam

3.Python 3

4.OpenCV

In this project we have to just detect our face through the haar cascade algorithm and show it.

I am using the Rasbian OS for the Raspberry Pi3B+. The NOOBS OS can be used for this project as well.

Steps:

-Enable Camera from the interface options in the terminal (raspi-config)

-Install OpenCV3 (This may take 5-6 hours)

-After Installing OpenCV Test Your Camera by using the simpleCamTest.py File

-Then run the faceDetection file.

Notes:

The Blue sticker side of the Pi Cam should be facing the USB ports.

sudo modprobe bcm2835-v4l2 <--- This is an important code which helped me throughout this project. If while running the camera you get an assertion failed error, running the code will solve it.

For displaying your raspberry pi to your Windows Computer you can use RemoteDesktop. You require your RaspberryPi's IP address which you can find by using the ifconfig command and taking the inet address. This address will connect you to your raspberry pi and you will have to put your username and password for your pi. Typically your username is "pi" and password is "raspberry". But you have to enable SSH from your interfacing options.

To shutdown your Raspberry Pi from RemoteDesktop run this Command. (sudo shutdown -h now)

References:

https://www.hackster.io/mjrobot/real-time-face-recognition-an-end-to-end-project-a10826

https://www.hackster.io

https://www.pyimagesearch.com/
