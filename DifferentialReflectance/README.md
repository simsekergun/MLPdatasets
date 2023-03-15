### Differential reflectance dataset 
This dataset is taken from one of my earlier papers. 
Please read it, if you have time. Here's the \href{https://redirect.cs.umbc.edu/~simsek/journal_papers/j31_n_with_NN.pdf}{link} for an electronic copy of that paper. 

### Introduction
Figures below shows a typical reflectance measurement setup. 
The one on the top measures reflectance from a p-polarized laser, the one on the bottom from an s-polarized laser. 
Note that these letters have a German origin: s = senkrecht = perpendicular, p = parallel. 
It basically tells whether the electric field is perpendicular or parallel to the plane of incidence. 
![](https://github.com/simsekergun/MLPdatasets/blob/main/DifferentialReflectance/p_reflectance.png)
![](https://github.com/simsekergun/MLPdatasets/blob/main/DifferentialReflectance/s_reflectance.png)

The wavelength of the laser is 400 nm. We place a 0.7 nm thick film on a substrate whose complex refractive index is $\tilde{n} = n+ik$, where the real part $n$ is the refractive index and indicates the phase velocity, while the imaginary part $k$ is called the optical extinction coefficient or absorption coefficient. We work either with SiO$_2$-coated silicon substrates or glass substrates. We change the incidence angle from 0 degrees to 60 degrees at a step of 1 degrees and we record the intensity of the reflected light with the help of a photodiode. When we use reflectance from the bare substrate as a reference, then we can get the differential reflectance by simply calculating $(\Gamma-\Gamma_0)/\Gamma_0$, where $\Gamma$ and $\Gamma_0$ are the reflectances from the sample coated substrate and bare substrate.

### Dataset
Reflectance_X_train.csv has 244 columns as follows. <br>
(a) Columns 1-61: reflectance data as a function of incidence angle (from 0 degrees to 60 degrees)<br>
of p-polarized 400 nm laser from a material with a thickness of 0.7 nm placed on top of a <br>
SiO$_2$/silicon substrate, <br>
(b) Columns 62-122: similar to (a) for s-polarized laser, <br>
(c) Columns 123-183: similar to (a) for a glass substrate,<br>
(d) Columns 184:244: similar to (c) for s-polarized laser.<br>

<br>
Each row corresponds to a unique ($n$, $k$)-pair given in Reflectance_Y_train.csv. <br>
As you can see, $n$ changes between 0.1 and 6 and $k$ changes between 0 and 5, both at the steps of 0.1. 
<br>
Your task is finding the (n, k) values for the reflectance data given in 
Reflectance_X_test.csv, which is in the same format as the Reflectance_X_train.csv.
