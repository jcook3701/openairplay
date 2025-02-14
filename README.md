# OpenAirplay 0.0.32

Stream from a Linux computer to an Airplay Receiver.

OpenAirplay is a python implementation of the Apple Airplay client, intended to mimic the OSX Airplay integration.

I have always been annoyed about how iOS, Mac OSX, and all of Apples proprietary hardware/software has inhibited so many of us technology savvy people.  

## Getting Started

1. Clone the repository.  
```
$ git clone https://github.com/openairplay/openairplay.git
```

2. Move into the newly cloned project directory.  
```
$ cd openairplay
```

3. Initialize and pull sub-modules.  
```
$ git submodule update --init --recursive
```

### Automated Virtual Environment Setup
1. First run will install python3 virtual environment and all proceeding runs will start Open Air Play.  
```
$ ./run.sh
```

### Manual Virtual Environment Setup
1. Create python 3 virtual environment.  
```
$ python3 -m venv env
```

2. Source the python environment.  You should see the name of the environment in parentheses after running the following command.  
__Note:__ Python virtual environment will have to be soured every time before you run openairplay.   
```
$ source ./env/bin/activate
```

3. __Optional:__ Upgrade newly created virtual environment's pip.  
```
$ python -m pip install --upgrade pip
```

4. Install python packages that are needed to run this project.  
```
$ python -m pip install -r requirements.txt
```

5. Run Open Air Play
```
$ python3 -m openairplay.gui_main
```

## Doxygen Documentation

1. Generate [Doxygen](https://www.doxygen.nl/manual/docblocks.html) documentation.  
__Note:__ Doxygen requires code to be commented in a special format to auto generate documentation.  
```
$ doxygen
```

## Project Status:

**No longer under active development.**

I no longer attend my high school full of Apple devices, so I have no platform to test this project on.

If someone wants to fund this project, buy me a 2nd gen Apple TV or later so I can actually get back to work on this project.

Otherwise, I have no need or ability to continue development, so if you are able and willing, send over some PRs or code edits.

https://github.com/robobenklein/openairplay/milestones

## Project Details:

Right now it's Python 3 using the QT system from PyQt4.  
It is designed in an Ubuntu Unity environment, but the application should work on any platform with Python 3 and a system tray.  
From my last testing, this ran fine on my Dad's Windows 8 laptop, and I've tested Ubuntu 14.04 to 15.10.

## Requirements:

See the `dependencies.md` file for installing the needed software.

## Why I'm doing this:

(From 2015:)  
I go to a school where everyone has iPads as their learning tool, which are horrid for coding/programming and software development, but make a good classroom common tool. As a result, there is an Apple TV in every single room for the students to quickly present whatever is on their screen, and the teachers can show their presentations with their assigned Macbooks.

I am one of two people at this school who use Linux (Ubuntu) and who bring their laptops every day. I use mine for school work fairly often, as I understand how much I can do in Linux and not iOS. But whenever some task comes up where I'd need to airplay my work to an Apple TV, I'm being restrained to my iPad.

## What this aims to be:

This application is designed to sit in your System Tray just like in OSX, with a drop down list of available Airplay Receivers, and allow you to:
- Stream your desktop  
- Send a photo/picture  
- Play a video  
- Stream Music  
And whatever else the users and developers of this project wish it to be.

## Want to help?

I'm always looking for contributors, if you can help with any of these I'd love to work with you.  
 * Python network discovery protocols (for finding listings of devices)
 * Airplay/Media protocols
 * Python Qt (thinking about things like screen capture)
 * And developers to help make this work for non-Ubuntu OSs.

