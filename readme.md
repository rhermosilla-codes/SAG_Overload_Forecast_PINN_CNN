# SAG's Overload Forecasting Using A CNN Physical Informed Approach

This directory contains the implementation of CNN-PINN model to forecast or predict the ocurrence of overload in SAG Mills. The datasets that underpin the experiments validating our architectural proposition originate from the SAG-5 mill at Minera La Escondida (BHP Billiton). This data, authorized for use by the company, encompasses the operational records from August 2018 to July 2019. The comprehensive dataset comprises 696,356 instances across more than 40 operational features. Out of the extensive feature set, 10 were identified as particularly relevant for overload prediction: returned pebble count, fine granulometry, medium granulometry, coarse granulometry, mill power, mill pressure, solid percentage, throughput and mill speed.

# Requeriments

Our experiments used authorized data from La Escondida Mine (BHP Groups). If you need the original data, you need to provide us with an express authorization from the mine to request it. You can request the original data (attaching a checkable authorization) to rodrigo.hermosilla@sansano.usm.cl. Anyway, you can find the scaled data in our repository for reproducibility of our experiments.


# Files

/code/

** cnn_pinn_overload_detection.ipynb**: notebook with the entire process of training and test of the model. This model includes metrics functions to meausure the efficency of the results.

/output/

** cnn_pinn_overload_detection.html**: hypertext file with the executed notebook.

/data/

** matrices.npz **: Compressed file containing temporal matrices (X) and their corresponding targets (y). The matrix X is scaled and has a shape of (n, 30, 8), where (30, 8) represents the size of each window with 30 time steps and eight features per step.


## Citation

```latex
@misc{hermosilla2024sagoverload,
  author = {Hermosilla, R., Valle, C.},
  title = {SAG\'s Overload Forecasting Using A CNN Physical Informed Approach},
  year = {2024},
  url = {https://github.com/username/repository](https://github.com/rhermosilla-codes/SAG_Overload_Forecast_PINN_CNN/)},
  note = {Version 1.0, commit hash: abcdef1234567890abcdef1234567890abcdef12}
}

<b>Soon, you will find a way to cite our last paper here.</b>
