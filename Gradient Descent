# Enter your code here. Read input from STDIN. Print output to STDOUT
import math
import numpy as np
# import matplotlib.pyplot as plt

def grad(x):
    return 6*x + 2 + 4*math.cos(x)

def cost(x):
    return 3*x**2 + 2*x + 4*math.sin(x)

def myGD1(eta, x0):
    x=[x0]
    for i in range (100):
        x_new = x[-1] - eta*grad(x[-1])
        if abs(grad(x_new)) < 1e-3:
            break
        x.append(x_new)
    return (x, i)

def main():
    (x1, i1) = myGD1(.1, -5)
    (x2, i2) = myGD1(0.01, -1)
    print('x1 = %f, cost = %f after %d', x1[-1], cost(x1[-1]), i1)
    print('x2 = %f, cost = {co} after %d', x2[-1], cost(x2[-1]), i2)


if __name__ == "__main__":
    main()
