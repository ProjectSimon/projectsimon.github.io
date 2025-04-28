---
title: "What is Project Simon ?"
keywords: homepage
sidebar: home_sidebar
permalink: index.html
summary: <q>Nan mais ce qui est dingue, c'est, c'est la première fois que j'en vois une, en vraie, une Kineuton!</q> Simon Jérémi, from the funniest French comedy <a href="https://letterboxd.com/film/fear-city-a-family-style-comedy/" target="_blank">La Cité de la peur</a>, eclaimed in front of the Kinoton projector he'd been dreaming of since childhood. Project Simon aims to build a 35 mm film scanner with a Raspberry Pi.
---

{% include note.html content="If you came here expecting to find a fully fonctionnal product, unfortunately it's not finished yet! Hopefully, if you feel so inclined, you can help contribute to one of the many repo listed <a href='https://github.com/orgs/ProjectSimon/repositories' target='_blank'>here</a>" %}

{% include warning.html content="Website under construction" %}

# Project Simon

The **Project Simon** is an open-source film scanner build around affordable DIY / maker friendly stuff as :
* Raspberry Pi computer (model 4 8Go is currently tested, should work with other Pi 4 and Pi 5 models)
* An HQ camera module
* 3D printing pieces

## Why Simon ?

The project name comes from the French comedy <a href="https://letterboxd.com/film/fear-city-a-family-style-comedy/" target="_blank">La Cité de la peur</a> by Alain Barberian and les Nuls, where one of the main character is called Simon Jérémy.

{% include important.html content="What?!? You've not watch the movie yet? Please, stop everything you're doing and come after once you've seen it!" %}

Meanwhile in Vera Cruz... During the Cannes Film Festival, every projectionist of <i>Red is Dead</i>, <a href="https://en.wikipedia.org/wiki/Cult_film#%22So_bad_it's_good%22">a "so bad it's good"</a> slasher, is murdered by a copycat of the movie's killer. Meanwhile a investigation is lead, we follow Odile Deray, <i>Red is Dead</i> publicist, Simon Jérémy, its intellectually disabled movie star and Serge Karamazov, their bodyguard and self-proclaimed womanizer.

In one scene, Simon reveals that he had always wanted to be a projectionist, against his father's wishes to make him an actor. Thus giving his name to this project. But, it can also stand for <i><b>S</b>canner d'<b>I</b>mages <b>M</b>ouvantes d'<b>O</b>rigine <b>N</b>on-numérique</i> [^1] in the language of Molière.

## Software

### libcamera

Quoting [`libcamera`](https://libcamera.org/) documentation, libcamera is <i>a complex camera support library for Linux, Android and ChromeOS.</i>

Project Simon uses its own [fork](https://github.com/ProjectSimon/libcamera) of Raspberry Pi's libcamera repository to be able to manage other camera sensor as [`IMX294`](https://www.willwhang.dev/OneInchEye/) sensor made by [Will Whang](https://www.willwhang.dev/). More sensors may come if I'm able to buy some.

### rpicam-apps

This part is related to libcamera-based applications to configure the cameras on a Raspberry Pi board. The whole Project Simon camera configuration application will be based on this [repository](https://github.com/ProjectSimon/rpicam-apps).

## Hardware

For now, it's only been tested on a [Raspberry Pi 4](https://www.raspberrypi.com/products/raspberry-pi-4-model-b/), with an [official HQ camera v1.0](https://www.raspberrypi.com/products/raspberry-pi-high-quality-camera/).

It should work with any newer boards and official cameras.

# Footnotes
[^1]: <b>M</b>oving <b>I</b>mage <b>S</b>canner of <b>N</b>on-digital <b>O</b>rigin : English translation of the project acronym. But we lose the word play.

{% include links.html %}
