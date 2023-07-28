---
layout: post
title:  "GPT'ing a YouTube Scraper into existence"
date:   2023-04-28
categories: gpt code-project
---

Working on building a Youtube scraper for some freelance work. I want to scrape all of the videos from my client's Youtube channel, and transcribe them into text, so that I can repurpose some of that content for marketing emails and blog content for him.

I'm using GPT4 to build this, just going back and forth with the chat prompt on the OpenAI site. ChatGPT has given my a Python script, which uses the Youtube Data API, and the Google Cloud Speech-to-Text API.

Still doesn't quite work yet, but I never would've been able to do this without GPT. I don't think I would've gotten past connecting the APIs. That's about where I would've given up in the past.

What I've learned so far:

- The 'youtube-dl' Python package sucks for this particular thing–'yt-dlp' is the way to go. I'm also using Bing Chat in creative mode(same as GPT4, supposedly), and ChatGPT and Bing are unanimous on this.
- 'yt-dlp' requires ffmpeg. Took 5 minutes or so to install. I like ffmpeg, it reminds me of Sam Lavigne's [Videogrep experiments](https://lav.io/notes/videogrep-tutorial/)
