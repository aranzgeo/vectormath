vectormath
**********

Vector math utilities for Python.

```python
import numpy as np
import vectormath as vmath

# Simple vectors
v = vmath.Vector3(5, 0, 0)
v.normalize()
print(v) # > [[1, 0, 0]]
print(v.x, type(v.x))  # > 1.0, float

# Array based vectors are much faster than a for loop
v_array = vmath.Vector3([[4,0,0],[0,2,0]])
print(v_array.x) # > [4, 0]
# we can
print(v_array.length) # [4, 2]
print(v_array.normalize())  # [[1,0,0],[0,1,0]]

# These vectors are just numpy arrays
assert isinstance(v, np.ndarray)
```


Major classes include `Vector3`, `Matrix3`, `Plane`, `Parallelogram`.
