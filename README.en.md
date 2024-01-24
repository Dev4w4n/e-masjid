<p align="center">
  <img src="./public-web/src/assets/home/logo.png" alt="E-Masjid.My" width="80" height="80"/>
</p>

<h2 align="center"><b>E-Masjid.My</b></h2>
<p align="center"><b>Sistem masjid untuk semua</b></p>
<p align="center">
  E-Masjid.My is a free and open source (MIT License) mosque management system
<p><br>
<h2 align="center">
  <a href='https://demo.e-masjid.my'>Live Demo</a>
</h2><br>

Philosophy
=====
The main goals for this system are listed below.

**Easy of use**

- Not everyone is an IT expert. Designing a system for non-IT people needs careful consideration.

**Time to use your IT skills for good deeds**

- Open source is a form of sadaqah which is a required practice in Islam.

**Longer living**

- Hosting/Tech companies may die, but we hope that by open-sourcing this project, it will live longer for the sake of ummah.

**We give, not take**

- We should be contributing to the Muslim community, rather than benefiting from them, especially the Masjid.


## Prerequisites
1. Docker
2. Java 17 (Spring Boot 3.2.0)
3. Maven
4. Node 20 (ReactJS 18 + CoreUI + Tailwind CSS)
5. VSCode (Recommended)

## Minimum Requirement for System Development

1. Docker:
    
    > OS: Windows 10 64-bit: Home or Pro (build 19043 or later), Enterprise or Education (build 19042 or later). Windows 11 64-bit: Home, Pro, Enterprise, or Education version 21H2 or newer.
    
    > Processor: 1.6 GHz or faster 64-bit processor with Second Level Address Translation (SLAT)
    
    > Memory: 4 GB RAM
    
    > BIOS-level hardware virtualization support must be enabled in the BIOS settings
    
    > Hyper-V and Containers Windows features must be enabled

2. Java:

    > OS: Windows 10 and 11 (64-bit), macOS versions with Apple security update support, Linux (Debian): Ubuntu Desktop 20.04, Debian 10, Linux (Red Hat): Red Hat Enterprise Linux 8, Fedora 36
    
    > RAM: 128 MB
    
    > Disk space: 124 MB for JRE; 2 MB for Java Update
    
    > Processor: 1.6 GHz or faster 64-bit processor

3. Maven:
    > OS: Windows, macOS, Linux
    
    > Java SDK installed

4. Node:
    > OS: Windows 10 and 11 (64-bit), macOS versions with Apple security update support, Linux (Debian): Ubuntu Desktop 20.04, Debian 10, Linux (Red Hat): Red Hat Enterprise Linux 8, Fedora 36

5. VSCode:
    > OS: Windows 10 and 11 (64-bit), macOS versions with Apple security update support, Linux (Debian): Ubuntu Desktop 20.04, Debian 10, Linux (Red Hat): Red Hat Enterprise Linux 8, Fedora 36
    
    > Processor: 1.6 GHz or faster 64-bit processor
    
    > Memory: 1 GB of RAM

## Quickstart guide ( Docker compose )
### Clone this repo
```
git clone https://github.com/Dev4w4n/e-masjid.my.git;
cd e-masjid.my
```
### run-dev.sh (for Linux)
```
sh run-dev.sh
```
### run-dev.sh (for Windows) - Use Git Bash terminal in VSCode
```
sh run-dev.sh
```

This will automatically build all the APIs, and run the docker-compose file where it will spin up 6 containers for the developments environment.

Once the containers are up, you may stop any of the containers depending on what you will be working on to free up your local resources.

## Gradle Build

You may utilise ./gradlew (or gradlew.bat on windows) provided to configure/execute your build. The commands below will show available tasks on gradle:

```sh
./gradlew task

./gradlew task --all
```

### Gradle build for each backend modules

As seen in the output of the aforementioned `./gradlew task --all`, you may execute builds separately for each of the backend modules. Each backend modules are written in Spring boot, so you may use org.springframework.boot plugin as below:

```sh
cd api

./gradlew api:tabung-api:bootRun --args='--spring.profiles.active=local'
```

You may also generate the Jar file separately for the use with docker-compose. Follow the step below to generate Jar:

```sh
cd api

./gradlew api:tabung-api:bootJar
```

## Contributing guide

Please fork this repo and submit your Pull Request.

We love your input! We want to make contributing to this project as easy and transparent as possible, whether it's:

- Reporting a bug
- Submitting a fix
- Proposing new features
- Enhancing features
- Documentation
- Unit testing
  
Or you would just like to chat with us, find us on [Discord](https://discord.gg/vz4WWM85)

