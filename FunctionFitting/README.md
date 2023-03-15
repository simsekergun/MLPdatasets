The first column of this dataset is some $x$ values and the second column is $f(x)$

![Visualization of the data](https://github.com/simsekergun/MLPdatasets/blob/main/FunctionFitting/clean_data.png)

We know that $f(x)$ is in the following form but we don't know what $\alpha$ values we should use. Your second task is finding these $\alpha$ values with $\textsf{fsolve}$ (either in MATLAB or Python). 

$f(x) = \frac{\alpha_1 x^2 e^{-\left(\frac{x-\alpha_2}{\alpha_3}\right)^2}}{1+\alpha_4 x^2}-\alpha_5$

Please use [20 60 80 2 5] as your initial guess 
