# blockchain

# scoe

AWS Instance:

1. Login/Register into AWS console:
https://ap-south-1.console.aws.amazon.com/ec2/home?region=ap-south-1#Instances:

2. Connect to the AWS instance

3. sudo apt update

4. Install git and curl
	- sudo apt-get install git
	- sudo apt-get install curl

5. Install Docker
	sudo apt-get -y install docker-compose

6. Now check if docker is proeprly installed
	- docker --version
	- docker-compose --version

7. Make sure docker daemon is running
	sudo systemctl start docker

8. Install GoLang
	- curl -O https://dl.google.com/go/go1.18.3.linux-amd64.tar.gz
	- tar xvf go1.18.3.linux-amd64.tar.gz
	- export GOPATH=$HOME/go
	- export PATH=$PATH:$GOPATH/bin

9. Install Hyperledger fabric
	curl -sSL https://bit.ly/2ysbOFE | bash -s -- 2.4.9 1.5.5

	Note: Incase of permission denied run the command:
		 sudo chmod 777 /var/run/docker.sock

10. Check if hyperledger fabric is installed...
	docker images
