# Revisiting Solution Techniques for Indirect Low-Thrust Trajectory Optimization

This repository contains the code and numerical examples accompanying the paper **“Revisiting Solution Techniques for Indirect Low-Thrust Trajectory Optimization.”**

The examples are organized according to the three solution techniques investigated in the paper:

- `technique1/` — **SIMD-accelerated forward–backward shooting**  
  Includes Cases 1 and 2, with comparisons among single shooting, forward–forward shooting, forward–backward shooting, and SIMD-accelerated forward–backward shooting.

- `technique2/` — **Augmented shooting with embedded smoothing homotopy**  
  Includes Cases 1 and 3, with comparisons among direct shooting, stepwise homotopy, ungated augmentation, and residual-gated augmented shooting.

- `technique3/` — **Equivalent reachability formulations**  
  Includes Cases 1 and 4, with comparisons between the minimum-required-thrust and maximum-initial-mass formulations.

Each case is provided as a Jupyter notebook with saved outputs, so the numerical results can be inspected without rerunning the full computation.

## Environment

The code was tested with:

- Python 3.12
- NumPy 2.5.3
- SciPy 1.18.0
- heyoka 7.12.1
- IPython 9.17.1

Runtime measurements reported in the notebooks use the native `%%timeit` command with seven serial repeats. Integrators are constructed beforehand and are therefore excluded from the reported timing measurements.

## Dynamics Files

The notebooks include saved outputs for inspecting the numerical results. Rerunning the full computations, however, requires additional dynamics files that are not currently included in this repository.

To request these files, please contact [zhongzhang.astro@gmail.com](mailto:zhongzhang.astro@gmail.com) and include your **name** and **affiliation** in the email.

The required dynamics files and additional supporting materials will be released progressively after the paper is published.

## Citation

If you find this work useful, we would appreciate it if you cite our paper:

```bibtex
@article{zhang2026revisiting,
  title   = {Revisiting Solution Techniques for Indirect Low-Thrust Trajectory Optimization},
  author  = {Zhang, Zhong and Yang, Jia and Jiang, Fanghua and Izzo, Dario and Topputo, Francesco},
  journal = {Journal of Guidance, Control, and Dynamics},
  year    = {2026},
  note    = {To appear}
}
```

The citation information will be updated once the paper is published.
