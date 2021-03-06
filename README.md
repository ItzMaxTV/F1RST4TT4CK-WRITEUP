# F1rst-4tt4ck Write Up
A beginner-level CTF challenge as one of the [TryHackMe room](https://tryhackme.com/room/f4), which focus on Stenography, Cracking, and processing audio files.
Don't forget to run this command before starting!

apt-get update -y && apt-get upgrade -y && apt-get install libsox-fmt-mp3 -y


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

* What is the song name?

Again, open up a Terminal and start typing "sox audio.mp3 newaudio.mp3 reverse"
The audio file will then be reversed, then start typing "sox newaudio.mp3 lastaudio.mp3 tempo 0.5" to slow it down.
Use the App "Shazam" to identify the name of the song.

* Checking the metadata, what is the original date of the audio?

You will have to use [Metadata2go](https://www.metadata2go.com/) to extract the date.
Upload the audio file to that website, then checkout the "Original Date", then you will have your answer!


## [Task 4] Cracking the attack
Topic : Cracking the attack
* Tools: John The Ripper, xxd, QR Decoder

#### How to solve : 
* We'll be using [Sox](http://sox.sourceforge.net/)

* What is the flag?

We will download the QR Code then upload it to [Zxing QR decoder](https://zxing.org/w/decode.jspx)

You will get a github link, download all the files and start cracking!

Open up the terminal, type "zip2john [file.zip] > hash"

The hash file will be automatically saved to your working directory.

Then you'll have to type "john hash --wordlist=/usr/share/wordlists/rockyou.txt

The password of the ZIP will be cracked instantly and will be showen on the Terminal.

Extract the Audio file from the ZIP file, and then type "xxd audio.mp3", you will get Hex values

Go down to the bottom and you will copy the hash code, then you will have to connect them together in a notepad or a text editor.

You will then go to [Base 64 decoder](https://www.base64decode.org/) and decode the hash. Your new hash will be a Base64 as well, so decode it again until you get the flag!

## [Task 5] The End
Topic : End
* Thank you!









