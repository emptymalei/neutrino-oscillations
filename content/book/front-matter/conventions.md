---
title: "Conventions"
description: "Conventions"
lead: ""
date: 2020-12-27
lastmod: 2020-12-27
draft: false
images: []
menu:
  book:
    parent: "Appendices"
weight: 910
toc: true
---


## Notations

- Variables with sans-serif fonts are matrices.
- Variables in bold are vectors in space-time.
- Variables with arrows are vectors in flavor-isospin space.


## Terms


- Normal hierarchy for two-flavor scenario is always defined as $m_2^2-m_1^2>0$, i.e., $\omega_{\mathrm v}>0$.
- Inverted hierarchy for two-flavor scenario is defined as $m_2^2-m_1^2<0$, i.e., $\omega_{\mathrm v}<0$.
- Solar neutrino mass splitting is $\delta m_{12}$, while atmospheric neutrino mass splitting refers to $\delta m_{23}$.


## Units


Natural units system makes the calculations of neutrinos convenient. By definition, we set reduced Planck constant and speed of light to be 1, $\hbar = 1 = c$.
The conversion between natural units and SI can be down by using the following relations,
{{<m>}}
\begin{align}
   1 \mathrm{GeV} &= 5.08 \times 10^{15} \mathrm {m^{-1}} \\
   1 \mathrm{GeV} &= 1.8\times 10^{-27} \mathrm{kg}
\end{align}
{{</m>}}
To convert between different physical quantities in this thesis, I always use the following tips.

- The energy-mass-momentum relations becomes $E^2 = p^2 + m^2c^2 = p^2 + m^2$. Thus mass $m$, momentum $\mathbf p$ and energy $E$ have the same dimension.
- An example of angular momentum in quantum mechanics is $L_z = m\hbar = m$ where $m$ is a quantum number. $\hbar$ is of dimension angular momentum.
- A plane wave in quantum mechanics is $\Psi = A e^{ \frac{E t - p x}{\hbar} }$. $\frac{E t - p x}{\hbar}$ should be dimensionless, which means $px$ has dimension angular momentum, which is obvious, meanwhile we notice that $E t$ also has the dimension of angular momentum. Previously we noticed momentum has the same dimension with energy, we should have time $t$ with the same dimension of length $x$. Also we can conclude that length and time have the same dimension as $1/E$.




## Pauli Matrices and Rotations


Given a rotation
{{<m>}}
\begin{equation}
   U = \begin{pmatrix} \cos \theta & \sin \theta \\ -\sin\theta & \cos \theta \end{pmatrix},
\end{equation}
{{</m>}}
its effect on Pauli matrices are
{{<m>}}
\begin{align}
      U^\dagger \sigma_3 U  &=\cos 2\theta \sigma_3 + \sin 2\theta \sigma_1 \\
  U^\dagger \sigma_1 U & = -\sin 2\theta \sigma_3 + \cos 2\theta \sigma_1.
\end{align}
{{</m>}}


## Lorentzian Distribution


Three-parameter Lorentzian function is
{{<m>}}
\begin{equation}
  f_{x_0,\sigma,A}(x)= \frac{1}{\pi} \frac{\sigma}{\sigma^2 + (x-x_0)^2},
\end{equation}
{{</m>}}
which has a width $2\gamma$.


## Fourier Series

The convention for the Fourier series used in this thesis is
{{<m>}}
\begin{equation}
\lambda(x) = \sum_{n=-\infty}^{\infty} \Lambda_n \exp\left( \frac{i2\pi n x}{X} \right) = \sum_{n=-\infty}^{\infty} \Lambda_n \exp\left( i \omega_0 n x \right),
\end{equation}
{{</m>}}
where $\omega_0 = \frac{2\pi}{X}$. The coefficients are evaluated using the orthogonal relation of exponential functions for $n\neq 0$,
{{<m>}}
\begin{align}
   \Lambda_n &= \frac{1}{X} \int_0^X \lambda(x) e^{ - i \omega_0 n x} dx \\
   & = \frac{1}{X} \left( \int_{0}^{X_1} \lambda_1 e^{ - i \omega_0 n x} dx + \int_{X_1}^{X_1+X_2} \lambda_2 e^{ - i \omega_0 n x} dx  \right) \\
   & = \frac{1}{X} \frac{X}{-i2\pi n} \left( \lambda_1 e^{-i\omega_0 n X_1} + \lambda_2 \left( e^{-i\omega_0 n X} - e^{-i\omega_0 n X_1}  \right) \right) \\
   & = \frac{i}{2\pi n} \left( -\lambda_1 + (\lambda_1 - \lambda_2) e^{-i2\pi n X_1/X} + \lambda_2 e^{-i 2\pi n} \right).
   \label{app-chap:convention-sec:fourier-series-eqn:parametric-resonance-castle-wall-fourier-coeff}
