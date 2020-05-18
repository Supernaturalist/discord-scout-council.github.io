---
title: "Announcing Campmaster Constantine"
date: 2020-04-29T22:12:20-05:00
categories:
  - project
---
## Overview
I've been on Discord for five years now, and I've been developing bots for it since at least 2016. In that time I've really had two major bot projects, namely the OtmasBot and Kronos. Both of those were implemented in Node.JS, and they both had their respective problems. The OtmasBot was a [mess](https://github.com/Muirrum/Kronos/tree/9e4aa458c62493671ea72c98d0ccd01fdeeca117), and sometimes the [token](2https://github.com/Muirrum/Kronos/commit/5c0d1218a70f4cf7f205ae70f7b21ff953d783bc) even got leaked into git as well. Kronos was different. Kronos had a decent command framework (run through [discord.js-commando](https://discord.js.org/#/docs/commando/master/general/welcome)) and commands that (sometimes) worked. The major difficulty I ran into with Kronos was getting the databases to play nicely with my code. There were multiple issues with SQLite and Docker, spread across many different repositories as I tried GitHub, GitLab, and different frameworks like Klasa. None of them worked, and the project lost my interest for a while.

## Camp Quarantine
Enter Camp Quarantine, a new Discord server focused around inclusive international Scouting. As one of the founding staff members, I wanted to provide something to help the server out, and I immediately thought of a bot. At first, I was going to implement it in Node.JS again. Then, I remembered all the difficulties I had last time I tried that, and I remembered that I've been meaning to learn [Rust](https://rust-lang.org) for a while. I know that making a Discord bot is not *exactly* the preferred way to learn a new language, but it worked for Node.JS, why couldn't it work with Rust? I decided on using the [serenity](https://github.com/serenity-rs/serenity) library, which included a "Standard Framework" to make commands easier.

## Sourcehut
Around this time, I discovered [Sourcehut](https://sourcehut.org/). Sourcehut is a simple, JavaScript-free project site that's split up into several different services, like Git, CI, and Todo lists. I decided I'd give Sourcehut a go along with Rust.

## The Outcome
Somehow, this combination of new services, languages, and libraries worked. I've been more productive in the last few weeks than I ever have been before. Campmaster Constantine has grown in functionality faster than either Kronos or the OtmasBot, and the code is cleaner and faster. My databases "just work". I've finally figured out how to make Continuous Deployment work properly, and I've learned so much about Rust and Git.

For all software developers, I'd *highly* recommened both Rust and Sourcehut. They're both incredibly powerful and useful tools. As for the Campmaster, he's available to [join](https://discordapp.com/api/oauth2/authorize?client_id=702632205062635607&permissions=26630&scope=bot) your Discord servers and start working today! You can read more about him [here](https://hub.sr.ht/~muirrum/Campmaster-Constantine/).