import turtle

#draws circle
def draw_circle():
    turtle.penup()
    turtle.goto(200, 100)
    turtle.pendown()
    turtle.shape("turtle")
    turtle.color("green", "red")  
    turtle.pensize(10)
    turtle.begin_fill()
    turtle.circle(100)
    turtle.end_fill()

#draws square
def draw_square():
    turtle.penup()
    turtle.goto(-200, -200)
    turtle.pendown()
    turtle.shape("turtle")
    turtle.color("green", "blue") 
    turtle.pensize(5)
    turtle.begin_fill()
    for _ in range(4):
        turtle.forward(200)
        turtle.right(90)
    turtle.end_fill()

def drawtriangle():
    turtle.penup()
    turtle.goto(0, 0)
    turtle.pendown()
    turtle.shape("turtle")
    turtle.color("green", "purple")  
    turtle.pensize(3)
    turtle.begin_fill()
    for _ in range(3):
        turtle.forward(150)
        turtle.left(120)
    turtle.end_fill()


turtle.speed(2)
turtle.bgcolor("white")  


draw_circle()
turtle.color("green")  
draw_square()
turtle.color("green") 
drawtriangle()

#resets to (0,0)
turtle.penup()
turtle.goto(0, 0)
turtle.pendown()

turtle.done()
