# project3
Two-Way Real-Time Voice Communication

docker -> kimakuma8/ubuntu:project3


![header](https://capsule-render.vercel.app/api?type=soft&color=006EDB&fontColor=DEEAF7&height=200&section=header&text=PIN_LAB&desc=Project%203&descAlignY=80&fontSize=90)
# PIN_LAB: Project 3

Two-Way Real-Time Voice Communication

## Navigation
1. [Description](#Description)
2. [Getting started](#Getting Started)
3. [Architecture](#Architecture)
4. [PoC]
5. [Author]

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
- Test Scenario
![image](https://user-images.githubusercontent.com/76460405/202167691-354c86f0-4664-4796-9dfd-8020f3d18030.png)
![image](https://user-images.githubusercontent.com/76460405/202168003-e979e001-38b4-47fa-be5f-8709350d8306.png)



## Deployment

Add additional notes about how to deploy this on a live system

## Built With

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency Management
* [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Billie Thompson** - *Initial work* - [PurpleBooth](https://github.com/PurpleBooth)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc
