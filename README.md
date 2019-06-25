
import pickle
import numpy as np
with open('array.pickle', 'rb') as p:
    arr = pickle.load(p)
a=np.array(p)
print(len(a))
a.resize(20,50)
b=a.T
print(b)
c=np.dot(a,b)
print(c)
d=np.sum(c,axis=1)
print(d)
print(np.cbrt(c))
print(np.sin(c))
print(np.cos(c))
print(np.arctan(c))
