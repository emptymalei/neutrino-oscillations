---
title: "Neutrino Interaction with Matter"
description: "Neutrino Interaction with Matter"
lead: ""
date: 2020-12-27
lastmod: 2020-12-27
draft: false
images: []
menu:
  book:
    parent: "Appendices"
weight: 920
toc: true
---


## Flavor Basis

In terms of formalism, vacuum oscillations is already a Rabi oscillation at resonance with oscillation width $\omega_\vv \sin 2\theta_\vv$. As derived, neutrino oscillations in matter are determined by Hamiltonian in flavor basis
{{<m>}}
\begin{equation}
      H^{(\ff)} = \left(- \frac{1}{2} \omega_\vv \cos 2\theta_\vv +\frac{1}{2}\lambda(x)  \right)\sigma_3 + \frac{1}{2} \omega_\vv \sin 2\theta_\vv \sigma_1,
\end{equation}
{{</m>}}
with the Schröding equation
{{<m>}}
\begin{equation}
    i \partial_x \Psi^{(\ff)} = H^{(\ff)} \Psi^{(\ff)}.
\end{equation}
{{</m>}}
To make connections to Rabi oscillations, we would like to remove the changing $\sigma_3$ terms, using a transformation
{{<m>}}
\begin{equation}
    U = \begin{pmatrix} e^{-i \eta (x)} & 0 \\  0 & e^{i \eta (x)}  \end{pmatrix},
\end{equation}
{{</m>}}
which transform the flavor basis to another basis
{{<m>}}
\begin{equation}
    \begin{pmatrix} \psi_e \\ \psi_x \end{pmatrix} = \begin{pmatrix} e^{-i \eta (x)} & 0 \\  0 & e^{i \eta (x)}  \end{pmatrix} \begin{pmatrix} \psi_{a} \\ \psi_{b} \end{pmatrix}.
\end{equation}
{{</m>}}
The Schrodinger equation can be written into this new basis
{{<m>}}
\begin{equation}
    i \partial_x (T \Psi^{(r)}) = H^{(\ff)} T\Psi^{(r)},
\end{equation}
{{</m>}}
which is simplified to
{{<m>}}
\begin{equation}
    i \partial_x \Psi^{(r)} = H^{(r)} \Psi^{(r)},
\end{equation}
{{</m>}}
where
{{<m>}}
\begin{equation}
 H^{(r)} = - \frac{1}{2}\omega_\vv \cos 2\theta_\vv \sigma_3 + \frac{1}{2} \omega_\vv \sin 2\theta_\vv \begin{pmatrix}
   0 & e^{2i\eta(x)} \\
   e^{-2i\eta(x)} & 0 \\
   \end{pmatrix},
\end{equation}
{{</m>}}
in which we remove the varying component of $\sigma_3$ elements using
{{<m>}}
\begin{equation}
    \frac{d}{dx}\eta(x) = \frac{\lambda(x)}{2}.
\end{equation}
{{</m>}}
The final Hamiltonian would have some form
{{<m>}}
\begin{equation}
     H^{(r)} = - \frac{1}{2}\omega_\vv \cos 2\theta_\vv \sigma_3 + \frac{1}{2} \omega_\vv \sin 2\theta_\vv \begin{pmatrix}
   0 & e^{i\int_0^x \lambda(\tau)d\tau + 2i\eta(0)} \\
   e^{-i\int_0^x \lambda(\tau)d\tau - 2i\eta(0)} & 0 \\
   \end{pmatrix},
\end{equation}
{{</m>}}
where $\eta(0)$ is chosen to counter the constant terms from the integral.

For arbitrary matter profile, we could first apply Fourier expand the profile into trig function then use Jacobi-Anger expansion so that the system becomes a lot of Rabi oscillations.
Any transformations or expansions that decompose $\exp{\left(i\int_0^x \lambda(\tau)d\tau\right)}$ into many summations of $\exp{\left( i a x + b \right)}$ would be enough for an Rabi oscillation interpretation.
As for constant matter profile, $\lambda(x) = \lambda_0$, we have
{{<m>}}
\begin{equation}
     \eta(x) = \frac{1}{2} \lambda_0 x.
