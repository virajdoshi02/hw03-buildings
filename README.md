# CIS 5660 HW03 Procedural Buildings

If you wanted to make a house inside a hurricane, how would you make sure it doesn't get damaged by the wind? You would have it rotate with the hurricane! 

For this project, I started by following the tutorial. However, in the middle I had a different idea. I replaced my regular loop with a triple nested loop, and changed the blocks so that I could create an inverted pyramid of rooms. The height h has h^2 rooms, each with its own doors, windows etc. The outermost loop loops over the height, the second one connects vertical segments together, and the innermost loop creates vertical segments of rooms, each length h (with h such segments, we get h^2 rooms). I changed the VEX code to remove the balcony from the bottom, to stop balconies from intersecting with other balconies and large windows I limited the number of each on each side of each room using VEX, I used a weighted random distribution to distribute more windows and fewer doors. The angle of the supports varies with the distance, and the closest and farthest ones have a higher angle than the others. I also modelled all of these assets in houdini and saved them in files. After putting the houses together in a pyramid, I added a random bevel to add wear and tear (from the hurricane), I added colour to the house, and then added a rotation animation using VEX to make it rotate. I also added a terrain with random colour (using some terrain noise and VEX) and an environment map for a skybox.

Renders:
![image](https://github.com/user-attachments/assets/2d368466-8783-4ece-8643-cd613adcb913)
![image](https://github.com/user-attachments/assets/aaae2fd9-a3f9-41e4-ada6-db047db516b8)
![image](https://github.com/user-attachments/assets/ece9cced-c406-45ed-a316-4d6ee933539c)
![image](https://github.com/user-attachments/assets/7a5952d6-9e1a-401e-b667-a466d7797e03)

Video:
https://github.com/virajdoshi02/hw03-buildings/blob/main/Recording.mp4