\end{align}
{{</m>}}
For $n=0$, we have
{{<m>}}
\begin{equation}
   \Lambda_0 = \frac{X_1 \lambda_1 + X_2 \lambda_2}{X}.
\end{equation}
{{</m>}}




For functions with specific parity, the Fourier series is much more simpler. I'll list below the Fourier series for even functions, since no odd functions are used in this thesis. In general the Fourier series of a periodic function defined on $\left[ -\frac{X}{2}, \frac{X}{2} \right]$ is
{{<m>}}
\begin{equation}
      \lambda(x) = \frac{a_0}{2} + \sum_{n=1}^\infty a_n \cos(n 2\pi x/X) + \sum_{n=1}^\infty b_n \sin(n 2\pi x/X),
\end{equation}
{{</m>}}
where
{{<m>}}
\begin{align}
    a_0 & = \frac{2}{X} \int^{X/2}_{-X/2} \lambda(x) d x \\
    a_n & = \frac{2}{X} \int_{-X/2}^{X/2} \lambda(x) \cos ( n2\pi x/X ) dx\\
    b_n & = \frac{2}{X} \int_{-X/2}^{X/2} \lambda(x) \sin( n 2\pi x/X ) dx.
\end{align}
{{</m>}}
For even function $\lambda(x)$, we have
{{<m>}}
\begin{equation}
      \lambda(x) = \frac{1}{2}a_0 + \sum_{n=1}^\infty a_n \cos (n 2\pi x/X).
\end{equation}
{{</m>}}


We shift the castle wall profile and make it always even so that
{{<m>}}
\begin{equation}
   \lambda(x) = \begin{cases} \lambda_2 , &\quad -\frac{X_2}{2}-\frac{X_1}{2}\le x\le -\frac{X_1}{2} \\
   \lambda_1, &\quad -\frac{X_1}{2}\le x\le \frac{X_1}{2} \\
   \lambda_2, &\quad \frac{X_1}{2}\le x\le \frac{X_1}{2}+\frac{X_2}{2}
   \end{cases}
\end{equation}
{{</m>}}
Fourier series of the profile is
{{<m>}}
\begin{equation}
   \lambda(x) = \frac{1}{2}\Lambda_0 + \sum_{q=1}^{\infty} \Lambda_q \cos\left( \frac{ 2\pi q x}{X} \right) = \frac{1}{2} \Lambda_0 + \sum_{q=1}^{\infty} \Lambda_q \cos\left( \omega_0 q x \right),
\end{equation}
{{</m>}}
where
{{<m>}}
\begin{align}
   \Lambda_0 =& \frac{2}{X} \int^{X/2}_{-X/2} \lambda(x) d x \\
    =& \frac{2}{X} \left(  \lambda_2 X_2 + \lambda_1 X_1   \right) \\
   \Lambda_q &= \frac{2}{X} \int_{-X/2}^{X/2} \lambda(x) \cos(n 2\pi x/X)dx \\
    =& \frac{2}{X} \left( \lambda_2 \int_{-X/2}^{-X_1/2} \cos(n 2\pi x/X)dx + \lambda_1 \int_{-X_1/2}^{X_1/2} \cos(n 2\pi x/X)dx \right. \\
   &\left.+ \lambda_2 \int_{X_1/2}^{X/2} \cos(n 2\pi x/X)dx \right) \\
    =& \frac{2}{q\pi} \left( \lambda_2\left( \sin(q\omega_0 X/2) - \sin(q\omega_0 X_1/2) \right) + \lambda_1 \sin( q\omega_0 X_1/2)  \right)  \\
    =& \frac{2}{q\pi} \left( \lambda_2\left( \sin(q \pi ) - \sin(q \pi X_1/X) \right) + \lambda_1 \sin( q\pi X_1/X)  \right)
\end{align}
{{</m>}}


## Jacobi-Anger expansion

