# Computation Through Dynamics

This repository contains a number of subprojects related to the
interlinking of computation and dynamics in artificial and biological
neural systems. 

This is not an officially supported Google product.


## Prerequisites

The code is written in Python 2.7.13. You will also need:

* **JAX** version 1.1.18 ([install](https://github.com/google/jax#installation)) -
* **NumPy, SciPy, Matplotlib** ([install SciPy stack](https://www.scipy.org/install.html), contains all of them)
* **h5py** ([install](https://pypi.python.org/pypi/h5py))


## LFADS - Latent Factor Analysis via Dynamics Systems

LFADS is a tool for inferring dynamics from noisy, high-dimensional observations
of a dynamics system.  It is a sequential auto-encoder with some very particular
bells and whistles.  Here we have released a tutorial version, written in
*Python / Numpy / JAX* intentionally implemented with readabilily, comprehension and
innovation in mind. You may find the full TensorFlow implementation with run manager 
support ([here] (https://github.com/lfads)).

## Integrator RNN - Train a Vanilla RNN to integrate white noise.
Integration is a very simple task and highlights how to set up a loop over time,
batch over multiple input/target examples, use just-in-time compilation to speed
the computation up, and take a gradient in *JAX*.  The data from this example is
also used as input for the LFADS tutorial.
