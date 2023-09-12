from mpl_toolkits import mplot3d


import numpy as np
import matplotlib.pylab as plt


p=10
r=28
b=8/3

h=0.001

x0=1.0
y0=1.0
z0=1.0

t0=0.0

def f1(x,y,z):
    return p*(y-x)
def f2(x,y,z):
    return -x*z+r*x-y
def f3(x,y,z):
    return x*y-b*z

"""
i)
"""

x=x0
y=y0
z=z0
t=t0

for i in range(100000):
    plt.plot(t,x,'bo', markersize=0.2)
    x+=(h/2)*(f1(x,y,z)+f1(x+h*f1(x,y,z),y,z))
    y+=(h/2)*(f2(x,y,z)+f2(x,y+h*f2(x,y,z),z))
    z+=(h/2)*(f3(x,y,z)+f3(x,y,z+h*f3(x,y,z)))
    t+=h
    
plt.title("x vs time t")
plt.xlabel("t")
plt.ylabel("x")
plt.show() 
    

x=x0
y=y0
z=z0
t=t0

for i in range(100000):
    plt.plot(t,y,'go', markersize=0.2)
    x+=(h/2)*(f1(x,y,z)+f1(x+h*f1(x,y,z),y,z))
    y+=(h/2)*(f2(x,y,z)+f2(x,y+h*f2(x,y,z),z))
    z+=(h/2)*(f3(x,y,z)+f3(x,y,z+h*f3(x,y,z)))
    t+=h
    
plt.title("y vs time t")
plt.xlabel("t")
plt.ylabel("y")
plt.show() 


x=x0
y=y0
z=z0
t=t0

for i in range(100000):
    plt.plot(t,z,'ro', markersize=0.2)
    x+=(h/2)*(f1(x,y,z)+f1(x+h*f1(x,y,z),y,z))
    y+=(h/2)*(f2(x,y,z)+f2(x,y+h*f2(x,y,z),z))
    z+=(h/2)*(f3(x,y,z)+f3(x,y,z+h*f3(x,y,z)))
    t+=h
    
plt.title("z vs time t")
plt.xlabel("t")
plt.ylabel("z")
plt.show()

"""
ii)
"""

x=x0
y=y0
z=z0
t=t0

for i in range(100000):
    plt.plot(x,y,'bo', markersize=0.2)
    x+=(h/2)*(f1(x,y,z)+f1(x+h*f1(x,y,z),y,z))
    y+=(h/2)*(f2(x,y,z)+f2(x,y+h*f2(x,y,z),z))
    z+=(h/2)*(f3(x,y,z)+f3(x,y,z+h*f3(x,y,z)))
    t+=h
    
plt.title("x vs y")
plt.xlabel("x")
plt.ylabel("y")
plt.show() 
    

x=x0
y=y0
z=z0
t=t0

for i in range(100000):
    plt.plot(y,z,'go', markersize=0.2)
    x+=(h/2)*(f1(x,y,z)+f1(x+h*f1(x,y,z),y,z))
    y+=(h/2)*(f2(x,y,z)+f2(x,y+h*f2(x,y,z),z))
    z+=(h/2)*(f3(x,y,z)+f3(x,y,z+h*f3(x,y,z)))
    t+=h
    
plt.title("y vs z")
plt.xlabel("y")
plt.ylabel("z")
plt.show() 


x=x0
y=y0
z=z0
t=t0

for i in range(100000):
    plt.plot(z,x,'ro', markersize=0.2)
    x+=(h/2)*(f1(x,y,z)+f1(x+h*f1(x,y,z),y,z))
    y+=(h/2)*(f2(x,y,z)+f2(x,y+h*f2(x,y,z),z))
    z+=(h/2)*(f3(x,y,z)+f3(x,y,z+h*f3(x,y,z)))
    t+=h

plt.title("z vs x")
plt.xlabel("z")
plt.ylabel("x")
plt.show()


"""
3D Plot
iii)
"""

fig = plt.figure(figsize=(4,4))
ax = fig.add_subplot(111, projection='3d')

x=x0
y=y0
z=z0
t=t0

for i in range(100000):
    ax.scatter(x,y,z, s=0.1, c='gray', marker='.')
    x+=(h/2)*(f1(x,y,z)+f1(x+h*f1(x,y,z),y,z))
    y+=(h/2)*(f2(x,y,z)+f2(x,y+h*f2(x,y,z),z))
    z+=(h/2)*(f3(x,y,z)+f3(x,y,z+h*f3(x,y,z)))
    t+=h

ax.set_title("x vs y vs z")
ax.set_xlabel("x")
ax.set_ylabel("y")
ax.set_zlabel("z")
plt.show()