One of the forms of Jacobi-Anger expansion is
{{<m>}}
\begin{equation}
    e^{i z \cos (\Phi)} = \sum_{n=-\infty}^\infty i^n J_n(z) e^{i n\Phi}.
    \label{eqn:jacobi-anger-expansion}
\end{equation}
{{</m>}}


## Bessel Functions

A special relation of Bessel function is that
{{<m>}}
\begin{equation}
  J_n(n \operatorname{sech} \alpha) \sim \frac{ e^{n(\tanh\alpha - \alpha)} }{\sqrt{ 2\pi n \tanh \alpha } }
\end{equation}
{{</m>}}
for large $n$ [^Ploumistakis2009]. As a matter of fact, for all positive $\alpha$, we always have $\tanh \alpha - \alpha < 0$.

Using this relation and defining $\operatorname{sech} \alpha = A \cos 2\theta_m$, which renders
{{<m>}}
\begin{equation}
  \alpha = 2 n \pi i + \ln \left(  \frac{ 1 \pm \sqrt{ -A^2 \cos^2 2\theta_m + 1 } }{ A\cos 2\theta_m } \right),\qquad n\in \mathrm{Integers},
  \label{eqn-width-alpha-solved}
\end{equation}
{{</m>}}
where the Mathematica code to solve it is shown below,

{{< highlight "mathematica" "linenos=table,linenostart=0" >}}
In[1]:= Solve[Exp[z] + Exp[-z]
== 2/(A Cos[2 Subscript[\[Theta], m]]), z] // FullSimplify
{{< / highlight >}}

we find out an more human readable analytical expression for the width
{{<m>}}
\begin{equation}
  \Gamma = \left\lvert 2 \hat k \tan 2\theta_m \frac{ e^{n ( \tanh \alpha - \alpha )} }{n_0 \sqrt{2\pi n_0 \tanh \alpha} } \right\rvert
\end{equation}
{{</m>}}
where $\alpha$ is solved out in \ref{eqn-width-alpha-solved}.
For small $\alpha$, we have expansions for exponential functions and hyperbolic functions $\tanh \alpha \sim \alpha - \frac{\alpha^3}{3}$,
{{<m>}}
\begin{equation}
  \Gamma \asymp 2\tan 2\theta_m \frac{ e^{n \alpha^3/3} }{\sqrt{2\pi \alpha} n_0^{3/2}  }.
\end{equation}
{{</m>}}
However, it doesn't really help that much since $n$ is large and no expansion could be done except for significantly small $\alpha$.





## Conversions in Neutrino Physics

Using natural units, length = time = 1/energy, we could rescale almost all quantities in neutrino oscillations using energy, or whatever characteristic scale we have.

We use two flavor vacuum oscillations between the two masses $m_1$ and $m_2$ as an example. The characteristic energy scale is the oscillation frequency $\omega_{v,21}$. The equation of motion
{{<m>}}
\begin{align}
   i\frac{d}{d x} \Psi = \frac{\omega_\vv}{2}(-\cos 2\theta_\vv \boldsymbol{\sigma_3} + \sin 2\theta_\vv \boldsymbol{\sigma_1}) \Psi,
\end{align}
{{</m>}}
can be rescaled using the characteristic energy scale $\omega_{v,21}$
{{<m>}}
\begin{align}
   i\frac{d}{d \hat x} \Psi = \frac{1}{2}(-\cos 2\theta_\vv \boldsymbol{\sigma_3} + \sin 2\theta_\vv \boldsymbol{\sigma_1})\Psi ,
\end{align}
{{</m>}}
where $\hat x = \omega_{v,21} x$. It is convenient for numerical calculations to convert quantities into dimensionless ones.

However, we usually discuss oscillation length in SI units for a grip of the picture. To convert from natural units to SI units, we write down the conversion here. The oscillation angular frequency is given by
{{<m>}}
\begin{align}
   \omega_{v,21} &= \frac{\delta m^2}{2E} \nonumber\\
   &=  \left(\frac{7.5\times 10^{-5}\mathrm{eV}^2}{2\times 1\mathrm{MeV}} \right) \left(\frac{\delta m^2}{7.5\times 10^{-5}\mathrm{eV}^2} \right) \frac{1\mathrm{MeV}}{E} \nonumber\\
   &= 3.75\times 10^{-11}\mathrm{eV}  \left(\frac{\delta m^2}{7.5\times 10^{-5}\mathrm{eV}^2}\right) \left(\frac{1\mathrm{MeV}}{E}\right) .
