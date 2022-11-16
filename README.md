![header](https://capsule-render.vercel.app/api?type=soft&color=006EDB&fontColor=DEEAF7&height=200&section=header&text=PIN_LAB&desc=Project%203&descAlignY=80&fontSize=90)
# PIN_LAB: Project 3

Two-Way Real-Time Voice Communication

## Navigation
1. [Description](#Description)
2. [Getting started](#Getting Started)
3. [Architecture](#Architecture)
4. [Author]

## Description

---

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. 
See deployment for notes on how to deploy the project on a live system.

### Installing & Setting
- Installing the ALSA library used for sound I/O in Linux
    - alsa-utils: Required for sound settings
    - libasound2-dev: Required for sound-related program development
```console
$sudo apt-get install alsa-utils
$sudo apt-get install libasound2-dev
```

- Configuring sound device in the ALSA library
```console
$aplay -l
$plughw : {card_number},{device_number}
$arecord –l
$plughw : {card_number},{device_number}

$alsamixer
```

### Running the tests
```console
gcc { .cpp} -lasound -Wno-write-strings -o { }
```

### docker
[kimakuma8/ubuntu:project3](https://hub.docker.com/layers/kimakuma8/ubuntu/project3/images/sha256-a7c68cba54a68254646067b6d37e700e0ff1d643d7900beafe8b2a5fcd9ea4f2?context=repo)

---

## Architecture
### Test Scenario
![image](https://user-images.githubusercontent.com/76460405/202168003-e979e001-38b4-47fa-be5f-8709350d8306.png)
<img align="center" width="100" height="100" src="https://user-images.githubusercontent.com/76460405/202168003-e979e001-38b4-47fa-be5f-8709350d8306.png">

### Test Bed
![image](https://user-images.githubusercontent.com/76460405/202168300-1d980c54-5547-483f-ba12-6907fcb7ad9a.png)

### Stack

---

## Author

* **Billie Thompson** - *Initial work* - [PurpleBooth](https://github.com/PurpleBooth)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

