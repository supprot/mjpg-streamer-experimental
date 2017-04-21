 
Download the project 
https://github.com/supprot/mjpg-streamer-experimental.git

Copy the package to your raspberyPi by SSH.Then:

	unzip mjpg-streamer-experimental-master.zip
	sudo apt-get install cmake
	sudo apt-get install libjpeg8-dev  
	cd mjpg-streamer-experimental-master
	make clean all
	sudo raspi-config  Enable Camera
	sudo reboot
	cd mjpg-streamer-experimental-master
	./mjpg_streamer -i "./input_raspicam.so" -o "./output_http.so -w ./www"  


Then open your browser, enter the following url can see static screenshots:

http://<your raspberryPI IP>:8080/?action=snapshot

Enter the following two url can see dynamic image:

http://<your raspberryPi IP>:8080/javascript_simple.html  



