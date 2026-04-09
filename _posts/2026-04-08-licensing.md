---
layout: post
title: "TGFOE 2026: The Licensing Rabbit Hole"
---

# Introduction
It's been 2 months, and a lot has changed. I last wrote about my efforts to switch to free and open source software (FOSS) in general. I still believe in that idea, but I've found meaning within it. For the last month or so, I've been working on the switch to a freer, more permissively licensed ecosystem.

# Open Source is a Big Umbrella
This was the turning point for me. Years ago, when I had first installed Linux I thought open source simply meant the availability of the source code; little did I know how far I was from the truth. The variety of open source licences was never a concern to me, and simply being open was enough for me.

Recently, I decided to put more thought into my values. I knew that software being free as in freedom was important. The nature of copyleft licences seemed to be in alignment, but proved to be a misconception. Forcing users to provide the source code for their modifications, which is their own work is a restriction in itself, even if it is done for the sake of preserving freedom. True software freedom is unconditional, and should permit anyone to do as they please with the software. The original work will always be open regardless of proprietary derivatives. 

# Permissive, Eh? Why Not Public Domain? 
With my logic, it only makes sense I prefer and advocate for the public domain. While I do see the public domain as theoretically the freest, the recognition of a public domain dedication varies by jurisdiction. This makes it a more reliable option to license software permissively under either the ISC or BSD licences, with no restrictions beyond attribution. The ISC license is my licence of choice whenever possible, as it provides essential freedoms with minimal text.

Check out the ISC licence [here](https://choosealicense.com/licenses/isc/). This website was recently re-licensed to it (see more below)!

The ISC licence is great, but is fairly uncommon in comparison to other permissive licences. I personally use [Copyfree](https://copyfree.org/)'s [licence list](https://copyfree.org/standard/licenses) to determine a licence's credibility. The Apache 2.0 licence, which is commonly considered to be permissive is excluded from this list due to its patent clause. 

# Practising What I Preach
With the base of this article being introduced, I made the switch with my own software.
* My [dotfiles](https://codeberg.org/charged/Dotfiles)
    * MIT --> Unlicense
    * I do not have any interest in preserving my dotfiles in any way, so I dedicated it to the public domain and never looked back.
* This website!
    * MIT --> ISC
    * Simply a removal of unnecessary wording, the freedoms remain the same.
* [`cysinfo`](https://codeberg.org/charged/cysinfo) - A super simple and minimal fetch tool for Linux. 
    * GPL v3 --> ISC
    * This is the biggest shift for me. I first created `cysinfo` in 2022, when I was fairly new to the open source space. I did not look into the licensing of it and simply picked what I believed to be the most popular open source licence. The recent C rewrite I did brings in a new licence too!

# The Progress Toward a Permissive Ecosystem
Besides just licensing my own software, I wanted to try and switch the software I use to this model, similar to my last article. The most significant piece of software I rely on daily is my operating system. I've been using NixOS comfortably for roughly 6 months now, and I've been satisfied with how it's holding up. OpenBSD has been on my mind however, for its [ideological similarity](https://www.openbsd.org/policy.html) to Copyfree as well as being a nice challenge for me to adapt to. 

## The Server OS
This was the first wave of the switch to OpenBSD. I plan to switch my Elitebook 2560p from Debian 13 to OpenBSD, and will report back on the ups and downs in a dedicated OpenBSD article I may write in the future. If all goes well, it could serve as the server hosting this site!

## The Desktop Plans...
This is a tough hurdle to get over. My desktop PC is physically incapable of connecting to WiFi on OpenBSD as far as I know. I recently bought a used Lenovo ThinkPad T480, which is much more popular for OpenBSD. Right now I'm just testing the waters with my home server, and when the summer rolls around, I'll give the graphical experience a go. If the ThinkPad project is successful, I'll consider finding a workaround for the my desktop. 

I've currently been working toward this, I've been configuring some suckless utilities as well as other permissively licensed applications to easily integrate myself into OpenBSD when the time comes. Here's what I've been working on:
* [dwm](https://codeberg.org/charged/dwm) - updating is probably my only concern here. Felt weird to be back on X11.
* [st](https://codeberg.org/charged/st)
* [dmenu](https://codeberg.org/charged/dmenu)
* [freedots](https://codeberg.org/charged/freedots) - no permissive nerd fonts really existed, so I took the MIT licensed Agave and patched it with permissively licensed icons :)
* Kakoune - coming soon, I'm too comfortable on Neovim.

![dwm scrot](https://codeberg.org/charged/dwm/media/branch/personal/scrot.png)
Pictured above: My minimal dwm rice.

## Social Media
Looking past the OS, I spend a lot of time on social media. Since the last post, I've gotten rid of Instagram and ChatGPT (well, I switched to Claude), which is a step in the right direction. I've also slowed down on the Fediverse and shifted toward Bluesky. While not as federated and open in practice, its clients are permissively licensed meaning I avoid copyleft applications on my phone, unlike most Mastodon clients which are GPL licensed. The user base is also more diverse, with more topics being discussed besides software and technology.

![bsky scrot](/images/2026-04-08-licensing/bsky.png)
Pictured above: [My Bluesky profile](https://bsky.app/profile/charged1.ca). Don't look at the follower count.

# Conclusion
This journey hasn't been perfect. There's some software I've had to avoid completely or deal with the copyleft/proprietary remnant. An example of this is the web browser, with most engines being copyleft or proprietary. [Ladybird](https://ladybird.org/) is an interesting project which aims to solve this problem, something which I'll be keeping my eyes on.

It all comes down to practicality in the end: As I've said before: I'm not trying to be a purist, I'm simply updating the software in my life to be more consistent with my views on free software.
