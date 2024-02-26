# jrecraft-server

JREcraft Minecraft Server

## NOTE: This GitHub repo is still being setup. It may not work and instructions are going to be very unhelpful at first.

# Setup

I did all of this with Minecraft 1.20.4 on Ubuntu 23.10, so all instructions will be for that.

Most of it really shouldn't matter (Windows, Mac, or Linux) as long as you have Java and whatever else is required to run a Paper (Spigot) server.

### Install Java
The default Java in Ubuntu is Java 17 which is fine. You'll need wget in the next step so get that too

	sudo apt install default-jdk wget

### Download Paper (Server)
I'm not going to include it because I don't want to read the license.
Terminal into your jrecraft-server directory and type:

    wget https://api.papermc.io/v2/projects/paper/versions/1.20.4/builds/408/downloads/paper-1.20.4-408.jar

### Edit server.properties

Edit the `server.properties` file to your specifications.

`NOTE: The JREcraft world seed is not currently public. Your world will not look like ours.`

### Run it
	java -Xmx3g -jar paper*

Replace 3g with the max amount of RAM you want the server to use.

### Connect to it

NOTE: You may want to open the ports in Ubuntu's firewall

	sudo ufw allow 25565

Connect to your server via its IP address. If you set it up on the computer you plan to play on then your IP is probably `localhost`  or something.