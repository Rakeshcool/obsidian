```
sudo apt install openjdk-8-jdk           # choose this or next line
sudo apt install openjdk-11-jre-headless # or Install Java 11 JDK/JRE
sudo apt install Jenkins
```
```
wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add
sudo bash -c 'echo deb https://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'
sudo apt update
sudo apt-get install jenkins
```
```
sudo ufw enable
sudo ufw allow 8080 # whatever port number you like
```
```
sudo ufw status
```
```
sudo service jenkins start
```
```
http://localhost:8080/
```