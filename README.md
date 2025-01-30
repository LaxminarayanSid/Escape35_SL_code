This repository contains the code which can generate the figures shown in the paper.
The code explores additional extrapolation scenarios other than the ones presented in the paper.
The following extrapolative scenarios are tested:
  1. Batch extrapolation - Different initial conditions outside of the initial training space for a batch bioprocess for a 200 hr time period
  2. Semi-Batch extrapolation - Different initial conditions outside of the initial training space for a semi batch bioprocess for a 200 hr time period

The following libraries are required to run the code:
  1. Scikit learn
  2. Numpy
  3. Scipy
  4. Pyomo
  5. Ipopt optimization solver
  6. Tensor flow
  7. Captum
  8. Matplotlib

Each code file corresponds to an image and analysis performed in the results and discussion section:
 1. **Integrated_vs_Sequential** : This jupyter notebook compares the performance of the integrated hybrid model and the sequential hybrid model.
 2. **Hybrid_Phenom_ML** : This jupyter notebook compares the performance of the best hybrid model (integrated hybrid model) with the performance of a phenemnological model and a machnine learning model. This file especially focuses on the case study where the maintenance-consumption of glucose is negligble.
 3. **Hybrid_Phenom_ML_high_maintenance** : This jupyter notebook compares the performance of the best hybrid model against phenmenological and machine learning model. This notebook focuses on the case stufy where the maintenance-consumption of glucose is high and comparable to the growth-consumption of glucose
 4. **Hybrid_Interpretability** : This jupyter notebook utilizes the Captum package to analyze the ANN models that are embedded within the integrated hybrid models. The code gives us physical insight about how the ANN output is impacted by the ANN input
 5. **Improved_hybrid_model** : This jupyter notebook uses the physical insight from the previous notebook to create an improved hybrid model. The performance of the original hybrid model is compared to the improved hybrid model.

