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
