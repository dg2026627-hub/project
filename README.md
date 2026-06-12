# project
Web VPython 3.2
body1 = sphere(pos=vector(3, 1, -10), radius=1, color=color.white)
body2 = sphere(pos=vector(3, -0.7, -10), radius=1.2, color=color.white)
head = sphere(pos=vector(3, 2.3, -10), radius=0.6, color=color.white)
eye1 = sphere(pos=vector(-5.2, 2.5, -10.5), radius=0.08, color=color.black)
eye2 = sphere(pos=vector(-5.2, 2.5, -10.5), radius=0.08, color=color.black)

a = arrow(pos=vec(1.3, -3, 0), axis=vec(1, 0, 0), color=color.orange, shaftwidth = 0.1)

box(pos = vec(7, 0, -10), size = vec(0.1,1,0.1))
box(pos = vec(7, 1, -10), size = vec(0.1,1,0.1))
box(pos = vec(7, 2, -10), size = vec(0.1,1,0.1))
box(pos = vec(7, 3, -10), size = vec(0.1,1,0.1))
box(pos = vec(7, 4, -10), size = vec(0.1,1,0.1))

box(pos = vec(-2, 0, -10), size = vec(0.1,1,0.1))
box(pos = vec(-2, 1, -10), size = vec(0.1,1,0.1))
box(pos = vec(-2, 2, -10), size = vec(0.1,1,0.1))
box(pos = vec(-2, 3, -10), size = vec(0.1,1,0.1))
box(pos = vec(-2, 4, -10), size = vec(0.1,1,0.1))

box(pos = vec(-1.5, 4.5, -10), size = vec(1,0.1,0.1))
box(pos = vec(-1, 4.5, -10), size = vec(1,0.1,0.1))
box(pos = vec(0, 4.5, -10), size = vec(1,0.1,0.1))
box(pos = vec(1, 4.5, -10), size = vec(1,0.1,0.1))
box(pos = vec(2, 4.5, -10), size = vec(1,0.1,0.1))
box(pos = vec(3, 4.5, -10), size = vec(1,0.1,0.1))
box(pos = vec(4, 4.5, -10), size = vec(1,0.1,0.1))
box(pos = vec(5, 4.5, -10), size = vec(1,0.1,0.1))
box(pos = vec(6, 4.5, -10), size = vec(1,0.1,0.1))
box(pos = vec(6.5, 4.5, -10), size = vec(1,0.1,0.1))
ball = sphere(pos=vec(-9, 0, 0), radius=0.5, color=color.purple,v=vec(2, 0, 0),pos = vec(0,-2.3,0))
dt = 0.1
while ball.pos.x < 1.5:
    rate(100)
    ball.pos = ball.pos + ball.v*dt
    
while True :
    rate(100)
    k = keysdown()
    if 'left' in k :
        a.axis.x -= 0.1
    if 'right' in k :
        a.axis.x += 0.1
    if 'down' in k :
        a.axis.y -= 0.1
    if 'up' in k:
        a.axis.y += 0.1
    if ' ' in k :
        ball.pos = ball.pos + a.axis * 0.01
https://www.glowscript.org/#/user/dg2026627/folder/MyPrograms/program/%EC%88%98%ED%96%89
