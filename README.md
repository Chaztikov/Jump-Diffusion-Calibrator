# Jump-Diffusion-Calibrator
In this project, calibration of parameters of Heston and Bates models using Markov Chain Monte Carlo (MCMC) is performed based on the findings in the [paper by Cape et al.](https://doi.org/10.1080/00949655.2014.926899) "Estimating Heston's and Bates’ models parameters using Markov chain Monte Carlo simulation".

There are two implementations: pure Python and cythonized Python:

**1. Pure Python:** the demo in [demo.ipynb](https://github.com/Imlerith/Jump-Diffusion-Calibrator/blob/master/demo.ipynb) shows that it takes approximately 27 minutes to calibrate the Heston model with 10,000 MCMC steps and 69 minutes to calibrate the Bates model with the same number of steps.

**2. Cythonized Python:** the demo in [demo_cythonized.ipynb](https://github.com/Imlerith/Jump-Diffusion-Calibrator/blob/master/demo_cythonized.ipynb) shows that it takes approximately 2.4 minutes to calibrate the Heston model with 10,000 MCMC steps, that is, **11x speed-up** is achieved.
