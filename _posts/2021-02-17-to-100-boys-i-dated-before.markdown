---
title: To 100 Boys I Dated Before
date: 2021-02-17 15:51:00 -05:00
layout: post
---

From [zeyaoli.com](http://zeyaoli.com)

## About
I started this project right after I ended my last long-term relationship. I was back on dating apps and had the familiar experience of swiping people, then got bored with it. I wondered how everyone could impress people with their profiles but had weird or boring conversations after getting matched. So we decided to do a project related to this experience and make fun of it with machine learning.

'To 100 (non-existed) Boys I've Dated Before' is a tinder clone that contains 100 profiles that are machine-learning generated, including the profile pictures and the bio. The user can swipe left or right on the website. If swiping right, there is a pop-up window that tells the bizarre dating story we had. The story is based on the training data and generated from context-free grammar.

The project process contains three parts: data collection, data training, and front-end development. It is a collaborative project with Tianxu Zhou.

## Data Collection
- Profile photos are from StyleGan2 for the FFHQ dataset, one of NVIDIA Research Projects.
Names are aggregated from the social security administration.
- Dating Bio is trained from Ok-Cupid profiles datasets from Kaggle, where contains around 60k users' dating profile information. From the open-ended questions, we picked the three most related ones, bio, fun fact, and "what are you looking for."
- Dating stories are trained from the 'what are you looking for' and fun fact categories of the Ok-Cupid profiles dataset. We put the training result into Tracey, a context-free grammar, and generated the story with particular grammar.