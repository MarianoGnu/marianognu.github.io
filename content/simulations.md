+++
date = '2026-01-11T19:57:43-03:00'
draft = false
title = 'Simulations'
+++

In the past i have worked integrating several simulation libraries to diffrent environments.
Here is a list of my work.

<!--more-->

## MSEP.one The Molecular Systems and Engineering Platform

As one of the main developpers of [MSEP.one](https://msep.one), i have implemented the modeling, construction, and simulation of arbitrary molecule systems.
From loading molecules from libraries, to generating DNA chains from it's sequence, and then simulating them using the OpenFF and OpenMM backends.

{{< rawhtml >}}
<video width="100%" controls>
  <source src="https://msep.one/wp-content/uploads/2024/11/bearing.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>
{{< /rawhtml >}}

This was possible by creating a connection between the frontend application, made with [Godot Engine](https://godotengine.org/), and a process running in python that takes the input of the system, process the simulation, and returns the new positions of particles frame by frame.

This communication was possible thanks to the integration of [zeromq](https://zeromq.org/) library to the Godot Engine, [also of my authory](https://github.com/MSEP-one/msep.one/tree/main/modules/zeromq)
