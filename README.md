# Analog Recording and Introduction to MAX 8

At the end of the session, you will have created an audio recording, and done your first patch with MAX 8.

This repo (short for repository) contains the activities for this session. If materials are referred to here, download the respective repository as a zip file, unpack it if necessary and then use its contents while working on the tasks outlined here in this README file.

![Audacity with Learning Music](/media/2024-01-09_07-57-54.png)

## What will you do today?

- [ ] Install Audacity and MAX 8
- [ ] Record your first composition made with Learning Music by Ableton and record it with Audacity
- [ ] Do some basic editing of your recording and export the recorded file as .mp3.
- [ ] Create your first MAX patch (program) and make use of your audio recording.


### Installing Audacity and MAX 8

## macOS (Apple M1 or newer)

On an Apple computer you need to install a special audio plugin in addition to Audacity and MAX 8. Here are the instructions:

### Install BlackHole Plugin and Configuration

This plugin runs on Apple M1/M2 and is required if you want to make recordings of sound coming from “within” your computer (sound from a website) Go to [BlackHole](https://github.com/ExistentialAudio/BlackHole)

1. Download and install the BlueHole Application for 2ch
2. Follow the instructions in [Setup Multi-Output-Device](https://github.com/ExistentialAudio/BlackHole/wiki/Multi-Output-Device)


## Audacity (For Windows and macOS)

Install and launch Audacity(https://www.audacityteam.org). Click on Audio Setup and then proceed as described below for macOS or Windows.

![Choose Setup](media/240110_Win11_1_Setup_Audacity.png)


### macOS

Select `BlackHole 2ch` in Audio Setup / Recording Device.


### Windows

Select Windows WASAPI in Audio Setup / Recording Device as described in the screenshot

![Select WASAPI and loopback](media/240110_Win11_2_Setup_Audacity.png)


## Install MAX 8

### School PC: 
1. Find MAX on the netsoft repository and install it (takes time, big application)
2. You are ready to go.

### BYOD: 
1. go to [cycling74](https://cycling74.com/downloads) and download MAX 8 for your operating system.
2. Then install MAX 8.
3. In order to use MAX beyond the 30 days trial version, you need to install a software keyfile on your computer. Ask the teacher for help set it up on your computer.


## Play some music and record it with Audacity
1. Find [Learningmusic by Ableton](https://learningmusic.ableton.com/index.html)
2. Get to know the the Music Device on the homepage and create some songs
3. Record your song with Audacity
4. Export the audio file as mp3


### Audacity settings for Windows 10, recording and sound editing

The video below demonstrates how to set up, record, and edit a sound recording. While the video shows an older version of the Audacity software on Windows, it still applies for macOS and newer Audacity versions, so have a look and follow the guide to record and polish your audio recording.

<iframe width="560" height="315" src="https://www.youtube.com/embed/knL6uKBGyIg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


#### Only for those that have a GitHub Pages site

The code snippet below adds an audio player that allows you to play the mp3 file "220516Rec1.mp3" that has been saved in the folder "assets" inside your repository to show on your website. The Name of the Audio file and the path to where it is saved in your repository may vary if you have a different setup.

``` language=html
<div>
  <audio controls>
    <source src="/assets/220516Rec1.mp3" type="audio/mpeg">
  </audio>
</div>
```


## Get to Know MAX 8 - The Very Basics and Your First Patch

Get started with MAX 8 - Get to know MAX 8 and create your first patch with MAX (programs are called patches), [here](https://youtu.be/XQIWh4AnluI) is a Youtube video that gives you a first introduction. You will learn to assemble a small two channel playlist and control it with buttons.

![My first MAX Patch](/media/2024-01-09_08-59-21.png)

If you want to learn more, have a look at this [video](https://youtu.be/-4nZ6wnVdY8) that also introduces you to MAX. Learn by patching and just recreate the patch introduced and then discover what happens when you remix the patch to tweak it doing other things.


## An Introductory Course to MAX

In the next sessions we will follow along a 20 lesson introduction to MAX that covers the basic objects of MAX.

**MAX** here can have two different meanings:
- It is the name of the overall application comprising all control, audio, and video functionalities. MAX is now in version 8. So if I talk about the application, I will use **MAX 8**.
- MAX is also the name of the control objects and how they can be patched (linked) to do things.


### A Quick Overview of MAX 8:

 **Objects** provide all the functionality in MAX, they "do things". They are represented by boxes, some of them ready-made, some of them need to be defined by typing their name inside an object box. You make things happening by **patching** these objects using **patch cords**. You do so by connecting an **outlet** with a mathching **inlet**. When hovering over the dots representing the inlets and outlets at the top and bottom of an object you see a pop-up text explaining what the inputs and outputs are for.

#### We will use three families or types of objects within MAX 8:

1. **MAX objects** make up and control a patch (**patch** := a MAX 8 program). You can also use *MAX only* to make music and sounds with MIDI. MAX objects are the default objects.
2. **MSP objects** help to make sound and music by generating, manipulating and mixing audio signals. A syntheziser is an example for an instrument that make use of this techniques. You can recognize MSP objects by the `...~` (tilde) symbol at the end of their name.
3. **Jitter objects** create and manipulate video content. You recognize them as their names start with `jit. ...`.

Each of these types of objects comes along with dedicated types of patch cords. They do not mix, so a MAX patchcord cannot carry  Jitter video data and in most cases you need special "translater" objects to link objects of different types.


### Let's Start

These links are for the supportive materials we are using.

#### [20 Objects](http://www.darwingrosse.com/20Objects/index.html)

These 20 lessons cover the basics of MAX (Lesson 1-11), MSP (Lesson 12-14), and Jitter (Lesson 15-20).


#### [Computer Music Programming](https://dobrian.github.io/cmp/week-by-week.html)

The course [Computer Music Programming](https://dobrian.github.io/cmp/week-by-week.html) covers MAX from a different angle, it also contains non-MAX/MSP materials. But it has easy to understand sections describing the basics of digital sound that is helpful if you want to dive deeper into the subject.
