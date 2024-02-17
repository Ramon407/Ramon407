import turtle

# Configurações iniciais
screen = turtle.Screen()
screen.bgcolor("black")
t = turtle.Turtle()
t.speed(10)
t.color("red", "yellow")

# Função para desenhar uma pétala
def petala():
    t.begin_fill()
    t.left(20)
    t.forward(100)
    t.left(100)
    t.forward(100)
    t.left(160)
    t.forward(100)
    t.left(100)
    t.forward(100)
    t.end_fill()

# Desenhar a flor
for _ in range(18):
    petala()
    t.left(20)

# Esconder a tartaruga e finalizar
t.hideturtle()
screen.mainloop()

