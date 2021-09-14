## The Code
```python
from turtle import *
import math
import random


def main():
    phi = ( 1 + math.sqrt(5) ) / 2
    pi = math.pi
    t1 = Turtle()
    t1.hideturtle()
    t1.speed(0)
    prev = 0
    c = random.random()
    R = float(c/5)
    B = float(c/2)
    G = float(c)
    t1.dot(random.randint(0, 100), (R,B,G))
    for x in range(1000):
        t1.penup()
        x = random.randint(-500, 500)
        y = random.randint(-500, 500)
        t1.goto(x, y)
        t1.pendown()

        h = random.random()
        hSize = random.randint(10, 50)
        o = random.random()
        
        t1.dot(hSize, (h/5,h/2,h))
        t1.right(random.randint(0, 360))
        t1.forward(50)
        t1.dot(random.randint(50, 100), (o,o/10,o/10))
        t1.right(360-104.5)
        t1.forward(50)
        t1.dot(hSize, (h/5,h/2,h))

    done()


if __name__ == '__main__':
    main()
```

## Notes
This program aims to illustrate water molecules

## Results

<img width="700" alt="cover_pic" src="_images/program6/1.png">
<br />
<br />

