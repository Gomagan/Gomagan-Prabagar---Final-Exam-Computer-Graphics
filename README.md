I did the Graphically enhancing packman task.

Hologram:
The hologram shader was added to the ghosts. Each ghost has a different color, but their base shader stays the same. I used shader graph to get the hologram effect. I did this by making an unlit urp shader, and then set the surface type to transparent. I then created a fresnel effect node and then gave in a float value to its power input so I can modify the effect of the rim. I then multiplied the the output with a color. Then I took another output and inverted it using the oneminus node, and then also multiplied that with a color. I then added both and gave them into the base color of the fragment shader. I also took the added output and multiplied it with a float value called transparency and gave the output into the alpha value. This allows me to modify the outer color, inner color, and the transparency of the ghosts. Multiplying the transperency value with the added rim shader values also makes the darker parts of the object more transparent, creating more realistic hologram effect.

Scrolling Texture:
I added the scrolling texture to the orbs. I implemented it by using the tiling and offset node and changing the offset overtime using the time node. I also use a float value called "slow" to modify the rate at which the orbs scroll. You can see the spinning effect from far because of their speed. I also set the surface type to transparent and multiplied the scrolling texture output with a float value so it has a minor transparency effect towards some areas to create more mystical vibe to the game.

For the two additional shaders, I used bump mapping from the first half of the course, and the water shader from the second half of the course.
