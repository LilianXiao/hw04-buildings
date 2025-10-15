# CIS 5660 HW04 Procedural Buildings

## Visual Goals
I'm personally a huge fan of Gothic, Neo-Gothic/Gothic Revival, and Victorian architecture!  Visually, Gothic architecture comprises spires, pointed arches, buttresses, and stained-glass traceries; Neo-Gothic architecture also developed alongside Neoclassical architecture in the Victorian era (think expansive and powerful geometric structures with pillars, facades, and an overall focus on horizontal and vertical lines).

<img width="425" height="635" alt="image" src="https://github.com/user-attachments/assets/e0901c84-de9e-4c8b-a58b-b6fa404a0629" />
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/df9d3499-73f5-4883-aa78-2d2292243d48" />
<img width="821" height="387" alt="image" src="https://github.com/user-attachments/assets/3ad6222c-9e3d-4f6e-b15f-9a40e8ba174e" />
<img width="730" height="486" alt="image" src="https://github.com/user-attachments/assets/91a6c85c-ba00-4873-8410-52d1fb17bf57" />
<img width="710" height="415" alt="image" src="https://github.com/user-attachments/assets/45d4fac6-7caa-4646-b224-5be1acb568e1" />
<img width="1100" height="717" alt="image" src="https://github.com/user-attachments/assets/305ab8b6-7249-4de3-8012-fed3f760207d" />
<img width="700" height="525" alt="image" src="https://github.com/user-attachments/assets/5797fc86-a950-431b-bb70-69ff45ce8c63" />
<img width="2560" height="1906" alt="image" src="https://github.com/user-attachments/assets/80c059b8-7870-46a5-b043-1068355da6d1" />


For the purposes of this assignment, I'll be simplifying the more grand flourishes present in Gothic architecture (I fear for the time I have to make everything, but we'll see how it goes...); required assets are boiled down to:
- Rectangular paned windows
- Greco-Roman pillars
- A couple different facade designs (I'm thinking Neoclassical and Gothic)
- Tower spires
- Arches
- A few different overhang styles (flat, leaning, pyramid, gable, etc.)
- Maybe even simple clocks (clocktowers, much?)

**These are just my initial thoughts.  I may end up straying into more modern architectural styles at the turn of the century, like Art Deco apartments and skyscrapers of the early to mid 20th century!


## Project Overview
In this homework you’ll gain more experience with tool creation and loops. The core of this homework will be following a Procedural House tutorial to create a multi-floor building generator. The tutorial is linked here: 
https://www.youtube.com/watch?v=uIe97023sDk&t=979s&ab_channel=SimonHoudini 

## Part 0: Setup and Planning 
### SideFX Labs 
The tutorial requires some nodes from SideFX Labs. If you haven’t already installed it, you can do so at the “Labs/Packages” tab of the Houdini Launcher.  

### Project Planning
Before you begin on this project, skim through the tutorial and then pick a building type/style you’d like to emulate (either from photos or concept art). You should watch the entirety of the tutorial  before committing to a style so you can pick something that is manageable and will be achievable using the techniques in the tutorial.  
Of course, you’re welcome to adapt the setup to support additional logic/features to match your style, and particularly complex additions could merit extra credit :) On the other hand, if you’re newer to Houdini and want to stick relatively close to the tutorial, that’s okay too. Just be sure to think through what changes your chosen buildings will require (additional assets? different placement logic?) before diving into the project so you don’t bite off more than you can chew.  
Make sure the include the reference you select in your README, and don’t forget to credit your sources.  
Here are a few examples of possible building styles that could be a decent fit for inspiration:
CIS 5660 HW03 Procedural Building 1 
https://www.behance.net/gallery/23773965/ISOBuilding-concept-art 

https://polycount.com/discussio 
low-poly-building
https://www.artstation.com/artwork/m6xYy 

## Part 1: Box Stacking HDA
First, start by following the tutorial to make a simple HDA that stacks boxes on each other.  Important note about HDA creation:  
Creating an HDA saves a .hda file at the location you specify with the definition of your HDA. Be sure to submit this .hda file along with your .hip file so we can see the contents of your tool.  
Alternatively, when you save your HDA you can choose the “Embedded in HIP File” option (rather than specifying the path), and the hda definition will be automatically embedded in your hip file (and no additional files will be needed with submission).  

## Part 2: Add Details
Next, Simon adds details to the boxes to create floors by refiing the shape and adding details like windows, doors, and balconies.  
Create your own models for windows, doors, and balconies based on your chosen style using Houdini. For each of the three types, create a Null “control” node with parameters that affect your window/door/balcony output (similar to how we made a control node for the jellyfish).  
You should have parameters to drive the width and height of the doors, windows, and balconies, as well as at least one other parameter of your choosing on each one (ex: double vs single doors, windows with and without shutters, and type of balcony railing). Apart from that, you can go as simple or complex as you like!  
Then follow Simon’s setup to integrate your windows, doors, and balconies into your buildings.  
CIS 5660 HW03 Procedural Building 2 

## Part 3: Pillars and Border
Continue following the tutorial to add pillars and borders to each floor. 

## Part 4: Supports
Continue following the tutorial to add supports to floors that overhang other floors.  
(Optional) Extra Credit 
Throughout the tutorial, Simon mentions ways you could extend his project setup. Implement any of his suggestions: 
More complex logic for creating supports (handle different length supports differently) Add more parameters to the user interface (for example, x and z offset options) UV and shade your models 
Add a “manual node” where users can control detail placement manually 
Add additional types of feature models (like fire escapes or chimneys). Note that, depending on what you choose, you might need to add new logic to integrate them into your building (ex: chimneys go on top instead of being chained on the side, fire escapes should be on one side of the building and go all the way down). We’ll award more extra credit accordingly.  
Add some flair to your scene by dressing together multiple buildings or additional procedural props or background elements 
Render your scene 

## Submission
Update your README with 
A description of your project 
A video of your building tool in action 
Create a pull request to this repository 
Submit your Houdini file to Canvas along with a link to your pull request 
IMPORTANT NOTE: make sure your HDA is either embedded in the HIP file or included with your submission (see the instructions under “Part 1: Box Stacking HDA” for additional details).
