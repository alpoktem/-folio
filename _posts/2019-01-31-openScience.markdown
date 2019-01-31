---
layout: post
title: Compiling the Heroes Corpus
date: 2019-01-31 21:01:00
description: How I used the MdM Open Science Award for my PhD research.
---
(This post originally was posted in the <a href="https://www.upf.edu/web/mdm-dtic/blog/-/blogs/open-science-award-to-alp-oktem-the-heroes-corpus-dataset?_33_redirect=https%3A%2F%2Fwww.upf.edu%2Fweb%2Fmdm-dtic%2Fblog%3Fp_p_id%3D33%26p_p_lifecycle%3D0%26p_p_state%3Dnormal%26p_p_mode%3Dview%26p_p_col_id%3Dcolumn-1%26p_p_col_count%3D1#.XFIlD8_0kWo" target="https://www.upf.edu/web/mdm-dtic/blog/-/blogs/open-science-award-to-alp-oktem-the-heroes-corpus-dataset?_33_redirect=https%3A%2F%2Fwww.upf.edu%2Fweb%2Fmdm-dtic%2Fblog%3Fp_p_id%3D33%26p_p_lifecycle%3D0%26p_p_state%3Dnormal%26p_p_mode%3Dview%26p_p_col_id%3Dcolumn-1%26p_p_col_count%3D1#.XFIlD8_0kWo">DTIC-MdM blog</a>.)

I have used the 2018 MdM Open Science award that I received in the DTIC 6th Doctoral Student Workshop for the collection of a prosodically annotated parallel speech audio dataset called *Heroes Corpus*.

A part of my thesis involves building of a speech translation pipeline to be used in automatic dubbing. I research on the reasons and ways to include prosodic characteristics (intonation, rhythm and stress) of the speakers' and actors' speech into this scenario. Developing such a pipeline requires parallel data, for training the translation model; and speech data since prosody is taken into account.

Speech data production is a highly costly process that involves script preparation, speaker selection, recording and annotation. Due to the inaccessibility of such an approach, I developed a framework to exploit dubbed media material which readily contains parallel and prosodically rich speech. The framework that I call movie2parallelDB provides an automation for this process by taking in audio tracks and subtitles of a movie and outputting aligned voice segments with text and prosody annotation. *Movie2parallelDB* is made available as an open source software in <a href="http://github.com/alpoktem/movie2parallelDB" target="http://github.com/alpoktem/movie2parallelDB">Github</a>.

The framework requires correctly labelled subtitles for both original and dubbed version of the movie. Although this is easy to find in the original language of a movie, it is often not the case in the dubbed language. Practical differences in the dubbing process and subtitling process leads to non-matching audio and transcripts and in turn hinders automatic extraction of the speech data. This means that a manual process needs to be followed to correct subtitles to match the dubbing script.

I decided to use a TV series called Heroes for this work as its Spanish subtitles were close enough to its Spanish dubbing scripts. Timing and transcript corrections were done for 21 episodes by two interns, Sandra Marcos and Laura Gómez. A part of the prize was used to finance their working hours.

The corpus extraction methodology that was developed during the process and the resulting corpus were presented in the <a href="http://hdl.handle.net/10230/35600" target="http://hdl.handle.net/10230/35600">Iberspeech 2018 conference</a>. See the poster below that gives a visual summary of the paper:

<p align="center"><a href="/img/OKTEM-poster1-heroes_med.png"><img src="/img/OKTEM-poster1-heroes_small.png" width="700"></a></p>

The resulting Heroes corpus contains 7000 mapped English and Spanish single speaker speech segments. Audio segments are accompanied with subtitle transcriptions and word-level prosodic/paralinguistic information. It is made openly accessible through the <a href="http://hdl.handle.net/10230/35572" target="http://hdl.handle.net/10230/35572">UPF e-repository</a>.

The rest of the prize was used to fund my final year registration fees and also a tutorial on "Educational dialog systems tutorial" that I attended in Interspeech 2019 in Hyderabad, India.

I am very grateful to have had this boost to my PhD work by the Maria de Maeztu programme and hope that it has further positive repercussions in the speech and translation research community through the resources that were made openly available.