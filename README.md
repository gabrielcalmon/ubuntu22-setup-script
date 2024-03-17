# ubuntu22-setup-script
Quick setup for robotics and programmer environment

## Usage
Clone o repositório
```
$ git clone https://github.com/gabrielcalmon/ubuntu22-setup-script
```

Forneça permissão de execução para o script
```
$ chmod +x setup.sh 
```

Execute o script
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
