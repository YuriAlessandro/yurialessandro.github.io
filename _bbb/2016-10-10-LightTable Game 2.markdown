---
layout: default
post-id: 3
autores: Yuri Alessandro Martins e Pedro Arthur Fernandes
video: <iframe width="560" height="315" src="https://www.youtube.com/embed/7tozcF_-gu4" frameborder="0" allowfullscreen></iframe>
date: 2016-10-10
project-date: Outubro 2016
category: C++
description: A simple game using BBB's utensils and fork function.
repo: https://github.com/YuriAlessandro/LightTableGame2
---
# Table Light Game v2#
This is almost the same thing the previous version.
However it has an interesting extra: the player should be able to guess the number within one minute.

Below you can remember how the first version works - but remember, you have only one minute.

# The Code #
For this version we use the function "fork" of C ++. With it, we created two processes (a father and son) that run at the same time.

The child process has the responsibility to run the entire game - it continues being basically the same thing the previous version. This is where all logics and testings will occur to ensure that the user can play.

The parent process is over to "pass the time". In it, we use an "alarm" signal to determine when pass 60 seconds since the program being run, it calls a function that indicates the user that the time is up and, because of that, he lost the game.

# How Works #
This is a simple game of luck. Using the potentiometer, the player must choose a number in a range that is determined by the photoresist. The game will pick a random number from the same range and the goal is to find the number. 

If there is little light, so the game will be easy. Otherwise, the game will become more complicated.

But that version 2 has an additional interesting: the player should be able to guess the number within one minute.

After choosing a position potentiometer (which will be your number), the player must press the button to register your bid. The number that corresponds to what you have determined the potentiometer will be displayed on your computer screen.

If the player passes by, a blue light will appear, indicating that the attempt is near the random number for the game, and the player loses 5 points (from a total of 100 initial).

However, if the attempt is far away, a red light will illuminate. In this case, the player loses 2 points.

When hit the random number, a light will illuminate and the final score of the player will be shown on screen. Every attempt, the player is able to see what your score and what was his last attempt, If you reach 0 points, he loses.


``` 
