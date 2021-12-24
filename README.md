# bandlimited-quadratures
Notebooks demonstrating bandlimited quadrature construction

These notebooks contain Julia examples of how to build quadratures for bandlimited functions using the method from "On Generalized Gaussian Quadratures for Bandlimited Exponentials" by Matthew Reynolds, Gregory Beylkin, and Lucas Monzon (2013). Right now, the examples are restricted to the uniform weight function w(x)=1 on the interval [-1,1]. However, this method was demonstrated (in the paper above) capabable of generating quadratures for different weight functions, even non-sign definite examples. 

There are currently two notebooks. The bandlimited_quadratures.ipynb notebook containw examples using double precision computations, capable of generating quadratures with a litte more than single precision accuracy. bandlimited_quadratures_high_precision.ipynb uses Julia's BigFloat capability to compute higher accuracy quadratures (even past double precision), but at a significant cost in terms of speed. If the user's goal is to generate quadratures with double precision accuracy, and speed is an important factor, the user should consider using libraries capable of quad precision computations.
