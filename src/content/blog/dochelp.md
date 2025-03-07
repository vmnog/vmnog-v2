---
title: "building dochelp.ai"
description: "life as a solo founder/cto"
icon: "3"
pubDate: "Feb 10 2025"
heroImage: "/src/assets/adriana.jpg"
---

hey there! thought i'd share a bit about what it's like wearing all the hats as the founder and cto of dochelp.ai.

## dochelp.ai

imagine a chatgpt but for doctors. we basically connect gpt models with some medical pdfs so the AI can answer correctly and more precisely.

**current frontend stack**:

- next.js
- tailwindcss
- shadcn/ui

**current backend stack**:

- node.js
- fastify
- drizzle orm
- postgresql
- vitest
- openai
- langchain
- upstash vector store

**infra**:

- vercel for frontend deploy
- railway for backend deploy
- github with ci/cd actions
- resend for sending messages

### where we're at?

- **2023/jan (first idea): anamnese ai generator**
  - this idea came as a freelance project for me, i delivered but the client didn't go forward with the app
- **2024/jan (pivot idea): chatgpt for doctors mvp 1**
  - i showed the custom gpt assitant that you can create and upload some pdf's for this old client
  - we talked about creating an mvp and trying to get people to use it
  - created an instagram profile and got about 300 subscribers into a online form
  - put them into a whatsapp group
  - developed the mvp within 2 days, this app version consisted of:
    - one single page next.js app
    - one text input only fixed at the bottom
    - user send message would connect to langchain
    - langchain would consult upstash vector store database
    - using langchain rag to keep context consistent
    - if user refresh pages it would reset the chat messages
    - user could not access previous chats
    - user could only send messages after login with a OTP code
    - stored everything on mongodb, next.js only project, very simple
    - user could send feedback
  - we let users using the app for 7 days for free and we got a lot of feedback
  - from about 300 form subscribers we got about 70 of them to register to the app
  - most of users only send one message and never came back
  - some of them uses everyday from morning to night
  - we offered a stripe subscription for 20$ at the end of 7 days but got no sales
- **2024/jul (first robust version): dochelp.ai**
  - after the mvp test we got some insights
  - also decided to go into this as a co-founder partner
  - the team now was me (tech), marcio (doctor and main financer) and marcos (marketing and audio-visual)
  - i started developing this new version with one goal in mind: build a more robust, pretty and sellable version
- **2025/feb: we launched!**
  - i finally finished the app new version
  - we started to produce instagram ads again
  - with organic and free traffic we could get 100 users to subscribe
  - most of users don't use the app enough, most of them only send a test message and never come back
  - we noticed that maybe our target clients will only come with paid traffic
  - (on going) started planning sales workflow to focus on get some revenue

> dochelp live website: [https://dochelp.ai](https://dochelp.ai)

## wrapping up

if you're thinking about going solo as a technical founder, here's my advice: embrace the chaos, keep learning, and don't forget to take breaks (something i'm still working on!). it's a wild ride, but i wouldn't have it any other way.

catch you later!

p.s. if you're curious about what we're building at dochelp.ai or want to chat about the solo founder life, drop me a line. always happy to connect with fellow tech enthusiasts!
<br /><br />(my socials are at the footer)
