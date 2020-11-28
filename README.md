# tf-optim: Barebones optimization of functions using tf.optimizers

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/lazyoracle/tf-optim/HEAD)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lazyoracle/tf-optim/blob/main/example.ipynb)

Have you wondered how well the optimizers used for training Machine Learning models perform on other optimization tasks? Have you been intrigued by all the hype around ADAM, RMSProp, SGD etc? 
Do you want to see if the *momentum* that ML folks talk about helps your optimization problems as well?

Well, fret not, because Tensorflow has a very robust suite of Optimizers under the `tf.keras.optimmizers` suite that have battle-tested for the toughest of ML training scenarios.

Only problem, the API is designed to only make sense for use in ML applications (Who uses a global variable and Why? Why can't I just pass a parameterised function?)

This is an effort to demonstrate how to write functions that could be fed to the `tf.keras.optimmizers`, so we essentially make wrappers around the function you wish to optimize instead 
of wrapping TF APIs.
