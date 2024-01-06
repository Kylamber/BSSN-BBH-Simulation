# BSSN Black Hole Simulation using Python
Binary black hole simulation using the Baumgarte-Shapiro-Shibata-Nakamura (BSSN) formalism with Python. The code and equations explanation is in the notebook, install the required packages or run in Goolge Colab. Currently the code is only for black hole simulation using Brill-Lindquist initial data. I plan to add support for black holes with linear momentum using Bowen-York initial data.

**Note.** If you plan to run this code locally, keep in mind that out of the box it will use the ./Data/ directory to save the files. To be safe, put the notebook file in an empty folder.

## Requirements
This notebook requires:
- Jupyter
- PyTorch (Install the CUDA version to enable GPU acceleration)
- NumPy
- Matplotlib

## Results
This is the resulting evolution using these parameters. Though unfortunately the simulation crashes before it properly merges.
```
Grid:
resolution = 0.0625
n_grid = 96

Black hole choice:
BH_locs = [[0.0, 0.0, 0.5], [0.0, 0.0, -0.5]]
BH_masses = [0.5, 0.5]

Evolution choice:
temporal_differencing = RK4
CF = 0.5

BSSN Parameters:
damping = 2
lambdas = [1, 1, 1, 1]
f1_alpha = 2/alpha
f2_alpha = one
enforce_constraints = True
conformal_variable = phi
epsilon = 1e-08
```

https://github.com/Kylamber/BSSN-BBH-Simulation/assets/32596839/863526a6-a4b0-489a-8fea-494354e4c2ef

https://github.com/Kylamber/BSSN-BBH-Simulation/assets/32596839/6c3319dd-bc90-4574-b4ee-33f5437b993a

## References

Alcubierre, M., Brügmann, B., Diener, P., Koppitz, M., Pollney, D., Seidel, E., & Takahashi, R. (2003). Gauge conditions for long-term numerical black hole evolutions without excision. Physical Review D, 67(8), 084023.

Baumgarte, T. W., & Shapiro, S. L. (2010). Numerical relativity: solving Einstein's equations on the computer. Cambridge University Press.

Baumgarte, T. W., & Shapiro, S. L. (2021). Numerical relativity: starting from scratch. Cambridge University Press.

Brügmann, B., González, J. A., Hannam, M., Husa, S., Sperhake, U., & Tichy, W. (2008). Calibration of moving puncture simulations. Physical Review D, 77(2), 024027.

Campanelli, M., Lousto, C. O., Marronetti, P., & Zlochower, Y. (2006). Accurate evolutions of orbiting black-hole binaries without excision. Physical Review Letters, 96(11), 111101.

Cao, Z., Yo, H. J., & Yu, J. P. (2008). Reinvestigation of moving punctured black holes with a new code. Physical Review D, 78(12), 124011.

Harris, C. R., Millman, K. J., Van Der Walt, S. J., Gommers, R., Virtanen, P., Cournapeau, D., ... & Oliphant, T. E. (2020). Array programming with NumPy. Nature, 585(7825), 357-362.

Hunter, J. D. (2007). Matplotlib: A 2D graphics environment. Computing in science & engineering, 9(03), 90-95.

Paszke, A., Gross, S., Massa, F., Lerer, A., Bradbury, J., Chanan, G., ... & Chintala, S. (2019). Pytorch: An imperative style, high-performance deep learning library. Advances in neural information processing systems, 32.

Ruchlin, I., Etienne, Z. B., & Baumgarte, T. W. (2018). SENR/NRPy+: Numerical relativity in singular curvilinear coordinate systems. Physical Review D, 97(6), 064036.

Shibata, M. (2015). Numerical relativity (Vol. 1). World Scientific.

van Meter, J. R., Baker, J. G., Koppitz, M., & Choi, D. I. (2006). How to move a black hole without excision: gauge conditions for the numerical evolution of a moving puncture. Physical Review D, 73(12), 124011.
