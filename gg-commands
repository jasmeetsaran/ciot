## Install Python and Git
sudo apt install -y python3 python3-pip git

## Install Java 11 LTS
wget -O - https://apt.corretto.aws/corretto.key | sudo gpg --dearmor -o /usr/share/keyrings/corretto-keyring.gpg && echo "deb [signed-by=/usr/share/keyrings/corretto-keyring.gpg] https://apt.corretto.aws stable main" | sudo tee /etc/apt/sources.list.d/corretto.list

sudo apt-get update; sudo apt-get install -y java-11-amazon-corretto-jdk

## Install GreenGrass gdk
pip3 install git+https://github.com/aws-greengrass/aws-greengrass-gdk-cli.git@v1.6.2 --break-system-packages

## Install AWS cli
curl "https://awscli.amazonaws.com/awscli-exe-linux-aarch64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install

## Create Component
gdk component init -n <package name> -l (language) -t HelloWorld

where: 
-n specifies your package name
-l specifies language (either java or python)
-t specifies template name here in our case it is HelloWorld

###For more templates:
https://github.com/aws-greengrass/aws-greengrass-component-templates

## Configure Packages
Modify: gdk-config.json

## Build Packages
gdk component build

## Publish Packages

Check if the package is deployed on Pi
sudo /greengrass/v2/bin/greengrass-cli component list

