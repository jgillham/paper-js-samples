GOAL: To provide samples with paperscript.

Resources:
http://git-scm.com/book
http://paperjs.org/reference/


Game project to do list:
0. Add firction to the tank, slow down if no movement given.
1. Add bullets to the game (get the tank to shoot stuff)
  GOAL: THE TANK WILL DESTROY BUILDINGS AND EVENTUALLY ENEMIES.
  a) Create a small test example to show a moving bullet acrossed the canvas.
    i. Create or download an image to use (I am using Gimp).
    ii. Embed the image into the HTML file.
    iii. Load the image with the Raster class.
    iv. Draw the image on the center of the screen.
    v. Use onFrame() to show the bullet moving over time acrossed the canvas.
    vi. Delete the bullet when it leaves the screen.
  b) Create a copy of example (a) that will use collision detection.
    i. Spawn a building in the direction that bullet will travel.
    ii. Test the bullets front tip to see if its inside the building.
    iii. Display a peice of HTML text when the bullet has entered the building.
    iv. Delete the bullet.
  c) The tank will fire bullets.
//TODO finish part c.
2. Add bad guys to shoot at
3. Make buildings explode or be damaged when hit with a tank bullet
4. Add status updates in real time (score, kills, deaths, bullets left, ect...)
5. Add exposion graphic when something is hit with a tank bullet
6. Add sound effects to the game (moving, shooting, blowing up, ect...)
7. Add background music to the game

Detailed Steps to finish todo #1:
  GOAL: THE TANK WILL DESTROY BUILDINGS AND EVENTUALLY ENEMIES.
  a) Create a small test example to show a moving bullet acrossed the canvas.
    i. Create or download an image to use (I am using Gimp).
    ii. Embed the image into the HTML file.
    iii. Load the image with the Raster class.
    iv. Draw the image on the center of the screen.
  b) Create a Bullet class to contain the Raster from (a).
    i. Create a constructor that will spawn the bullet at an x and y position and a speed.
    ii. Create an action in the Bullet class to update the bullet's position.
    iii. Call <Bullet>.update() in onFrame() to show the bullet moving.
    iv. Delete the bullet after 30 secs.
  NOTE: onFrame() happens every 1/60th of a second. 30 Seconds will be 30 * 60 or 1800 onFrame() events.
  c) Create a copy of example (a) that will use collision detection.
    i. Spawn a building in the direction that bullet will travel.
    ii. Test the bullets front tip to see if its inside the building.
  NOTE: Use the contains method inside the Block.
    iii. Display a peice of HTML text when the bullet has entered the building.
    iv. Delete the bullet.
  d) The tank will fire bullets (resuse code from (a) through (c) ).
    i. The space bar will spawn the bullet.
    ii. The onFrame() event will update the bullet's position.
    iii. Each building will check the bullet to see if it is inside.
    iv. When the building is hit its image will be changed to a broken building.
