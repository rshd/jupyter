# linear alegbra

## Solving a System of Linear Equations

Let's take the puzzle shown for example.

```
x+y=8
u-v=6
x+u=13
y+v=6
```
Putting this matrix in the form Ax=b,

```
x,y,u,v=b_i
1,1,0,0=8
0,0,1,-1=6
1,0,1,0=13
0,1,0,1=8
```

### NumPy

The linear algebra functions are shown [here](https://docs.scipy.org/doc/numpy-1.13.0/reference/routines.linalg.html).

```
a=np.array([[1,1,0,0],[0,0,1,-1],[1,0,1,0],[0,1,0,1]])
b=np.array([8,6,13,8])
x=np.linalg.solve(a,b)
```
The solution is 
```
>>> x
array([ 3.5,  4.5,  9.5,  3.5])
```