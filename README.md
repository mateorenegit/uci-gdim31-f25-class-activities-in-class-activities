# in-class-activities
## Hello world!
### W1
Write your W1 activity Devlog here.
In my version of the game I kept the camera as a child within the Cat model as a First Person POV.
However, if the camera was taken off the cat and put outside of the model, it would stay still and not follow the cat.
The player would still be able to view the cat, just not follow it. 
https://whatnotpebble.itch.io/w1

### W2
Create future Devlog sub-headers with the three # symbols, then write your Devlogs below them.
1) Because Floats are fractionless numbers. R, G, B was divided by 3 (0.66666). Int defines only whole numbers, strings and booleans are not applicable because they only regard text or t/f statements, not fractions.
2) Because Int is applicable to only whole numbers. _bounce falls under that category similarly to the specifics of R, G, B. 
3) Its because the value we put did not include f after the whole number 1.0. 
## Open-Source Assets
### W1
- Animals: https://assetstore.unity.com/packages/3d/characters/animals/animals-free-animated-low-poly-3d-models-260727 
- Low-poly environment: https://assetstore.unity.com/packages/3d/environments/landscapes/low-poly-simple-nature-pack-162153 

### W3
Activity 1:
1. The input would be the player's friendship level as well as the flag for the dialogue. The output would be the dialogue succeeding itself. 
2. The method input would be the percentage or decimals. The output is void since the sanity dictates the output, not a if or when. 
3. The method would return a boolean since the beat is dependant on a true or false statement. Basically meaning, "did we hit the beat or not?". The output would be "we hit it" or "we didn't".

Activity 2: 
Metaphor: In the original W1 minigame, the Cat Moving Script itself is the class. The blueprint. 
While the actual script written or key features in it are the Components.
The Member Variables are the data. Data as in the color of the cat, traits, etc. 

Part 3:
The balls get really bright because every time they bounce the value of their color is multiplied (*=) and increased instead of resetting between the bounces. 

### W4
Table #10
1.) We found that adding a Rigid Body to the Cat and and turning Freeze Rotation checked for the X, Y, and Z axis allows the ball to be hit by the cat instead of phased. 
	We added Rigid Body to the Soccerball and Cat but none on the Goal because Rigidbody is only applicable to physics based objects. The Goal doesn't need this.
	The Ball has a sphere collider with Is Trigger unchecked so that the ball can move whereas the goal has Is Trigger checked. The goal only has a box collider on with Is Trigger. 

2.) Me and Yixiong encountered an error in Step 1 where the OnTrigger enter method written with the .tag was not working as written on the slides.
	This was due to the full method type we initially wrote as (Collider other). So we had to write our if statement as:
	        if (other.gameObject.tag == ("Goal"))
To work. Emphasis on other.gameObject.tag! Took awhile to fix and got some assitance but resolved at the end. 