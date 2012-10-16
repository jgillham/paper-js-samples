<h1>Tank Paper.js Arcade Game</h1>

<h2>Contributing</h2>
If you would like to get involved with this project email me at: <a href="mailto:usajoshgillham@gmail.com">usajoshgillham@gmail.com</a>.

<h2>Resources</h2>
Download Git Client: <a ref="windows.github.com">Windows</a>, <a ref="http://mac.github.com">Mac</a>
<br><br>
Check JavaScript code for errors: <a ref="http://www.jslint.com">JSLint</a>
<br><br>
Paper.js:
<a ref="http://paperjs.org/reference">Paper.js Reference</a>, <a ref="http://paperjs.org/tutorials">Paper.js Tutorial</a>
<br><br>
Git:
<a ref="http://git-scm.com/book">Git Book</a>, <a ref="http://gitready.com">Git Reference</a>, <a ref="http://gitfu.wordpress.com">Git Advanced Tricks</a>
<br><br>

<h2>Game project to do list:</h2>
<br>
&nbsp;&nbsp;0. Add firction to the tank, slow down if no movement given.
1. Add bullets to the game (get the tank to shoot stuff)
<br>
&nbsp;&nbsp;2. Add bad guys to shoot at
<br>
&nbsp;&nbsp;3. Make buildings explode or be damaged when hit with a tank bullet
<br>
&nbsp;&nbsp;4. Add status updates in real time (score, kills, deaths, bullets left, ect...)
<br>
&nbsp;&nbsp;5. Add exposion graphic when something is hit with a tank bullet
<br>
&nbsp;&nbsp;6. Add sound effects to the game (moving, shooting, blowing up, ect...)
<br>
&nbsp;&nbsp;7. Add background music to the game
<br><br>

<h2>Detailed Project Outline:</h2>
<h3>&#35;1 I) Create a test to make bullets move acrossed the screen. DONE</h3> 
<h4>&nbsp;&nbsp;a) Create a small test example to show a moving bullet acrossed the canvas. DONE</h4>
&nbsp;&nbsp;&nbsp;&nbsp;i. Create or download an image to use (I am using Gimp).<br>
&nbsp;&nbsp;&nbsp;&nbsp;ii. Embed the image into the HTML file.<br>
&nbsp;&nbsp;&nbsp;&nbsp;iii. Load the image with the Raster class.<br>
&nbsp;&nbsp;&nbsp;&nbsp;iv. Draw the image on the center of the screen.<br>
&nbsp;&nbsp;&nbsp;&nbsp;v. Put code in onFrame() to make the bullet move acrossed the screen.<br>
<h4>&nbsp;&nbsp;b) Copy the test in (a) and modify it with a class to contain the bullet. DONE</h4>
&nbsp;&nbsp;&nbsp;&nbsp;i. Create a constructor that will spawn the bullet at an x and y position, an angle, and a speed.<br>
&nbsp;&nbsp;&nbsp;&nbsp;ii. Create an action in the Bullet class to update the bullet's position called update().<br>
&nbsp;&nbsp;&nbsp;&nbsp;iii. Use update() in onFrame() to show the bullet moving.<br>
&nbsp;&nbsp;&nbsp;&nbsp;NOTE: onFrame() happens every 1/60th of a second. 30 Seconds will be 30 * 60 or 1800 onFrame() events.<br>
<h4>&nbsp;&nbsp;c) Copy (b) and modify it to fire many bullets. DONE</h4>
&nbsp;&nbsp;&nbsp;&nbsp;i. Create an array to hold the bullets.<br>
&nbsp;&nbsp;&nbsp;&nbsp;ii. Add a bullet every second with up to 5 bullets.<br>
<h4>&nbsp;&nbsp;d) Copy (c) and modify it to fire bullets repeatedly every second. DONE</h4>
&nbsp;&nbsp;&nbsp;&nbsp;i. Delete the bullet when it leaves the screen.<br>
&nbsp;&nbsp;&nbsp;&nbsp;ii. Continue spawning bullets with no limits.<br>
<br>

<h3>&#35;1 II) Implement Bullet into the game.</h3>
<h4>&nbsp;&nbsp;e) Reuse the code from (d) to make the take fire the bullet.</h4>
&nbsp;&nbsp;&nbsp;&nbsp;i. All the bullets in the game will be contained in an Array class.<br>
&nbsp;&nbsp;&nbsp;&nbsp;i. The space bar will spawn the bullet.<br>
&nbsp;&nbsp;&nbsp;&nbsp;ii. The onFrame() event will update all the bullets' positions in the array.<br>
<br>

<h3>&#35;2 I) Enemies move randomly.</h3>
<h4>&nbsp;&nbsp;a) Create a test with a raster showing enemy.</h4>
<h4>&nbsp;&nbsp;b) Copy the test and hide the raster inside an Enemy class.</h4>
<h4>&nbsp;&nbsp;c) Copy the test and modify it to randomly move the enemy around the screen.</h4>
<h4>&nbsp;&nbsp;d) Copy the test and modify it to stop the enemy from going off the screen.</h4>
<br>

<h3>&#35;2 II) Enemies moves towards Character</h3>
<h4>&nbsp;&nbsp;e) Copy the test and modify it to move towards a random point on the screen.</h4>
<h4>&nbsp;&nbsp;f) Implement the finished class into tank game.</h4>
<br>

<h3>&#35;4 I) Create an test to show updating feilds along with paper.js.</h3>
<h4>&nbsp;&nbsp;a) Create an example with a text field that increments. DONE</h4>
<h4>&nbsp;&nbsp;b) Create an example of paper.js and the text field together.</h4>

<h3>&#35;4 II) The game updates stats to the HUD.</h3>
<h4>&nbsp;&nbsp;c) Add a text field for each stat we want to display.</h4>
<h4>&nbsp;&nbsp;d) The game should update the fields.</h4>
