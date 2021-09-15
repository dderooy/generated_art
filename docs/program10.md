## The Code
```python
from turtle import *
import math
from random import *

def check_prime(num):
   if num > 1:
       for i in range(2, num):
           if (num % i) == 0:
               return False
       else:
           return True
           primes.append(num)

def main():
    phi = ( 1 + math.sqrt(5) ) / 2
    pi = math.pi
    t = Turtle()
    t.hideturtle()
    t.speed(0)
    colormode(255)
    prev = 0
    prev_angle = 72

    for x in range(1000):
        #path
        t.up()
        #t.color("white")
        t.forward(prev*phi)
        prev = x
        t.right(prev_angle)
        prev_angle += 0.1
        t.down()

        #shape properties
        size = randint(5, 5)
        if check_prime(x):
            t.fillcolor((250, randint(100, 180), 100)) #rgb
        elif (x % 2) == 0:
            t.fillcolor((100, randint(200, 250), 250)) #rgb
        else:
            t.fillcolor((100, randint(100, 150), 250)) #rgb
        t.begin_fill()

        #draw shape
        path_dir = t.heading()
        t.right(x*pi)
        poly_angle = 90
        # for angle in range(360/poly_angle):
        #     t.right(poly_angle)
        #     t.forward(size)

        #golden rect
        t.right(poly_angle)
        t.forward(size)
        t.right(poly_angle)
        t.forward(size*phi*2)
        t.right(poly_angle)
        t.forward(size)
        t.right(poly_angle)
        t.forward(size*phi*2)

        t.setheading(path_dir)
        t.end_fill()

    done()


if __name__ == '__main__':
    main()
```

## Notes
Similar to prog 9 but with more variants

## Results

<img width="700" alt="cover_pic" src="_images/program10/1.png">
<br />
<br />
<img width="700" alt="cover_pic" src="_images/program10/2.png">
<br />
<br />
<img width="700" alt="cover_pic" src="_images/program10/3.png">
<br />
<br />
<img width="700" alt="cover_pic" src="_images/program10/4.png">
<br />
<br />
<img width="700" alt="cover_pic" src="_images/program10/5.png">
<br />
<br />
<img width="700" alt="cover_pic" src="_images/program10/6.png">
<br />
<br />
<img width="700" alt="cover_pic" src="_images/program10/7.png">
<br />
<br />
<img width="700" alt="cover_pic" src="_images/program10/8.png">
<br />
<br />
<img width="700" alt="cover_pic" src="_images/program10/9.png">