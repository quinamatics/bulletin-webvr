# Bulletin
![Bulletin VR](project/static/assets/blong_large.png)

## Introduction
We tackle social anxiety by creating a shared interactive virtual reality bulletin board to allow users to anonymously post encouraging messages. [Try it out! (https://bulletinvr.online)](https://bulletinvr.online)

## Inspiration
Social anxiety affects hundreds of thousands of people and can negatively impact social interaction and mental health. Around campus, we found bulletin boards with encouraging anonymous messages, and we felt that these anonymous bulletin boards were a viable approach to combat social anxiety. Previous studies have shown that people with social anxiety felt more comfortable with online interaction and that online interaction decreases social anxiety even more in people with high levels of social anxiety or depression. With these results, we decided that an online platform would enhance the capabilities of the aforementioned bulletin boards. Further, being online can add yet another layer of anonymity to encourage those struggling with social anxiety to contribute their voices.

## What is BulletinVR?
BulletinVR is a user-friendly, fully-immersive, interactive, and anonymous online virtual reality bulletin board for positive and encouraging messages. Using a virtual reality platform for these bulletin boards can add interactivity and make communication feel more personal and realistic. Eliminating keyboard controls allows the experience to be completely immersive, minimizing technological distractions. Using speech-to-text would both make the platform easy to use and allow users to become fully immersed in the experience, using their literal voice to contribute to the bulletin. We do not store any user information in our backend, promoting the anonymity of our platform.

## What is WebVR?
WebVR, or Web-based virtual reality allows for users to experience a computer-generated 3D simulation through their own web browser. This provides a much greater ease of access because users can access virtual reality without other browsers or technology.

We chose to create a WebVR application to promote social wellness because of we wanted to build a fluid means of communicating positive messages over an aesthetically-pleasing, smooth interface. WebVR lets us create an immersive message board that is available for anyone to use and anyone to contribute to. The code behind it is free to use and anyone can modify it, creating a continually updating landscape as developers add to and improve upon it.

The advantages of a Web-based virtual reality (shortened to WebVR) application over a traditional system-dependent virtual reality application are its wide availability (as internet-connected devices are commonplace), elimination of any proprietary software or hardware, and its open-sourced nature. The code behind it is free to use and anyone can modify it, creating a continually updating landscape as developers add to and improve upon it.

## How it works
Our platform uses the A-Frame WebVR Framework to create VR scenes that can run in a browser environment. Every five seconds, the JavaScript script uses AJAX to make a request to the Flask-powered server. The server queries the database and returns the messages that the frontend should display. If a user submits their own message, the server checks the message to see if it is appropriate and then saves it to the database, replacing old elements if the current number of messages is above the capacity that we define.
## Installation
Installing everything is very simple. After cloning the Repo to your computer, enter the folder.

If you don't have `virtualenv` installed for Python, run
``` bash
pip install virtualenv
```

Make a virtual environment:
``` bash
python -m venv virt
```

To activate the environment, on Windows run:
``` bash
virt\Scripts\activate
```

And on Linux or Mac run:
``` bash
source virt/bin/activate
```

To install the necessary pip packages into the environment, run:
``` bash
pip install -r requirements.txt
```

Finally, to run the Python application, run:
``` bash
python application.py
```

Now you can go to `http://localhost:5000/` and use the application.

## Team Members
- [Kevin Chen](https://github.com/k3vnchen), [kevin.n.chen@yale.edu](mailto:kevin.n.chen@yale.edu)
- [Mykyta Solonko](https://github.com/msolonko), [mykyta.solonko@yale.edu](mailto:mykyta.solonko@yale.edu)
- [Hamilton Wan](https://github.com/wanh23), [hamilton.wan@yale.edu](mailto:hamilton.wan@yale.edu)
- [Brandon Zhu](https://github.com/quinamatics), [brandon.zhu@yale.edu](mailto:brandon.zhu@yale.edu)

![B VR](project/static/assets/bulletin.png)
