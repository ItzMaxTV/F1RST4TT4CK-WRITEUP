# F1rst-4tt4ck Write Up
A beginner-level CTF challenge as one of the [TryHackMe room](tryhackme.com/jr/f4), which focus on Stenography, Cracking, and processing audio files.

## Authors 
* [ItzMaxYT](https://tryhackme.com/p/ItzMaxYT)
* [CrUsHiNg](https://tryhackme.com/p/CrUsHiNg)

## [Task 1] Intro
Topic : Intro
* A basic intro to the room and to the tools.

## [Task 2] Cracking
Topic : Cracking
* Tools: John The Ripper, Sonic Visualiser

Okay, we will launch the terminal and start cracking.

#### How to solve : 
* We'll be using John The Ripper and Sonic Visualiser to solve this

Firstly, type "zip2john [file.zip] > hash"

The hash file will be automatically saved to your working directory.

Then you'll have to type "john hash --wordlist=/usr/share/wordlists/rockyou.txt

The password of the ZIP will be cracked instantly and will be showen on the Terminal.







