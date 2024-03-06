---
title: Room Automation 
author: Kiddo42069
pubDatetime: 2024-06-03T22:06:31Z
slug: room-automation
featured: false
draft: false
tags:
  - IoT
  - Easy
description:
  Using ESP32 based development boards, we automate various electronics around a room, like locking a door, switching the lights etc.
---

## Door

Will have one esp cam outside the door, triggered by an accelerometer attached to the door on the inside, so need to check viability of deep sleep in the esp cam. 
The esp cam will also alert another esp, or just send telegram notifications itself with photos of the person and a link to a live feed in case the door is opened without a green light by the room owners
Next there would be some kind of servo located near the door lock on the inside, which can be operated by website, app,  or a device created just for that.

## Lights

Powered by induction just to look cool and also prevent loose wires. Automated by an app, website or device. Nothing impressive to be achieved here, unless somehow can integrate WLED to a touch screen system or smth like that. Can also be triggered by a PIR.

## Alarm

Controlled purely by an analog circuit using NE555. Will also add in an esp with deep sleep to send notifications via telegram after a set period of time using voltage trigger