I did the Graphically enhancing packman task.

Hologram:
The hologram shader was added to the ghosts. Each ghost has a different color, but their base shader stays the same. I used shader graph to get the hologram effect. I did this by making an unlit urp shader, and then set the surface type to transparent. I then created a fresnel effect node and then gave in a float value to its power input so I can modify the effect of the rim. I then multiplied the output with a color. This color value is changable so each ghosts can have a different color. I also gave the output into the alpha value of the fragment shader so the dark parts can be transparent so it creates a glowing hologram effect.

