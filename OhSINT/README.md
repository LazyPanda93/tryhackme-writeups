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

## 🔎 Step 2 - Username Investigation

From the metadata, I noticed a copyright name: **OWoodflint**, which looked like a possible username.
I started by searching it on Google to see if anything would come up. Very quickly, I found both an X (Twitter) account and a GitHub profile with the same name.

I opened the X account first, and it immediately helped me answer the first question of the challenge: the user’s avatar is a cat.
While exploring the profile, I also found another useful piece of information. The user mentioned having free WiFi and shared a BSSID.

![X Profile](screenshots/Owoodflint_X_Account.png)

I used a website like **wigle.net** to search for this BSSID. By doing an advanced search, I was able to find its location in London, and also discovered that the SSID was **UnileverWiFi**.

![Wigle Result](screenshots/advance_wigle_BSSID_SSID.png)

With this, I was able to answer two questions and move on to the next one: finding the user’s email address.
