---
layout: post
title:  Time-tracking in a Foundry
date: 2015-05-15
description: Implementing a time-tracking solution
---

This is a write-up of my multi-year project that culminated in a time-tracking software and hardware solution.


## The Foundry

See article - The Lost Wax Method.

When I first visited the foundry, only the General Administrator had a computer. The "lost-wax" method of making sculptures has its origins possibly 6000 years ago, and is still in use today, largely unchanged. So it was not surprising that the foundry had no need for advanced technology. As it turned out, most were technologically averse.

With the 2008 financial crisis unfolding in the background, this foundry had secured a partnership with a prominent artist, who had in turn secured a contract with a famous gallery. While businesses were closing, operations in the foundry were ramping up. The first order of business was establishing some lines of communication between the needs of the gallery, the constraints of the artist and the abilities of the foundry.

In the world of the gallery, e-mail and spreadsheets were ubiquitous. They would send through "London-style" messages, asking the impossible, the ridiculous, but at least they did so with some aloof politeness and a spreadsheet attached. The owner of the foundry would read a print out of the e-mail and become incensed. He couldn't believe how brash they were, and how much they asked for.

What he didn't know was that the message from the gallery should have been read as a wish-list and not a demand. I can't blame him for not realizing this. The e-mail was full of words like: "must be", "asap", "no delay" and "deadline". What they needed in response was - "Ok, we'll do out best and keep you informed of our progress." Instead, he would respond: "Impossible!", or just ignore them.

Stereotypes are real only in the sense that people rely on them, and in most cases, are just negative oversimplifications. The foundry came to look upon the gallery as arrogant and the gallery came to look upon the foundry as lazy. We stepped in and started to mediate the conversation as soon as possible.

## Spreadsheets

These became our bread and butter. The gallery, as the sole client, wanted numbers, dates and progress reports. Each sculpture had to have a unique edition number, and so we started tracking individual sculptures from order to delivery. At the time there were around 30 artisans working making the sculptures. The number of sculptures that could be simultaneously in production were about 50. Though, depending on the size of the sculptures, only 20 or so could be worked on simultaneously.

I defined a series of steps that the sculpture needed to go through. The simplified version of which was:

* Wax
* Ceramic
* Casting
* Chiselling / Sandblasting
* Mounting
* Finishing
* Crating

I implemented a simple priority system using numbers from 1 to 5. We had progress bars to indicate which stage of production the sculpture was in. It was also a place to store technical specifications and other information.

It was a great success, but at the same time led to many problems.

## Data Entry

I had always assumed that somehow, the work of data entry would be distributed or automated somehow. The spreadsheet was being asked to track too much information for one person to handle. Yet management expected one person to do just that. That person happened to be the Floor Manager, who already had enough on his plate.

After what seemed like an age of trying to convince 







* Developing a way of working with IT from the ground up.
	* A slow start persuading colleagues (many of whom were technologically adverse) by **evangelizing** the benefits and talking one-on-one to understand the resistance.
	* I demonstrated software such as **Dropbox**, **Google Sheets**, **Google Docs**, **SQL**. I demonstrated what was possible with simple scripts in **VBA** or **Python**.
	* I **piloted** solutions (out of my own pocket) from adopting Dropbox, to paying developers to consult with and explore options such as **Ruby on Rails**, **Access**, **Django**.
	* **Incremented** progress slowly by **introducing** behaviours and technologies that lead to the final solution.
	* Eventually implementing a **server**, **database** and touch-screen and bar-code **interface** in the factory which has been in use now for 5 years.
