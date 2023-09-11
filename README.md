# Driving-Parameters-Supplemented-to-arXiv-2305.17097
We will update the paper arXiv:2305.17097 soon. This repository contains data for driving parameters in the 5 figures in Supp. Mat of the updated version.
$\eta$ range is $[0, \log(2.6)+x]$ with 200 equally spaced points.
Pickle files with driving parameters contains Fourier modes in the form of Eq. (S14) in Supp. Mat. in arXiv.2305.17097.
They can be opened in Python with, e.g. (after renaming files)
```python
import pickle
import numpy as np

with open('drive_x.pickle', 'rb') as f:
    drive_x = np.array(pickle.load(f))

with open('drive_y.pickle', 'rb') as f:
    drive_y = np.array(pickle.load(f))

with open('drive_z.pickle', 'rb') as f:
    drive_z = np.array(pickle.load(f))

with open('x.pickle', 'rb') as f:
    x = pickle.load(f)
```
