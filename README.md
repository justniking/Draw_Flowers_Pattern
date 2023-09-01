# Draw_Flowers_Pattern
import turtle

# Function to draw a flower
def draw_flower():
    turtle.begin_fill()  # Start filling the shape
    turtle.color("red")
    for _ in range(4):
        turtle.circle(20)
        turtle.left(90)
    turtle.end_fill()  # End filling the shape

turtle.speed("fastest")  # Set the speed to the fastest

# Number of rows and columns
rows = 6
cols = 6

# Distance between flowers
flower_spacing_x = 100
flower_spacing_y = 100

# Total width and height of the grid
total_width = (cols - 1) * flower_spacing_x
total_height = (rows - 1) * flower_spacing_y

# Draw flowers in a grid pattern, centered
for row in range(rows):
    for col in range(cols):
        turtle.penup()
        x = -total_width / 2 + col * flower_spacing_x
        y = total_height / 2 - row * flower_spacing_y
        turtle.goto(x, y)  # Adjust the position for each flower (centered)
        turtle.pendown()
        draw_flower()

# Hide the turtle
turtle.hideturtle()

# Keep the window open
turtle.done()

import turtle
from turtle import*
t=turtle.Turtle()
shape("turtle")
screensize(1.0,1.0)
bgcolor("white")
backward(100) 
right(120)
width(1)
for c in ['red', 'green', 'blue', 'yellow']:
    t.color(c)
    t.forward(100)
    t.left(120)
for steps in range(100):
    for c in ('blue', 'red', 'green'):
        color(c)
        forward(steps)
        right(40)      
color('red')
fillcolor('yellow')
begin_fill()
while True:
    forward(200)
    left(180)
    if abs(pos()) < 1:
        break
end_fill()

