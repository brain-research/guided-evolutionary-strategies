# Guided Evolutionary Strategies

### Escaping the curse of dimensionality in random search

## Overview

Many applications in machine learning require optimizing a function whose true
gradient is unknown, but where surrogate gradient information (directions that
may be correlated with, but not necessarily identical to, the true gradient) is
available instead. This arises when an approximate gradient is easier to compute
than the full gradient (e.g. in meta-learning or unrolled optimization), or when
a true gradient is intractable and is replaced with a surrogate (e.g. in certain
reinforcement learning applications, or when using synthetic gradients).

Here, we propose _Guided Evolutionary Strategies_, a method for optimally using
surrogate gradient directions along with random search. We define a search
distribution for evolutionary strategies that is elongated along a guiding
subspace spanned by the surrogate gradients. This allows us to estimate a
descent direction which can then be passed to a first-order optimizer.

This repository contains a colaboratory (colab) notebook with a demo of the
method on a toy problem.

## Contact

Authors:

-   Niru Maheswaranathan (nirum@google.com)
-   Luke Metz (lmetz@google.com)
-   George Tucker (gjt@google.com)
-   Jascha Sohl-Dickstein (jaschasd@google.com)

This is not an officially supported Google product.
