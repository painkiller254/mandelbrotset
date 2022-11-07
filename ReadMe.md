# In this project, I learnt how to:

<ul>
    <li>Apply complex numbers to a practical problem</li>
    <li>Find members of the mAndelbrot and Julia sets</li>
    <li>Draw these sets as fractals using Matplotlib and pillow</li>
    <li>Make colorful artistic representations of the fractals</li>
</ul>

Fractals are infinitely repeating patterns on differet scales.

The Mandelbrot set is the set of complex numbers c, for which an infinite sequence of numbers, Z0, Z1,.....,Zn,..... remains bounde.

The first elemnet if the sequence Z0, is always equal to zero. TO calculate the next element, Zn+1, you'll keep squaring the last element, Zn and adding your initial number, c, in a feedback loop.

>>> def z(n, c):
...     if n == 0:
...             return 0
...     else:
...             return z(n - 1, c) ** 2 + c
...
>>> for n in range(10 :
  File "<stdin>", line 1
    for n in range(10 :
                      ^
SyntaxError: invalid syntax
>>> for n in range(10):
...     print(f"z({n}) = {z(n, c=1)}")
...
z(0) = 0
z(1) = 1
z(2) = 2
z(3) = 5
z(4) = 26
z(5) = 677
z(6) = 458330
z(7) = 210066388901
z(8) = 44127887745906175987802
z(9) = 1947270476915296449559703445493848930452791205
>>>

-------------------
