Func # ex.
  func name():
    instruction 1
    instruction 2

Parameteres # is the ()
Arguments # is in the parenthesis
rotate
variables # values that change over time and you can give names to them
_process(delta)   # runs multiple times per second,  every frame
delta # the time it took godot to complete the previous frame, when multiplying by delta you make  it time depandant instead of frame dependant  ex. (3.0 * delta)
Range(n) # used for numbers in parameters -1
array # is like range but typed out manually and with brackets [1, 2, 3...] an empty array count as false and an array with items counts as true
# for comments
-= for health -= amount to lose health
+= for health += amount to gain health
move_left
move_right
== # means equal to
!= # means not equal to
pass # can be used as a placeholder to not recieve and error
.append() # adds a new value at the end of an array 
string # or str() holds the value of text with quotes "this is text" and can be used to turn numbers and vectors into text
round() # rounds decimals to the nesrest whole number
lerp() # short for linear interpolate takes 3 arguments a start value, an end value, and and a blend amount between 0.0 and 1.0
Vector2(x,y) # used to write coordinates
.pop_front() # used to remove values from the start of the array
.pop_back() # removes values from the end of the array
dictionary # allows you to map pairs of values ex.
  var dictionary = { key1: value1, ...}
int() # short for integer, can turn strings, deicmals, and booleans into whole numbers
float() # can turn strings into decimals
deviding by whole  numbers will only return whole numbers ex 3/2 = 1. deviding by decimals will return decimals ex 3.0/2.0 = 1.5
:= # can be used like var cell_size := Vector2(50.0, 50.0) to set the type value after the equal sign to use type hints and can help find errors faster 
CanvasLayer Node # can make UI stay on the screen like the heath bar if you make the health bar a child node of CanvasLayer
F # press the F key in Godot to center
# +, -, +- can be seen next to code to indicate if the code has been added, subtracted, or changed on the old, diff, or new tab
.angle() # is a function of Vector2 and can be used with rotation to always face the direction that the object is moving in... var velocity := Vector2(0,500)... rotation = velocity.angle()
