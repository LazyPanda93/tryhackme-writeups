# OhSINT Write-up 

## 🧠 Overview

This room is an introduction to Open Source Intelligence (OSINT), where the goal is to gather information using publicly available sources.
In this challenge, I was given an image and had to analyze it to find clues about a person. By following these clues and searching online, I was able to uncover information such as usernames, social media accounts, and eventually the password.
This room helped me understand how small pieces of information can be connected to build a bigger picture.

## 🔍 Step 1 - Image Analysis

I started by downloading the image provided in the challenge and analyzing it, since images often contain hidden information in their metadata.

To extract this information, I used the tool `exiftool`, which allows you to view metadata stored inside files.

Command used: exiftool WindowsXP_1551719014755.jpg
![Exiftool Output](screenshots/outcome_exiftool.png)