\end{equation}
{{</m>}}
The Hamiltonian becomes
{{<m>}}
\begin{equation}
     H^{(r)} = - \frac{1}{2}\omega_\vv \cos 2\theta_\vv \sigma_3 + \frac{1}{2} \omega_\vv \sin 2\theta_\vv \begin{pmatrix}
   0 & e^{i\lambda_0 x} \\
   e^{-i\lambda_0 x} & 0 \\
   \end{pmatrix},
\end{equation}
{{</m>}}
which is exactly a Rabi oscillation. The resonance condition is
{{<m>}}
\begin{equation}
   \lambda_0 = \omega_\vv \cos 2\theta_v.
\end{equation}
{{</m>}}





## Instantaneous Matter Basis


Neutrino oscillations can be calculated in instantaneous matter basis, where the Schrödinger equation is transformed to instantaneous matter basis by applying a rotation $U$,
{{<m>}}
\begin{equation}
    i \partial_x \left(  U\Psi^{(\mm)} \right)= H^{(\ff)} U\Psi^{(\mm)},
\end{equation}
{{</m>}}
where
{{<m>}}
\begin{equation}
    U = \begin{pmatrix} \cos \theta_m & \sin \theta_m \\ -\sin\theta_m & \cos \theta_m \end{pmatrix}.
\end{equation}
{{</m>}}
With some simple algebra, we can write the system into
{{<m>}}
\begin{equation}
    i \partial _x \Psi^{(\mm)} = H^{(\mm)}\Psi^{(\mm)} ,
\end{equation}
{{</m>}}
where
{{<m>}}
\begin{equation}
    H^{(\mm)} = U^\dagger H^{(\ff)} U - i U^\dagger \partial_x U.
\end{equation}
{{</m>}}
By setting the off-diagonal elements of the first term $U^\dagger H^{(\ff)} U$ to zero, we can derive the relation
{{<m>}}
\begin{equation}
   \tan 2\theta_m = \frac{\sin 2\theta_\vv}{\cos 2\theta_\vv - \lambda/\omega_\vv}.
\end{equation}
{{</m>}}
Furthermore, we derive the term
{{<m>}}
\begin{equation}
    i U^\dagger \partial_x U = - \dot\theta_m \sigma_2.
\end{equation}
{{</m>}}
We can calculate $\dot\theta_m$ by taking the derivative of $\tan 2\theta_m$,
{{<m>}}
\begin{equation}
    \frac{d}{dx} \tan 2\theta_m = \frac{2}{\cos^2 2\theta_m} \dot\theta_m,
\end{equation}
{{</m>}}
so that
{{<m>}}
\begin{align}
    \dot\theta_m &= \frac{1}{2} \cos^2 (2\theta_m) \frac{d}{dx} \tan 2\theta_m \\
   & = \frac{1}{2} \frac{(\cos 2\theta_\vv - \lambda/\omega_v)^2}{ (\lambda/\omega_v)^2 + 1 - 2\lambda \cos 2\theta_\vv /\omega_\vv } \frac{d}{dx} \frac{\sin 2\theta_\vv}{\cos 2\theta_\vv - \lambda/\omega_\vv} \\
   & = \frac{1}{2} \frac{(\cos 2\theta_\vv - \lambda/\omega_v)^2}{ (\lambda/\omega_v)^2 + 1 - 2\lambda \cos 2\theta_\vv /\omega_\vv }  \frac{\sin 2\theta_\vv}{(\cos 2\theta_\vv - \lambda/\omega_v)^2} \frac{1}{\omega)v} \frac{d}{dx} \lambda(x) \\
   & = \frac{1}{2} \sin 2\theta_m \frac{1}{\omega_m} \frac{d}{dx} \lambda(x).
\end{align}
{{</m>}}





