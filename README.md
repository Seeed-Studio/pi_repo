Seeed deb Package Repository for Embeded Linux Platform
==============================================

| Codename | Architecture | 
| :------: | :----------: |
| stretch  | armhf        | 
| bionic   | arm64        |
| mendel   | arm64        |


### Add repository
```
#For raspberry pi
echo "deb https://seeed-studio.github.io/pi_repo/ stretch main" | sudo tee /etc/apt/sources.list.d/seeed.list

#For Google Coral dev board
echo "deb https://seeed-studio.github.io/pi_repo/ mendel main" | sudo tee /etc/apt/sources.list.d/seeed.list

#For Nvidia Jetson nano
echo "deb https://seeed-studio.github.io/pi_repo/ bionic main" | sudo tee /etc/apt/sources.list.d/seeed.list
```

### Add public GPG key
```
curl https://seeed-studio.github.io/pi_repo/public.key | sudo apt-key add -
```

### Install MRAA & UPM
```
sudo apt update
sudo apt install python-mraa python-upm
```

### Install librespeaker & respeakerd (only works on RPI)
```
sudo apt update
sudo apt install librespeaker respeakerd
```
