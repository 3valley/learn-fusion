# learn-fusion
The Estes Valley Library's very own Fusion 360 tutorial

## Our first project: making a die
In Fusion's top bar menu, choose the paper icon `File` menu and then `Save`. Name your document "game pieces"
To keep everything neat, choose `Create > New Component` and name it "die"

### Selecting the plane
We have three axes and three planes to work with. Sketches are created on a flat plane, so now's the time to choose how you want to think about your model. Are you going to start top-down, from the front, from the side?

For this first example, we are going to start from the top, as if we are looking down on our die, so click the orange square between the blue and red axes (the X-Y plane)

## Start sketching
From the `Sketch` menu, choose `Rectangle > Center Point Rectangle`
When you see the crosshairs, **click once** to place the center of the rectangle. 

There are two ways to choose the size of the rectangle.
- *By dragging:* Move the cursor away from the center point, then **click** to place the rectangle.
- *By entering parameters:* Your rectangle will have two floating fields- the parameters for the sides. Begin typing (no need to select anything) to fill in the first field, then use <kbd>Tab</kbd> to move to the second field.

Let’s make a perfect square. You choose the size. Use <kbd>Command-Z</kbd> to undo if you don’t like your square.

## Entering the third dimension
Now, we officially enter the 3D realm. Choose `Create > Extrude`
A floating Extrude **pane** showing the tool options will appear. **Click** your square to select.

Now, rotate the view cube slightly so you can get a better look, and you’ll see your square has a nice blue arrow-handle sticking out. **Drag** to pull up on the handle *or* type to add the parameter. Hit <kbd>Enter</kbd> or the <kbd>OK</kbd> button on the Extrude pane to apply the extrude.

We *could* stop there, because we’ve created a printable 3D object- but I assume you want to keep going.

## Modify
I noticed that dice have slightly rounded-off sides, so we are going to `Modify` our cube to give it softened edges.

Choose either:
- `Modify > Chamfer`
- `Modify > Fillet`

then *click and drag* a selection window around the entire cube to select all of its edges. Notice the you get both a blue handle :arrow_up: you can drag or a parameter box for typing the dimension.

Try them both- just click <kbd>cancel</kbd> to leave the tool without applying the change. Try some of those crazy options even if you don’t know what they’re for. I certainly don’t. Take a second to evaluate the options and then click <kbd>OK</kbd> or hit <kbd>Enter</kbd> when you’ve got one you like.

Rotate the `view cube` a little to admire your edge treatment, because it’s about to get really wild.

## Sketching and creating on faces
First, we sketched on a plane- the first square we drew. Now, we are going to work on the *planar faces* of the die, one face at a time, The thing I think the faces need is some dots.

Choose `Create > Sphere`

Hover your cursor over a face of the die until you see the edges of the face turn *light*. You’ll also see an inviting golden-yellow square representing the plane, but don't click that- we want to select the face.

After selecting the face, **click once** to place the center of the sphere, then type a parameter for the sphere's diameter.

*Notice something different?* The sphere is red because it intersects with the face of the die and Fusion selects the Cut operation automatically. That's just fine, since we want to scoop a half-sphere out. Hit <kbd>Enter</kbd> or the OK button.

Use the view cube to move the view so another face is visible.  This time, **right-click** on the face.

A circular `context menu` will appear around your cursor. Choose `Repeat Sphere` from this menu, click once to place the center of the sphere, and use <kbd>Enter</kbd> or <kbd>OK</kbd> to cut.

## Now, finish the last four faces:
-	Rotate your view using the `view cube`
-	**Right-click** on faces to display the `context menu`, then choose `Repeat Sphere`
-	**Click once** to place the center of the sphere and use <kbd>Enter</kbd> or <kbd>OK</kbd> to cut.

## Our second project: a Monopoly-style house
Let's continue keeping things neat by creating a new component. Click the radio button next to the top level item in the `Browser` to activate it, then choose `Create > New Component` and name it "monopoly house"

- Rotate the `view cube` so the Front face is visible
- Choose `Sketch > Rectangle > 2-point Rectangle`
- Click to place one corner, then move and click to place the other.
- Choose `Sketch > Line` to draw a roof across the top of the rectangle
- Choose `Sketch > Trim`, then hover over to highlight and click to remove the extra line between the rectangle and the roof.
- Choose `Create > Extrude`. Rotate view cube if needed, then either pull the handle or enter the parameter. <kbd>OK</kbd> or <kbd>Enter</kbd> to apply.

Now, I want to add a chimney. The logical place would be on one side of this roof, but I’ll show you what happens if I do that. Instead, I want to sketch the chimney on the flat bottom of the house, and extrude it through the roof.

- Choose `Sketch > Circle > Center Point Circle` OR `Sketch > Rectangle > Center Point Rectangle`, then click and drag or type the parameter.
- Choose `Create > Extrude`, select your chimney shape and extrude it through the roof. Rotate the `view cube` as needed to see it better and then pull the handle. 

Notice that like the spheres on the die, it’s red. Because it intersects the house body, Fusion chooses the `Cut` operation by default. In the Extrude plane, change the `Operation` to `Join` and click OK.

Now, let’s add a tiny bit of character to the chimney.
- Chooose `Sketch > Offset`, click to select the face on top of the chimney, then click the line around the edge of the chimney. Pull inward or enter a negative value in the parameter field. <kbd>OK</kbd> or <kbd>Enter</kbd> to apply.
- Choose `Create > Extrude`. Select the new offset shape we just made and pull the handle down to hollow out the chimney.

###Now, on your own, add 1 more feature to the house:
-	Rotate your view using the `view cube`
-	Choose `Create > Sketch` and click on a planar face
-	Using the `Sketch` tools of your choice, sketch something on that planar face. Front steps? Door? Window? Up to you.
-	Use `Sketch > Offset` and `Create > Extrude` to make the feature 3D.

## Last trick: Rotational-symmetry game piece
Create a new component. Click the radio button next to the top level item in the `Browser` to activate it, then choose `Create > New Component` and name it "pawn" (or anything you want)

- Rotate the `view cube` so the Front face is visible
- Using the `Create > Sketch` tools, click to select the front pane and begin drawing a shape of your choosing. This one uses Center Point Circle, 2-Point Rectangle, and 3-Point Arc.
- Whatever you drew, make sure you place a `Sketch > Line` down the middle of the drawing to cut everything in half. This piece is going to have rotational symmetry and that line will be the axis that we rotate around.
- Use Sketch > Trim to remove stray lines.

### Revoling your shape
- Choose `Create > Revolve`
-	Select the shape you created. The Revolve pane will show “Profile: 1 selected”
-	In the Revolve pane, click on the <kbd>Select</kbd> button next to the `Axis` setting, then click the edge of your shape, the one that you want to be the center.
-	Leave the rest of the settings how they are and click <kbd>OK</kbd>.
















