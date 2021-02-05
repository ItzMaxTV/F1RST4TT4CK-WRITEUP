# F1rst-4tt4ck Write Up
A beginner-level CTF challenge as one of the [TryHackMe room](https://tryhackme.com/room/f4), which focus on Stenography, Cracking, and processing audio files.

## Authors 
* [ItzMaxYT](https://tryhackme.com/p/ItzMaxYT)
* [CrUsHiNg](https://tryhackme.com/p/CrUsHiNg)

## [Task 1] Intro
Topic : Intro
* A basic intro to the room and to the tools.

## [Task 2] Cracking
Topic : Cracking
* Tools: John The Ripper, Sonic Visualiser

#### How to solve : 
* We'll be using John The Ripper and Sonic Visualiser to solve this

Firstly, type "zip2john [file.zip] > hash"

The hash file will be automatically saved to your working directory.

Then you'll have to type "john hash --wordlist=/usr/share/wordlists/rockyou.txt

The password of the ZIP will be cracked instantly and will be showen on the Terminal.

You will then extract the files from the ZIP file and start [Sonic Visualiser](https://www.sonicvisualiser.org/)

There will be audio file, try dragging it into Sonic Visualiser. Next, press on Layer > Add Spectrogram > audio.wav: All Channels Mixed

You will have to change the color to Blue and Black
Scale, Linear and Hybrid
Bins, All Bins and Linear

Then the flag will gradually pop out from out of all the colors.

## [Task 3] Stenography
Topic : Stenography
* Tools: Sox

#### How to solve : 
* We'll be using [Sox](http://sox.sourceforge.net/)

Again, open up a Terminal and start typing "sox audio.mp3 newaudio.mp3 reverse"









