---
permalink: /
title: "academicpages is a ready-to-fork GitHub Pages template for academic personal websites"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

This is the front page of a website that is powered by the [academicpages template](https://github.com/academicpages/academicpages.github.io) and hosted on GitHub pages. [GitHub pages](https://pages.github.com) is a free service in which websites are built and hosted from code and data stored in a GitHub repository, automatically updating when a new commit is made to the respository. This template was forked from the [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/) created by Michael Rose, and then extended to support the kinds of content that academics have: publications, talks, teaching, a portfolio, blog posts, and a dynamically-generated CV. You can fork [this repository](https://github.com/academicpages/academicpages.github.io) right now, modify the configuration and markdown files, add your own PDFs and other content, and have your own site for free, with no ads! An older version of this template powers my own personal website at [stuartgeiger.com](http://stuartgeiger.com), which uses [this Github repository](https://github.com/staeiou/staeiou.github.io).

Problem Diagnosis
======
The global Covid-19 pandemic has imposed enormous restrictions on people’s daily life. One of the most noteworthy limitations is the difficulty to gather in a public area for completing essential daily tasks. Among all, college students are a major group inevitably influenced, deprived of the opportunity to participate in various group events such as in-person classes, group discussions, and team projects. As a result, multiple successful solutions, such as Zoom, Webex, etc. arose in the past year aiming to bridge students over physical limitations when studying from home. These solutions offer students the chance to avoid getting infected by the disease and save time on commuting. However, there are also certain deficiencies for these existing platforms: the plain meeting interface lacks the learning atmosphere, and students lose their chance to demonstrate by sketching on whiteboards. A solution is urgently needed to merge the advantages of the in-person campus experience and distanced learning style into one platform/software. 

Proposed Solution
======
In this project, we propose a virtual workspace uniquely built for students bringing spatial presence and immersive experience which cannot be achieved in online meetings and providing a personalized study environment with limitless space which cannot be achieved in real life.

Minimum functionalities
-------
Lobby: After logging into the platform, users will find themselves inside a big lobby where everyone can talk, socialize and explore. There will be two huge portals displayed on the wall, teleporting users to either a private dorm or a public space. The users can use the joystick on the controller to walk to the portal after they decide where to go. 
Personal Room/Dorm:  If users enjoy being alone, they can enter their private dorm room, where they focus on personal work without being distracted. Users will have a toolbar surrounding them where they can choose to spawn tools like a whiteboard in different sizes for sketching thoughts, sticky notes for brainstorming or taking a quick note, or multiple browsers/remote desktop windows from a real personal computer to the virtual dorm space. The most amazing thing is that users can drag and relocate all these tools to wherever they want without any real-world physics limitations.
Public study room: If users enjoy studying with others or need a space for group meetings, they can enter the public study room, where dozens of tables are provided. Users can sit around a table and spawn tools visible either to everyone for discussions, or only to themselves for personal work. Just like in a real study space, users can hear the voice from nearby tables. Users are free to mute others if they prefer a quiet environment or to mute their table to others if they prefer private conversation. Other users can request to join a table/discussion if they want to see the contents of a specific table. In this way, users can control their privacy while experiencing a real study room environment. 

Implementation Plan
------
On the hardware side, we will use Oculus Quest 1 or 2. This is because we already own these devices and Oculus Quest is a competitive product that has various advantages such as affordable prices, no cables required, lightweight, sharp display with high refresh rate, powerful processor, accurate motion tracking capability, and real-time debugging functionality with additional cables. It also has disadvantages such as short battery life. However, short battery life is a common issue to have for all standalone head-mounted display devices, and Oculus stated that it should last for several hours between charges, which is our expected user’s usage time. We also expect the future generations of Oculus devices to have a better battery life due to a rising market in VR/AR.
On the software side, the Oculus website recommends Unreal Engine and Unity3D Game Engine as development platforms. We will be mainly working with Unity Game Engine with C# language, since Unity3D has a built-in library specifically developed for the Oculus application, and it is easier to learn Unity than to learn Unreal Engine.
Since our project requires a multiplayer feature, we will choose Photon PUN as a network solution. Photon is a relatively mature networking product aiming to make the multiplayer development process a lot easier. Additionally, PUN (Photon Unity Networking) is a wrapper for different layers, and it is designed for Unity, which means its documentation is suitable for Unity development. Its wrapper characteristic implies possible customizations for each layer from the low level of protocols, mid-layer of callbacks and working with Photon servers, and high level of Unity-specific features such as Unity object’s add-on and RPC calls, etc.
With the help from the above 3 tools, we should be able to achieve the minimum functionalities that we promised. We may use other tools to develop the possible additional functionalities in the future.

Possible Stretch Goal
------
Friend/contact system: Users can add anyone they meet either in any study area or social event to their friends’ list and a message system will be provided for communications. Users can invite friends to private dorm rooms for shared work or recreation experiences.
Reward points and customizable elements: Users will be given reward points according to their time spent studying in our system. The reward points can be used to redeem virtual room decorations and apparel. The room can be set up in whatever way the user/event host wants it to be to guarantee an experience with the highest degree of freedom, immersiveness, and creativity.
Speech room: There will be a speech room for users to host speech events, practice presentations, or have classes. 
Entertainments: There are also entertainments offered on our platform if users feel tired of studying. The planned entertainments contain movie theatres and game centres. The users will need to consume their rewarded points to enjoy entertainment activities.
Social event system: If users want to make new friends, or participate in others’ academic activities, there will be a social event system posting all the social events that are happening on the virtual campus. They can see a list of ongoing or upcoming social events with different topics along with related details. Social events will contain movie nights, public speeches, academic discussions, and networking events.

Market Analysis
======
Our product is intended to be used by college students who suffer restrictions on attending a physical campus for group studying or those who tend to try a new mode of studying in VR that fuses multiple virtual but interactive elements. Students will have a few options: they can either study in an enclosed, individual and customizable room to avoid distractions; or they can gather with groups in a public study lounge for discussion and teamwork. There are more attractive functionalities such as friend/social system, entertainment, and speech events to be developed on the platform.

Commercial Product Analysis
======
Immersed [1][2] is an example of VR platforms that offer an immersive virtual working experience. It has two distinct modes: solo and collaboration. In solo mode, the user works in a private workspace that eliminates distractions and supports up to 5 virtual monitors. This feature enables the user to largely enhance productivity without investing in additional hardware such as physical monitors. In the collaboration mode, more than 4 people can join the user’s room for synchronous collaboration. In this room, users can share multiple screens and access a shared whiteboard.

vSpatial [3][4] is another example of VR workspace products. It offers a shared workspace for all co-workers. It has full integration with Slack workspace so that all the channels and contacts are available during working. It can access all the programs running on the computer and share them within the virtual workspace. There is spatial audio integrated into the meeting environment, which makes all users feel like in a physical room.

Compared to the state-of-the-art products listed above, our solution focuses more on building a study environment for students and teachers. For example, besides the personal study room which is similar to that in Immersed, we proposed the public study room to create a real-life study atmosphere to help students focus on their work. Moreover, we proposed the speech room to give both the teachers and students an in-person course experience, which is missing from the products listed above. In the speech room, students can whisper with one another, teachers can stand by a podium and see students raising their hands. Thus, although there are already several competitors and mature products in the market, our product still stands out with its unique functions and specifically targeted customers. 

Component Diagram
======

OSS Components Used
======
Meta Avatars SDK
a.Using the Meta Avatars SDK, users can create their own appearances to increase social presence and enhance VR immersion.
b.Link: https://developer.oculus.com/documentation/unity/meta-avatars-overview/
Unity Asset Store
a.Asset Store provides various premade assets such as texture and objects to fit our needs when building the scene.
b.Link: https://assetstore.unity.com/

Related Sources
======
1. https://immersed.com/
2. https://www.xrtoday.com/virtual-reality/immersedvr-review/
3. https://www.vspatial.com/
4. https://ryanschultz.com/2019/08/13/vspatial-a-brief-introduction-yet-another-remote-workteams-vr-platform/
