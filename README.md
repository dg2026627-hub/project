# project
Web VPython 3.2
body1 = sphere(pos=vector(0, 1, 0), radius=1, color=color.white)
body2 = sphere(pos=vector(0, -0.7, 0), radius=1.2, color=color.white)
head = sphere(pos=vector(0, 2.3, 0), radius=0.6, color=color.white)
eye1 = sphere(pos=vector(-0.2, 2.5, 0.5), radius=0.08, color=color.black)
eye2 = sphere(pos=vector(-0.2, 2.5, 0.5), radius=0.08, color=color.black)
a = arrow(pos=vec(0, -3, 0), axis=vec(1, 0, 0), color=color.orange, shaftwidth = 0.1)
box(pos = vec(10, 0, 0), size = vec(0.1,1,0.1))
box(pos = vec(10, 1, 0), size = vec(0.1,1,0.1))
box(pos = vec(10, 2, 0), size = vec(0.1,1,0.1))
box(pos = vec(10, 3, 0), size = vec(0.1,1,0.1))
box(pos = vec(10, 4, 0), size = vec(0.1,1,0.1))
box(pos = vec(1, 0, 0), size = vec(0.1,1,0.1))
box(pos = vec(1, 1, 0), size = vec(0.1,1,0.1))
box(pos = vec(1, 2, 0), size = vec(0.1,1,0.1))
box(pos = vec(1, 3, 0), size = vec(0.1,1,0.1))
box(pos = vec(1, 4, 0), size = vec(0.1,1,0.1))
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
