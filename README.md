![header](https://capsule-render.vercel.app/api?type=soft&color=006EDB&fontColor=DEEAF7&height=200&section=header&text=PIN_LAB&desc=Project%203&descAlignY=80&fontSize=90)
# PIN_LAB: Project 3

Two-Way Real-Time Voice Communication

## Navigation
1. [Description](#Description)
2. [Getting started](#Getting-Started)
3. [Architecture](#Architecture)

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
sudo apt-get install alsa-utils
sudo apt-get install libasound2-dev
```

- Configuring sound device in the ALSA library
```console
aplay -l
plughw : {card_number},{device_number}
arecord –l
plughw : {card_number},{device_number}

alsamixer
```

### Running the tests
```console
gcc {file_name.cpp} -lasound -Wno-write-strings -o {exe_name}
```

### docker
[kimakuma8/ubuntu:project3](https://hub.docker.com/layers/kimakuma8/ubuntu/project3/images/sha256-a7c68cba54a68254646067b6d37e700e0ff1d643d7900beafe8b2a5fcd9ea4f2?context=repo)

---

## Architecture
### Test Scenario
![image](https://user-images.githubusercontent.com/76460405/202168003-e979e001-38b4-47fa-be5f-8709350d8306.png)

### Test Bed
![image](https://user-images.githubusercontent.com/76460405/202168300-1d980c54-5547-483f-ba12-6907fcb7ad9a.png)

### Stack
- Language
<svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><title>C</title><path d="M16.5921 9.1962s-.354-3.298-3.627-3.39c-3.2741-.09-4.9552 2.474-4.9552 6.14 0 3.6651 1.858 6.5972 5.0451 6.5972 3.184 0 3.5381-3.665 3.5381-3.665l6.1041.365s.36 3.31-2.196 5.836c-2.552 2.5241-5.6901 2.9371-7.8762 2.9201-2.19-.017-5.2261.034-8.1602-2.97-2.938-3.0101-3.436-5.9302-3.436-8.8002 0-2.8701.556-6.6702 4.047-9.5502C7.444.72 9.849 0 12.254 0c10.0422 0 10.7172 9.2602 10.7172 9.2602z"/></svg>
- OS
