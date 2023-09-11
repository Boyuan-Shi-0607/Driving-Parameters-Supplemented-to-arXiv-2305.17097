# Driving-Parameters-Supplemented-to-arXiv-2305.17097
[![DOI](https://zenodo.org/badge/690008146.svg)](https://zenodo.org/badge/latestdoi/690008146)

We will update the paper arXiv:2305.17097 soon. This repository contains data for driving parameters in the 5 figures in Supp. Mat of the updated version.

$\eta$ range is $[0, \log(2.6)+x]$ with 200 equally spaced points. For Fig. S1 (a), the $102^{\mathrm{th}}$, $103^{\mathrm{th}}$ and $104^{\mathrm{th}}$ $\eta$ values are excluded. Such $\eta$ values are near $1/2$.

Pickle files with driving parameters contains Fourier modes in the form of Eq. (S14) in Supp. Mat. in arXiv.2305.17097.


Numpy arrays are arranged from the most negative Fourier modes to the most positive Fourier modes. E.g. drive_x,y,z[i,j] refer to the $(i-M_{1})^{\text{th}}$ $\omega_{1}$ mode $(j-M_{2})^{\text{th}}$ $\omega_{2}$ mode of $d_{x}(t)$, $d_{yy}(t)$ and $d_{zz}(t)$.

They can be opened in Python with, e.g. for Fig. (S1) (a), after renaming files:
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



