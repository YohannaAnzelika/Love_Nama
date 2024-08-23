import turtle
import time

Screen = turtle.Screen()
Screen.setup(800, 800)
Screen.bgcolor("gray")

t = turtle.Turtle()
t.hideturtle()
t.speed(0)  

def draw_heart(x, y, size, color, thickness):
    t.penup()
    t.goto(x, y)
    t.color(color)
    t.pensize(thickness)
    t.pendown()
    t.begin_fill()
    t.left(140)
    t.forward(size)

    for _ in range(100): 
        t.right(2)
        t.forward(size * 0.018)

    t.left(120)

    for _ in range(100):  
        t.right(2)
        t.forward(size * 0.018)

    t.forward(size)
    t.end_fill()
    t.setheading(0)

heart = [
    (0, -150, 300, "#8B4513", 6),
    (0, -135, 270, "#FA8072", 6),
    (0, -120, 240, "#DA70D6", 6),
    (0, -105, 210, "#DB7093", 6),
    (0, -90, 180, "#800080", 6),
    (0, -75, 150, "#DDA0DD", 6),
    (0, -50, 100, "#4682B4", 6)
]

for heart in heart:
    draw_heart(*heart)
    time.sleep(0.2)

t.penup()
t.goto(0, 20)  
t.color("black")
t.write("Yoongi", align="center", font=("Arial", 22, "bold"))

Screen.mainloop()