\end{align}
{{</m>}}
On the other hand, electro-volt is related to length through the useful formula
{{<m>}}
\begin{equation}
   197\mathrm{MeV}\cdot \mathrm{fm} = \hbar c = 1.
\end{equation}
{{</m>}}
Thus we have the oscillation angular frequency written as
{{<m>}}
\begin{align}
   \omega_{v,21} &= 3.75\times 10^{-11}\mathrm{eV}  \frac{\delta m^2}{7.5\times 10^{-5}\mathrm{eV}^2} \frac{1\mathrm{MeV}}{E} \nonumber\\
   &= 3.75\times 10^{-17}\mathrm{MeV}  \frac{\delta m^2}{7.5\times 10^{-5}\mathrm{eV}^2} \frac{1\mathrm{MeV}}{E}\nonumber \\
   &= 1.90\times 10^{-4}  \mathrm{m}^{-1}  \frac{\delta m^2}{7.5\times 10^{-5}\mathrm{eV}^2} \frac{1\mathrm{MeV}}{E}.
   \label{common-sense-eqn-omega-v-si-unit}
\end{align}
{{</m>}}
Similarly for $\delta m_{32}=2.4\times 10^{-3}\mathrm{eV^2}$ the frequency is
{{<m>}}
\begin{align}
   \omega_{v,32} =\frac{\delta m^2_{32}}{2E} = 6.3\times 10^{-3} \mathrm{m}^{-1}  \frac{\delta m^2_{32}}{2.5\times 10^{-3} \mathrm{eV}^2 } \frac{1MeV}{E}.
\end{align}
{{</m>}}
With the results for angular frequencies, the rescaled length $\hat x$ is restored using
{{<m>}}
\begin{align}
    x = \frac{\hat x}{\omega_\vv} &= \frac{\hat x}{  1.90\times 10^{-4}  \mathrm{m}^{-1}  \frac{\delta m^2}{7.5\times 10^{-5}\mathrm{eV}^2} \frac{1\mathrm{MeV}}{E} } \\
    &= \frac{\hat x}{0.190} \mathrm{km} \frac{7.5\times 10^{-5}\mathrm{eV}^2}{\delta m^2}  \frac{E}{1\mathrm{MeV}}.
\end{align}
{{</m>}}


Another important example is the 2 flavor neutrino oscillations in constant matter background potential $\lambda_c = \sqrt{2}G_{\mathrm F} n_e$. The characteristic energy scale is $\omega_m$ which is calculated using
{{<m>}}
\begin{equation}
   \omega_m = \omega_\vv \sqrt{ \frac{\lambda_c}{\omega_\vv}^2 + 1 - 2 \frac{\lambda_c}{\omega_\vv}\cos 2\theta_\vv }.
   \label{common-sense-eqn-omega-m}
\end{equation}
{{</m>}}
Meanwhile, the effective mixing angle $\theta_m$ is determined by
{{<m>}}
\begin{equation}
   \tan 2\theta_m = \frac{\sin 2\theta_\vv}{\cos 2\theta_\vv - \frac{\lambda}{\omega_\vv} }.
\end{equation}
{{</m>}}
Similar to vacuum equation of motion, we rescale the equation of motion in constant background using $\omega_m$
{{<m>}}
\begin{equation}
   i \frac{d}{d\hat x} \Psi = \frac{1}{2}(-\cos 2\theta_m \boldsymbol{\sigma_3} + \sin 2\theta_m \boldsymbol{\sigma_1})\Psi ,
\end{equation}
{{</m>}}
we find out the scaled distance
{{<m>}}
\begin{equation}
   \hat x = \omega_m x.
\end{equation}
{{</m>}}
To reverse the process and find out the actual SI unit distance after the numerical calculation, we use
{{<m>}}
\begin{equation}
   x = \frac{\hat x}{\omega_m}.
   \label{common-sense-eqn-actual-distance-constant-matter}
\end{equation}
{{</m>}}
The procedure will be the following.

- Calculate $\omega_\vv$ using Eq.~\ref{common-sense-eqn-omega-v-si-unit}.
- Calculate $\hat\lambda_c = \frac{\lambda_c}{\omega_\vv}$.
- Calculate $\omega_m$ using Eq.~\ref{common-sense-eqn-omega-m}.
- Find out the actual distance using Eq.~ \ref{common-sense-eqn-actual-distance-constant-matter}.



[^Ploumistakis2009]: {{< cite key="Ploumistakis2009">}}