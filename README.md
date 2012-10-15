GOAL: To provide samples with paperscript.

Paper.js Resources:
<a ref="http://paperjs.org/reference">Paper.js</a>

Git Resources:
<a ref="http://git-scm.com/book">Git Book</a>
<a ref="http://gitready.com">Git Reference</a>
<a ref="http://gitfu.wordpress.com">Git Advanced Tricks</a>

Game project to do list:
0. Add firction to the tank, slow down if no movement given.
1. Add bullets to the game (get the tank to shoot stuff)
2. Add bad guys to shoot at
3. Make buildings explode or be damaged when hit with a tank bullet
4. Add status updates in real time (score, kills, deaths, bullets left, ect...)
5. Add exposion graphic when something is hit with a tank bullet
6. Add sound effects to the game (moving, shooting, blowing up, ect...)
7. Add background music to the game
<br>
#1 Tank fires bullets:
<br>
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
  d) The tank will fire bullets (resuse code from (a) through (c) ).
    i. The space bar will spawn the bullet.
    ii. The onFrame() event will update the bullet's position.
    iii. Each building will check the bullet to see if it is inside.
    iv. When the building is hit its image will be changed to a broken building.

#2 Enemies pursue character
  a) Spawn an enemy.
  b) Create an Enemy class.
  c) Move the enemy randomly around the screen.
  d) Add collision detection.
  e) Enemies move towards character.
  f) Enemies have stop advancing towards character at a distance.

#4 Add status updates in real time (score, kills, deaths, bullets left, ect...)
  GOAL: Game HUD.
  a) Create an example with a text field that increments.
  b) Create an example of paper.js and the text field together.
  c) Add a text field for each stat we want to display.
  d) Integrate with the game.

