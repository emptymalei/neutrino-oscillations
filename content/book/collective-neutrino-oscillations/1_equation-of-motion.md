---
title: "Equation of Motion"
description: "Equation of Motion"
lead: ""
date: 2020-04-20T11:53:07+02:00
lastmod: 2020-04-20T11:53:07+02:00
draft: false
menu:
  book:
    parent: "4. Collective Neutrino Oscillations"
images: []
weight: 410
toc: false
---


The equation of motion for neutrino oscillations with self-interaction is [^Sigl1993]
{{<m>}}
\begin{equation}
   \ri \frac{\dd}{\dd t}\rho = [ \mathsf H,\rho],
   \label{chap:collective-sec:collective-eqn:equation-of-motion-general}
\end{equation}
{{</m>}}
where the total derivative is
{{<m>}}
\begin{equation}
   \frac{\dd}{\dd t} = \partial_t + \mathbf v\cdot \boldsymbol{\nabla},
\end{equation}
{{</m>}}
and the Hamiltonian is composed of three different terms:
{{<m>}}
\begin{equation}
   \mathsf H = \mathsf H_{\mathrm v} +\mathsf  H_{\nu\nu}.
\end{equation}
{{</m>}}
In the above equation, the vacuum Hamiltonian is
{{<m>}}
\begin{align*}
    \mathsf H_\vv =& \begin{cases}
    -\frac{1}{2}\eta \omega_\vv \sigma_3 & \text{for neutrinos},\\
    \frac{1}{2}\eta \omega_\vv \sigma_3 & \text{for antineutrinos},
    \end{cases}
\end{align*}
{{</m>}}
where $\eta = +1$ for the normal neutrino mass hierarchy and $-1$ for the inverted neutrino mass hierarchy, $\omega_\vv$ is the vacuum oscillation frequency of the neutrino or antineutrino.
The neutrino self-interaction is more complicated and can be written as
{{<m>}}
\begin{equation}
    \mathsf H_{\nu\nu} = \sqrt{2}G_{\mathrm F} \int \frac{E'^2\dd E'}{8\pi^3} \dd\Gamma_{\mathbf v'} \left[ n(E',\mathbf v')\rho(E',\mathbf v') - \bar n(E',\mathbf v')\bar\rho(E',\mathbf v') \right] (1-\mathbf v \cdot \mathbf v'),
    \label{chap:collective-sec:collective-eqn:equation-of-motion-self-interaction}
\end{equation}
{{</m>}}
where $\dd \Gamma_\nu$ is the differential solid angle, $n(E,\mathbf v)$ and $\rho(E, \mathbf v)$ are the number density and the flavor density matrix of the neutrino with energy $E$ and velocity $\mathbf v$, and $\bar n(E, \mathbf v)$ and $\bar \rho(E,\mathbf v)$ are the corresponding quantities of the antineutrino.

The presence of the neutrino self-interaction potential makes the equation of motion \eqref{chap:collective-sec:collective-eqn:equation-of-motion-general} nonlinear, and many interesting phenomena arise because of it. For example, a dense neutrino medium can experience synchronized oscillations during which all the neutrinos and antineutrinos oscillate with the same frequency [^Pastor2002] [^Hannestad2006] [^Raffelt2008] [^Duan2010]. To see this, I will consider an isotropic and homogeneous neutrino gas and use the flavor isospin picture discussed in Sec. [Flavor Isospin Formalism](/book/principles-of-neutrino-oscillations/flavor-isospin-formalism/). The flavor isospin $\vec s$ of the neutrino is defined by
{{<m>}}
\begin{equation}
   \rho = \frac{1}{2} + \vec s \cdot \vec \sigma.
\end{equation}
{{</m>}}
The equation of motion of the flavor isospin is
{{<m>}}
\begin{equation}
    \dot{\vec s} = \vec s \times \left(\vec H_\vv + \vec H_{\nu\nu} \right),
    \label{chap:collective-eqn:flavor-isospin-eom}
\end{equation}
{{</m>}}
where
{{<m>}}
\begin{equation}
   \vec H_{\mathrm v} =  \omega_{\mathrm v}\begin{pmatrix}
   -\sin 2\theta_{\mathrm v}\\
   0 \\
   \cos 2\theta_{\mathrm v}
   \end{pmatrix} = \omega_\vv \vec B,
\end{equation}
{{</m>}}
and
{{<m>}}
\begin{equation}
\vec H_{\nu\nu} = \frac{\sqrt{2}G_{\mathrm F}}{2\pi^2} \int E'^2\dd E' n(E') \vec s(E').
\end{equation}
{{</m>}}
Here for simplicity I have assumed $n_{\mathrm e}=0$ and $\bar n=0$. When the neutrino density is very large, $\vec H_{\nu\nu}$ dominates over $\vec H_\vv$ in Eqn.~\eqref{chap:collective-eqn:flavor-isospin-eom}, and $\vec s$ precesses about $\vec H_{\nu\nu}$ rapidly. Meanwhile, the total flavor isospin
{{<m>}}
\begin{equation}
    \vec S = \int \dd E' f(E') \vec s(E')
\end{equation}
{{</m>}}
precesses about $\vec H_\vv$ slowly with a mean oscillation frequency $\langle \omega_\vv \rangle$, where
{{<m>}}
\begin{equation}
    f(E) = \frac{ E^2 n(E) }{ \int E'^2 \dd E' n(E') }
\end{equation}
{{</m>}}
is the energy distribution of the neutrino. To see this, one can multiply Eqn.~\eqref{chap:collective-eqn:flavor-isospin-eom} by $f(E)$ and integrate over $E$ which gives
{{<m>}}
\begin{align}
    \dot{\vec S} &= \int \dd E f(E)\vec s(E) \times \omega_\vv \vec B \\
    &\to \int \dd E f(E) \left[ \frac{\vec s(E) \cdot \vec S}{ \lvert \vec S \rvert^2 } \vec S \right] \times \omega_\vv \vec B \\
    &= \langle \omega_\vv \rangle \vec S \times \vec B,
\end{align}
{{</m>}}
where
{{<m>}}
\begin{equation}
    \langle \omega_\vv \rangle  = \int \dd E f(E) \left[ \frac{\vec s(E) \cdot \vec S}{ \lvert \vec S \rvert^2 } \right] \omega_\vv.
\end{equation}
{{</m>}}
In the above equation I have replaced flavor isospin $\vec s$ with its projection along the direction of $\vec S$ because its precession about $\vec S$ is much faster than the precession of $\vec S$ about $\vec B$.


[^Sigl1993]: {{<ref key="Sigl1993">}}
[^Pastor2002]: {{<ref key="Pastor2002">}}
[^Hannestad2006]: {{<ref key="Hannestad2006">}}
[^Raffelt2008]: {{<ref key="Raffelt2008">}}
[^Duan2010]: {{<ref key="Duan2010">}}