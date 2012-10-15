<br>

Paper.js Resources:
<br>
<a ref="http://paperjs.org/reference">Paper.js</a>
<br>

Git Resources:
<br>
<a ref="http://git-scm.com/book">Git Book</a>, <a ref="http://gitready.com">Git Reference</a>, <a ref="http://gitfu.wordpress.com">Git Advanced Tricks</a>
<br>

Game project to do list:
<br>
0. Add firction to the tank, slow down if no movement given.
<br>
1. Add bullets to the game (get the tank to shoot stuff)
<br>
2. Add bad guys to shoot at
<br>
3. Make buildings explode or be damaged when hit with a tank bullet
<br>
4. Add status updates in real time (score, kills, deaths, bullets left, ect...)
<br>
5. Add exposion graphic when something is hit with a tank bullet
<br>
6. Add sound effects to the game (moving, shooting, blowing up, ect...)
<br>
7. Add background music to the game
<br>
#1 I) Create a test to make bullets move acrossed the screen. 
<br>
  a) Create a small test example to show a moving bullet acrossed the canvas.
    i. Create or download an image to use (I am using Gimp).
    ii. Embed the image into the HTML file.
    iii. Load the image with the Raster class.
    iv. Draw the image on the center of the screen.
    v. Put code in onFrame() to make the bullet move acrossed the screen.
<br>
  b) Copy the test in (a) and modify it with a class to contain the bullet.
    i. Create a constructor that will spawn the bullet at an x and y position, an angle, and a speed.
    ii. Create an action in the Bullet class to update the bullet's position called update().
    iii. Use update() in onFrame() to show the bullet moving.
  NOTE: onFrame() happens every 1/60th of a second. 30 Seconds will be 30 * 60 or 1800 onFrame() events.
<br>
#1 II) Implement Bullet into the game.
<br>
  c) Reuse the class from (b) to make the take fire the bullet.
    i. All the bullets in the game will be contained in an Array class.
    i. The space bar will spawn the bullet.
    ii. The onFrame() event will update all the bullets' positions in the array.
<br>


#2 I) Enemies move randomly
<br>
  a) Create a test with a raster showing enemy.
<br>
  b) Copy the test and hide the raster inside an Enemy class.
<br>
  c) Copy the test and modify it to randomly move the enemy around the screen.
<br>
  d) Copy the test and modify it to stop the enemy from going off the screen.

#2 II) Enemies moves towards Character
<br>
  e) Copy the test and modify it to move towards a random point on the screen.
<br>
  f) Implement the finished class into tank game.
<br>

#4 I) Create an test to show updating feilds along with paper.js.
<br>
  a) Create an example with a text field that increments.
<br>
  b) Create an example of paper.js and the text field together.
<br>

#4 II) The game updates stats to the HUD.
<br>
  c) Add a text field for each stat we want to display.
<br>
  d) The game should update the fields.
<br>
