# ubuntu22-setup-script
Quick setup for robotics and programmer environment

## Usage
Clone the repository
```
$ git clone https://github.com/gabrielcalmon/ubuntu22-setup-script
```

Give the script execution permission
```
$ chmod +x setup.sh 
```

Execute the script
```
yes | ./setup.sh
```

## Incorrect time in windows (dualboot)

Verify with the command bellow if _RTC in local TZ: no_
```
timedatectl
```

If so, fix it with
```
timedatectl set-local-rtc 1 --adjust-system-clock
```

## Configure SSH

Generate and copy the ssh key
```bash
ssh-keygen -t rsa -b 2048 -C "youremail@address.com"
cd ~/.ssh
cat id_rsa.pub
```

Go to github -> settings -> SSH and GpG keys and click at New ssh key. Give it a name and paste the key.

## ROS2
### Install rosdel
```bash
sudo apt install python3-pip
sudo pip install -U rosdep
sudo rosdep init && rosdep update
```
