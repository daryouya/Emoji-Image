# smiley-face-image
Simple smiley face constructed via the python programming language

To kick-start this github profile, here is the code for a smiley face via an import file






#download the import file via the internet in order to get access to pre-made functions and such

import arcade

# set your screen boundaries - heoght and width

SCREEN_WIDTH = 600
SCREEN_HEIGHT = 600

#open a seperate window to display our visual

arcade.open_window(SCREEN_WIDTH, SCREEN_HEIGHT, "Today's Example") # this labels what you'd like to call your example

arcade.set_background_color(arcade.color.white)

arcade.start_render()

#drawing the face

x = 300
y = 300
radius = 200
arcade.draw_circle_filled(x, y, radius, arcade.color.YELLOW)

#drawing the eyes

x = 370
y = 350
radius = 20
arcade.draw_circle_filled(x, y, arcade.color.BLACK)

x = 230
y = 350
radius = 20
arcade.draw_circle_filled(x, y, arcade.color.BLACK)

#drawing the smile

x = 300
y = 280
width = 120
height = 100
starting_angle = 190
ending_angle = 350
arcade.draw_arc_outline(x, y, width, height, arcade.color.BLACK, starting_angle, ending_angle, 10)

arcade.finish_render()

#run this code

arcade.run()
