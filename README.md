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
string # holds the value of text with quotes "this is text"
round() # rounds decimals to the nesrest whole number
lerp() # short for linear interpolate takes 3 arguments a start value, an end value, and and a blend amount between 0.0 and 1.0
Vector2(x,y) # used to write coordinates
.pop_front() # used to remove values from the start of the array
.pop_back() # removes values from the end of the array
