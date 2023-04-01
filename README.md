# Cora-o-em-python

import turtle

# função para desenhar um coração
def draw_heart(x, y, size):
    turtle.penup()
    turtle.goto(x, y)
    turtle.pendown()
    turtle.begin_fill()
    turtle.left(45)
    turtle.forward(size)
    turtle.circle(size/2, 180)
    turtle.right(90)
    turtle.circle(size/2, 180)
    turtle.forward(size)
    turtle.end_fill()

# desenhar o coração
turtle.speed(2)
turtle.color('black', 'red')
draw_heart(0, 0, 100)

# escrever o texto no meio do coração
turtle.penup()
turtle.goto(-55, 80)
turtle.write("I LOVE YOU", font=("Arial", 16, "normal"))

# finalizar a janela
turtle.done()
