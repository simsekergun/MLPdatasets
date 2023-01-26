PIN Dataset-1
### Rows
This dataset includes physical parameters of 200 p-i-n type photodetector, where the 
* p-layer is a p-doped InGaAs layer with a thickness of t1 and a doping level of d1
* i-layer is an n-doped InGaAs layer with a thickness of t2 and a doping level of d2
* n-layer is an n-doped InP layer with a thickness of t3 and a doping level of d3

### Columns
Columns 1-3: t1, t2, t3 (layer thicknesses, unit: nm) <br>
Columns 4-6: d1, d2, d3 (doping levels, unit: cm<sup>-3</sup>) <br>
Column 7: Phase noise (dBc/Hz) <br>
Column 8: Quantum efficiency (unitless) <br>
Column 9: Decay time (ps) <br>
Column 10: Bandwidth (GHz) <br>

### Objectives
1. Do an EDA
2. Predict the quantum efficiency using phase noise as the single input in a simple linear regression
3. After determining the correlation between inputs (t1, t2, t3, d1, d2, d3) and the output (phase noise), predict the phase noise using columns 1-6 (t1, t2, t3, d1, d2, d3) as the inputs in a multivariate linear regression.
4. Repeat step 3 to predict the quantum efficiency
5. Comment on the results.


