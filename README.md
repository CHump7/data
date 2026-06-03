
# Func 
```
Ex.
  func name():
    instruction 1
    instruction 2
```
# Parameteres 
## is the ()
# Arguments 
## is in the parenthesis
# rotate
# variables 
## are values that change over time and you can give names to them
# _process(delta) 
## runs multiple times per second,  every frame
# delta 
## is the time it took Godot to complete the previous frame, when multiplying by delta you make it time depandant instead of frame dependant... delta represents a fraction of a second, its value is typically very small (around 0.0167 at 60 frames per second)  
```
Ex.
(3.0 * delta)
```
# Range(n) 
## used for numbers in parameters, in the example below it would count 0 through 4  
```
Ex.
Range(5)
```
# array 
## is like range but typed out manually and with brackets [1, 2, 3...] an empty array counts as false and an array with items counts as true
# # for comments
# -= for health -= amount to lose health 
# += for health += amount to gain health... The big difference is replacing (=) vs. building on (+=)
# move_left, move_right
# ==  
## means equal to
# != 
## means not equal to
# pass 
## can be used as a placeholder to not recieve and error
# .append() 
## adds a new value at the end of an array 
# string 
## or str() holds the value of text with quotes "this is a text string" and can be used to turn numbers and vectors into text
# round() 
## rounds decimals to the nesrest whole number
# lerp() 
## short for linear interpolate takes 3 arguments a start value, an end value, and and a blend amount between 0.0 and 1.0
# Vector2(x,y) 
## used to write coordinates... 
## Vector2.length() calculates and returns the length of the vector in pixels... 
## Vector2.normalized() calculates and returns the vector divided by its length, which helps us limit the length to one... 
## Checking if the vector length is greater than zero is a good way to check if the player is pressing any movement keys... 
### To calculate the length of the vector, we use the following calculations:

    We square the x and y components of the vector.
    We sum the results.
    We take the square root of the sum.

# .pop_front() 
## used to remove values from the start of the array
# .pop_back() 
## removes values from the end of the array
# dictionary 
## allows you to map pairs of values 
```
Ex.
  var dictionary = { key1: value1, ...}
```
# int() 
## short for integer, can turn strings, deicmals, and booleans into whole numbers
# float() 
## can turn strings into decimals
# deviding by whole  numbers will only return whole numbers
## ex. 3/2 = 1.  
# deviding by decimals will return decimals 
## ex. 3.0/2.0 = 1.5
# := 
## can be used to set the type value after the equal sign to use type hints and can help find errors faster like below
```
Ex.
var cell_size := Vector2(50.0, 50.0)
```
# CanvasLayer Node 
## can make UI stay on the screen like the heath bar if you make the health bar a child node of CanvasLayer
# F 
## press the F key in Godot to center
# +, -, +- 
## can be seen next to code to indicate if the code has been added, subtracted, or changed on the old, diff, or new tab
# .angle() 
## is a function of Vector2 and can be used with rotation to always face the direction that the object is moving in 
```
Ex.
var velocity := Vector2(0,500)
  rotation = velocity.angle()
```
# Input.get_axis() 
## The function Input.get_axis() takes two input action names as arguments and returns a value between -1.0 and 1.0. and the order of the arguments in Input.get_axis() matters. The first argument corresponds to the negative direction, while the second argument corresponds to the positive direction. If you invert them, you'll get inverted movement!
```
Ex.
direction.x = Input.get_axis("move_left", "move_right")
```
# ^ 
## ^ stands for "to the power of"
# sqrt() 
## sqrt means "square root"
# Input.is_action_just_pressed()
## is used to detect when the player first presses a key
# In Godot 4.6, when you run your game, it can appear directly inside the editor in the Game workspace. 
## You can playtest your game without switching to a separate window, and you get access to useful debugging tools.
```
func _ready() -> void:
	if not Engine.is_embedded_in_editor():
		get_window().mode = Window.MODE_FULLSCREEN
```
## This code checks if the game is running inside the editor. If it's not (meaning the player launched the exported game), it switches to fullscreen.
# Control + A
## is the hotkey for addinbg a node
# Sprite2D node 
## right-click on the empty Texture property of the Sprite2D node in the Inspector. Godot offers a long list of compatible resource types you can manually create, and it also offers a Quick Load option at the bottom of the list. then uou can fuzzy search for the compatable file if you know the file name.
# warning sign next to node
## Whenever Godot shows a warning like this, it means the node is missing something to do its job. You can hover over the warning sign or click it to see what's missing.
# signal syntax to connect a signal
```
signal_name.connect(function_to_call)
```
# _
## A leading underscore in a variable or function name means that you don't want anyone to use this function or variable from another script. It's a convention to indicate that this function or variable should only be used within the same script. Functions like _ready() and _process() are special functions that Godot calls automatically, so you don't want other scripts to call them directly. Similarly, When we make a function that responds to a signal, it's often very specific, so we use an underscore to show that it's not meant to be used elsewhere.
# _ready()
## tells Godot to call the node once
# queue_free
## To delete a node and its children, you can call the queue_free() function
# Refactoring
## Reworking a scene or a script to allow adding new features is a common task in programming and game development. We call this refactoring.
# Remote scene tree
## The remote scene tree is a tool that allows you to inspect the nodes in your running game.
# Refactoring
##  Reworking a scene or a script to allow adding new features is a common task in programming and game development. We call this refactoring.
# Control node
## The Control node is an invisible point or box that can contain other UI elements
