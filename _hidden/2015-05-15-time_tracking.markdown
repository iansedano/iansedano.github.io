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

I implemented a simple priority system using numbers from 1 to 5. We had progress bars to indicate which stage of production the sculpture was in. It was also a place to store technical specifications and other information. I also convinced everyone to use Dropbox and Google Suite.

It was a great success, but at the same time led to many problems.

## Data Entry

I had always assumed that somehow, the work of data entry would be distributed or automated somehow. The spreadsheet was being asked to track too much information for one person to handle. Yet management expected one person to do just that. That person happened to be the Floor Manager, who already had enough on his plate.

I started to see the solution as being computers or tablets distributed around the foundry that were able to quickly update a central database. Yet this suggestion was shot down time and again.

After what seemed like an age of trying to persuade them, the floor manager left his position and the next in line was unable to keep up. So in an effort to make an incremental change towards what I saw as the solution I proposed some time-sheets. Each worker would fill out a piece of paper, by hand, and hand it to an office assistant, who would be tasked with entering it into a spreadsheet.

I spoke with the assistant in private and told them that they were never going to be able to keep up with the flow of data, but to keep the backlog organized in boxes. The boxes piled up and soon I was being asked to investigate subcontractors to implement a solution. They had seen the boxes and understood the magnitude of the data.

## Implementation

I looked at many different proposals for the solution, and in the end I chose one that supported touch screens, bar-code scanning and most importantly, the option to view your data in a spread-sheet, where you can edit values directly from the spread-sheet. Finally, it could export to Excel. I knew that I couldn't rely on any of the admin users to learn a new interface, and this was one that came closest to what they were used to.

Then came long meeting to discuss the specifications of the implementation. I was always clear that what I wanted from the company was a solution to the bounded problem of time-tracking. I needed their help procuring and setting up the server, the database and the touch-screen network. From there, we could develop our own solutions for reporting.

Then management spoke to the salesman, and what was simple, began to get complex. The sales-man had convinced them that their software package was able to achieve everything they wished "out-of-the-box". Something I was sceptical about, but didn't have the experience necessary to fully trust my instinct. I advised against it, but didn't have the language to formulate my argument. We ended up buying various software packages from them, with the promise that they would be able to customize their product towards out needs. I have to admit, once I accepted that route, I got excited about it.

The initial spec I had drawn up was:
* install touch-screens with bar-code scanners.
* install a server and a database.
* create a UI for workers to identify themselves, the piece they were working on, and what they were doing to the piece.
* make the data available for us.


The renewed spec, that only I kept track of was:
* all of the above
* e-mail notifications if a worker had spent 30min inactive
* automatic invoice creation
* repository for all data relating to artwork
* shipping dashboard
* material costs for every sculptures down to the gram
* ...

You get the idea. It was to become the all-singing, all-dancing machine of the future.

It didn't take long for their team to assign me endless data-entry tasks. They asked me to learn their code-base and start defining every single separate part of the sculpture. It wasn't even possible to do it programmatically. I was expected to insert every conceivable part of every sculpture. I started it thinking that I must have something wrong, but quickly it became obvious that their tech-support didn't know what they were doing, and the salesman had become "unavailable". When they told me that I couldn't even copy a 'set' of parts from one sculpture edition to the next, I had had it.

I spend hours on the phone with the technical team deciding how to implement my simplified spec, from which if we needed, we could build on later. Eventually we implemented it and apart from some minor server connection hiccups, which of course, I had to troubleshoot, we started training the staff.

## Conclusion

Since then, it is used everyday, to track hours, piece progress, and for invoicing. Those extra features that we were promised were never delivered. The software obviously has a lot under the hood that we are not using, but for our use case, it has been stable.

I wish I could have developed it more, but soon after I was give a new role and started to develop other things.

