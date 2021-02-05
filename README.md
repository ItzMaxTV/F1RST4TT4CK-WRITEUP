# F1rst-4tt4ck Write Up
A beginner-level CTF challenge as one of the [TryHackMe room](tryhackme.com/jr/f4), which focus on Stenography, Cracking, and processing audio files.

## Authors 
* [ItzMaxYT](https://tryhackme.com/p/ItzMaxYT)
* [CrUsHiNg](https://tryhackme.com/p/CrUsHiNg)

## [Task 1] Intro
Topic : Intro
* Intro to the rooom. 
* It shows you the tools we'll be using

## [Task 2] Cracking
Topic : Cracking
* We'll be using John The Ripper to crack the ZIP File.
* It shows you the tools we'll be using

Personally recommend to use [CyberChef](https://gchq.github.io/CyberChef/) as a tool to solve most of the questions here easier.

### #1 Leet/1337/L33T

[Leet](https://simple.wikipedia.org/wiki/Leet) is an alternative alphabet set that general for English language that used mostly on internet. It can also applies on those language that constructed similarly to english alphabet set, eg. German and Spanish

It can be confusing at first, while considering those 'weird' (non-alphabetic) characters and guess with their nearest lower/uppercase alphabet helps a lot in translation. 

#### Cipher : c4n y0u c4p7u23 7h3 f149?

#### How to solve : 
* Translate by using this [tool](http://www.robertecker.com/hp/research/leet-converter.php), or
* By guessing (pretty straight forward here) , ie.
  * 4 > A > a
  * 0 > O > o
  * 7 > T > t
  * 2 > |2 > R > r 
  * 1 > l
  * 9 > g

