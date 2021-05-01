# Various Particle Physics and Machine Learning TikZ diagrams

This repository contains various Tikz diagrams I made for my publications and
presentations. Both the LaTeX source code and a compiled version (.pdf) of all
diagrams is included. A table of contents of all diagrams in this repository
can be found below.

---

## How to compile the figures

By default command to compile the TikZ figures is `pdflatex`. Compiling the
neural network diagram `nn.tex` can thus be done through

    pdflatex nn.tex

This creates, amongst a .log and .aux-file also a .pdf-file containing the
diagram.

A notable exception to the use of `pdflatex` is the Feynman diagram file, which
needs to be compiled with `lualatex`.

---

## Can I use these figures? For realz?

I have made the figures and source code available under the MIT license,
meaning you are free to download, modify and distribute the diagrams yourself.
You *do* need to include the original copyright notice, however.

---

## Table of contents

- **active learning**
  - `active_learning_workflow.pdf`: Simple diagram showing a possible workflow
    for active learning.
  - `normal_sampling.pdf`: Depiction of a normal sampling procedure in which
    the oracle is explicitly named as such. Makes comparison to the pool-based
    active learning diagrams possible.
  - `pool_based_sampling_finite.pdf`: Depiction of the pool-based sampling
    approach for active learning with a finite pool.
  - `pool_based_sampling_finite.pdf`: Depiction of the pool-based sampling
    approach for active learning with an infinite pool.
- **decision trees**
  - `boosted_decision_trees.pdf`: Diagram depicting the creation process of a
    Boosted Decision Trees model.
  - `decision_tree.pdf`: A simple decision tree consisting out of just a couple
    of splitting nodes. The prediction map of this tree can be found in
    `decision_tree_prediction_map.pdf`.
  - `decision_tree_prediction_map.pdf`: The prediction map of the decision tree
    shown in `decision_tree.pdf`.
- **neural network architectures**
  - `autoencoder.pdf`: Example of an autoencoder neural network architecture .
  - `ffnn_with_biases.pdf`: Visualisation of a standard feedfoward neural
    network consisting out of two hidden layers. Biases are explicitly included
    in this diagram.
  - `ffnn.pdf`: An as simple as possible diagram of a feedforward neural
    network (2 hidden layers).
  - `gan.pdf`: Diagram showing the two different networks in a Generative
    Adversarial Network and their different tasks. The training feedback loop
    is not included in this figure.
  - `made.pdf`: Example of the network architecture needed for a Masked
    Autoencoder for Distribution Estimation (ensuring that the autoregressive
    property is adhered to).
  - `vae.pdf`: Architecture for a Variational Autoencoder. It is instructional
    to compare this diagram to `autoencoder.pdf`.
- **normalising flows**
  - `normalising_flow.pdf`: Basic visualisation of a normalising flow.
  - bijectors
    - `iaf_forward.pdf`: Forward pass through an Inverse Autoregressive Flow
      with a simple affine transformation.
    - `iaf_inverse.pdf`: Inverse pass through an Inverse Autoregressive Flow
      with a simple affine transformation.
    - `maf_forward.pdf`: Forward pass through a Masked Autoregressive Flow with
      a simple affine transformation.
    - `maf_inverse.pdf`: Inverse pass through a Masked Autoregressive Flow
      with a simple affine transformation.
    - `piecewise_linear_spline.pdf`: Diagram showing the construction of a
      piecewise linear spline.
    - `piecewise_quadratic_spline.pdf`: Diagram showing part of the
      construction of a piecewise quadratic spline (I have not yet taken the
      time to code quadratic curves...).
    - `rational_quadratic_spline`: Diagram showing the construction and use of
      a rational quadratic spline.
    - `realnvp.pdf`: Diagram showing the splitting of features in a RealNVP
      transformation (as for *any* coupling transform) and the subsequent
      dependencies on the transformation functions.
- **parameter spaces**
  - `slicing.pdf`: Visualisation of what a 'slice' of a parameter space is, and
    that knowledge of a specific function on that slice doesn't tell you
    anything about that function outside of that slice. The diagram shown on
    the slice originates from [arxiv:2004.10894](https://arxiv.org/abs/2004.10894).
- **particle physics**
  - `analysis.pdf`: Schematic outline of what a particle physics analysis
    typically entails.
  - `feynman_diagram.pdf`: Example of a Feynman diagram, showing the
    annihilation and creation of a particle pair. *Compiling this diagram 
    requires the use of `lualatex`*.
  - `standard_model.pdf`: Particle content of the Standard Model.