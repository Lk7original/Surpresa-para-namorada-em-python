# Surpresa-para-namorada-em-python

import turtle


 # Definindo a janela e a caneta
window = turtle.Screen()
pen = turtle.Turtle()

# Definindo a cor da caneta
pen.color('red')


# Desenhando o coração
pen.begin_fill()
pen.left(45)
pen.forward(100)
pen.circle(50, 180)
pen.right(90)
pen.circle(50, 180)
pen.forward(100)
pen.end_fill()

# Definindo a cor da caneta para amarelo e o tamanho da estrela
pen.color('yellow')
star_size = 15

# Desenhando as estrelas em volta do coração
pen.penup()
pen.goto(-135, 180)
pen.pendown()
for i in range(5):
    pen.begin_fill()
    for j in range(5):
        pen.forward(star_size * 2)
        pen.right(144)
    pen.end_fill()
    pen.penup()
    pen.forward(star_size * 5)
    pen.right(144)
    pen.pendown()

# Desenhando a segunda estrela em volta do coração
pen.penup()
pen.goto(95, 180)
pen.pendown()
for i in range(5):
    pen.begin_fill()
    for j in range(5):
        pen.forward(star_size * 2)
        pen.right(144)
    pen.end_fill()
    pen.penup()
    pen.forward(star_size * 5)
    pen.right(144)
    pen.pendown()


# Desenhando a terceira estrela em volta do coração
pen.penup()
pen.goto(95, 80)
pen.pendown()
for i in range(5):
    pen.begin_fill()
    for j in range(5):
        pen.forward(star_size * 2)
        pen.right(144)
    pen.end_fill()
    pen.penup()
    pen.forward(star_size * 5)
    pen.right(144)
    pen.pendown()


# Desenhando a quarta estrela em volta do coração
pen.penup()
pen.goto(-135, 80)
pen.pendown()
for i in range(5):
    pen.begin_fill()
    for j in range(5):
        pen.forward(star_size * 2)
        pen.right(144)
    pen.end_fill()
    pen.penup()
    pen.forward(star_size * 5)
    pen.right(144)
    pen.pendown()


# Escrevendo o nome no meio do coração
pen.penup()
pen.goto(-60, 80)
pen.color('white')
pen.write('Seu nome', font=('Arial', 20, 'bold'))

# Finalizando o desenho
pen.hideturtle()
window.mainloop()



