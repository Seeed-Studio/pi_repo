Seeed deb Package Repository for Embeded Linux Platform
==============================================

| Codename | Architecture | Architecture |
|----------|--------------|--------------|
| stretch  | armhf        | arm64        |


### Add repository
```
echo "deb https://seeed-studio.github.io/pi_repo/ stretch main" | sudo tee /etc/apt/sources.list.d/seeed.list
```

### Add public GPG key
```
curl https://seeed-studio.github.io/pi_repo/public.key | sudo apt-key add -
```
or
```
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys BB8F40F3
```


### Install MRAA & UPM
```
sudo apt update
sudo apt install python-mraa python-upm
```

### Install librespeaker & respeakerd
```
sudo apt update
sudo apt install librespeaker respeakerd
```
