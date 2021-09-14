## The Code
```python
from turtle import *
import math


def main():
    phi = ( 1 + math.sqrt(5) ) / 2
    pi = math.pi
    t1 = Turtle()
    t1.hideturtle()
    t1.speed(0)
    angle = 50 #variant 
    angles = (360/angle)
    for x in range(1000):
        t1.forward(x)
        t1.right(angle)
        for num in range(angles):
            t1.right(angle)
            t1.forward(x)
    done()


if __name__ == '__main__':
    main()
```

## Notes
Similar to program 1 but without using phi. Angle is still the main variant.

## Results

<img width="700" alt="cover_pic" src="_images/program2/1.png">
<br />
<br />
<img width="700" alt="cover_pic" src="_images/program2/2.png">
<br />
<br />
<img width="700" alt="cover_pic" src="_images/program2/3.png">
<br />
<br />
<img width="700" alt="cover_pic" src="_images/program2/4.png">
<br />
<br />
<img width="700" alt="cover_pic" src="_images/program2/5.png">
<br />
<br />
<img width="700" alt="cover_pic" src="_images/program2/6.png">
<br />
<br />
<img width="700" alt="cover_pic" src="_images/program2/7.png">
