---
title: "Schrödinger's Cat 2"
date: 2024-04-24 21:08:00 +0800
image: /assets/images/blog2/challenge-preview.jpg
categories: [Schrödinger's Cat 2]
tags: [Schrödinger's Cat 2, Writeup, CTF, Blog]
---

# Schrödinger's Cat 2

![Challenge Details](/assets/images/blog2/challenge.png)

One of my favorite CTF challenges in SKRCTF and I am so happy that I could solve this fun challenge. Before that, I suggest you to do Schrödinger's Cat 1 first to get an idea of this 2nd challenge and my solution.

Challenge Link: https://skrctf.me/challenges#Schr%C3%B6dinger's%20Cat

How do I find out the answer/flag? It is actually simple but quite a lengthy process. I will try my best to explain it in detail.

At the beginning, I just play around this guessing game by entering 1 or 2 as you can see in the terminal screenshot below.

Of course, initially I thought it is randomized until I restarted the game and tried countless times like a noob. Only to realize it is a fixed question and answer with that specific pattern. And I also realized that since the result is either 1 or 2 (alive or dead) can be interpreted as true or false in boolean and binary. So I come up with this idea 0 for Wrong (Dead) and 1 for Right (Alive)

From that information, we can find out SKR in binary format which are 01010011 01001011 01010010 01111011 01111101.

![Challenge Details](/assets/images/blog2/image1.png)

Using the information and same idea to find the right answer from the correct answer (from the bot) and you will get something like what I did.

![Challenge Details](/assets/images/blog2/image2.png)

![Challenge Details](/assets/images/blog2/image3.png)

Doing of all that, you just need to convert the binary to ASCII and you will get the flag. 



### Flag: SKR{R1gh7_or_Wr0nG}