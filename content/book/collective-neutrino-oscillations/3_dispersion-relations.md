---
title: "Dispersion Relations"
description: "Dispersion Relations"
lead: ""
date: 2020-04-20T11:53:07+02:00
lastmod: 2020-04-20T11:53:07+02:00
draft: false
menu:
  book:
    parent: "4. Collective Neutrino Oscillations"
images: []
weight: 430
toc: false
---

In the two-beam model, I have assumed the neutrino flavor density matrix $\rho(z)$ depends on $z$ only. For the neutrino medium in a real physical environment, $\rho(t,\mathbf r)$ is a function of both time $t$ and spatial coordinate $\mathbf r$. The collective mode $a$ of neutrino oscillations takes the form
{{<m>}}
\begin{equation}
    \epsilon_i(t,\mathbf r) = Q_{i}^{(a)} e^{\ri (\Omega_a t - \mathbf K_a \cdot \mathbf r) }
    \label{chap:collective-sec:dispersion-relation-eqn:collective-mode-epsilon}
\end{equation}
{{</m>}}
where index $i$ denotes the species and the propagation direction of the neutrino, and $\Omega_a$ and $\mathbf K_a$ are the oscillation frequency and wavevector of the corresponding collective mode, respectively.  In this section, I will review the dispersion relations between $\Omega_a$ and $\mathbf K_a$ discussed by I. Izaguirre, G. Raffelt, and I. Tamborra in reference [^Izaguirre2016a].

The equation of motion for the flavor transformation of a dense neutrino medium in flavor basis is
{{<m>}}
\begin{equation}
\ii (\partial_t + \mathbf v\cdot \mathbf{\nabla}) \rho = \left[ \frac{\lambda}{2} \sigma_3 + \mathsf H_{\nu\nu}, \rho \right],
\label{eqn-liouville-eqn}
\end{equation}
{{</m>}}
where I have ignored the vacuum Hamiltonian. This is because the vacuum oscillation frequency of the neutrino
{{<m>}}
\begin{align*}
 \omega_{\mathrm v} = \frac{\Delta m^2}{2E}  \sim& \frac{2\pi}{ 10  \mathrm{km} }  \left(\frac{\Delta m^2_{32}}{2.5\times 10^{-3} \mathrm{eV}^2 } \right) \left( \frac{10 \mathrm{MeV}}{E} \right) \\
\sim & \frac{2\pi}{ 330  \mathrm{km} } \left( \frac{\Delta m_{12}^2}{7.5\times 10^{-5}\mathrm{eV}^2} \right) \left( \frac{10 \mathrm{MeV}}{E} \right)
\end{align*}
{{</m>}}
is much smaller than the neutrino potential
{{<m>}}
\begin{equation*}
\mu = \sqrt{2}G_{\mathrm F} n \sim  \frac{1}{0.01 \mathrm{km}} \left(\frac{100\mathrm{km}}{R}\right)^2 \left(\frac{1\mathrm{MeV}}{E}\right) \left( \frac{ L }{ 10^{50}\mathrm{erg\cdot s^{-1}} } \right),
\end{equation*}
{{</m>}}
where $E$ is the typical energy of the supernova neutrino, $n$ is the total number density of the neutrino, $R$ is the distance from the center of the supernova, and $L$ is the total luminosity of the neutrino.
In Eqn.~\eqref{eqn-liouville-eqn},
{{<m>}}
\begin{equation}
\mathsf H_{\nu\nu} = \sqrt{2} G_{\mathrm F} \iint \dd \Gamma' v^\mu v'_\mu \int \frac{E'^2 \mathrm d E'}{8\pi^3} \left( (n_{\nu_{\mathrm e}}' - n_{\nu_{\mathrm x}}' )\rho' -  (n_{\bar\nu_{\mathrm e}}' - n_{\bar\nu_{\mathrm x}}' ) \bar\rho' \right),
\end{equation}
{{</m>}}
where
{{<m>}}
\begin{equation}
    v^\mu = (1, \mathbf v)^{\mathrm T} = ( 1, \sin\theta\cos\phi, \sin\theta\sin\phi, \cos\theta )^{\mathrm T}
\end{equation}
{{</m>}}
is the four velocity of the neutrino and the primed quantities such as $\rho'=\rho_{\mathbf v'} (t, \mathbf r)$ depend on the primed physical variable $\mathbf v'$. Without the vacuum Hamiltonian, the equation of motion for the antineutrino is the same as Eqn.~\eqref{eqn-liouville-eqn}.

In the supernova, the fluxes of non-electron-flavor neutrinos are approximately the same. It is convenient to define the electron lepton number (ELN) as [^Izaguirre2016a]
{{<m>}}
\begin{equation}
G({\mathbf v}) =  \sqrt{2}G_{\mathrm F} \int \frac{E'^2 \mathrm d E'}{8\pi^3} \left[ n_{\nu_{\mathrm e}}(\cos\theta',\phi',E')  - n_{\bar\nu_{\mathrm e}}(\cos\theta',\phi',E')  \right].
\end{equation}
{{</m>}}
I will perform the linear stability analysis as in Sec.~\ref{chap:collective-sec:two-beams}. For this purpose, I will assume that the density matrices of the neutrino and antineutrino have the form
{{<m>}}
\begin{equation}
\rho_{\mathbf v} (t,\mathbf r)   = \bar \rho_{\mathbf v}  (t,\mathbf r)  = \begin{pmatrix}
1 & \epsilon_{\mathbf v}(t,\mathbf r) \\
\epsilon^*_{\mathbf v}(t,\mathbf r) & 0
\end{pmatrix},
\end{equation}
{{</m>}}
where $\lvert \epsilon_{\mathbf v}(t,\mathbf r) \rvert \ll 1$. Plugging this into the equation of motion, I obtain the linearized equation of motion
{{<m>}}
\begin{equation}
    \ri ( \partial_t + \mathbf v \cdot \boldsymbol{\nabla} ) \epsilon = v^\mu \Phi_\mu \epsilon - \int \dd \Gamma' v^\mu v'_\mu G(\mathbf v') \epsilon',
    \label{chap:collective-sec:fast-mode-eqn:eom-continuous-general-linearized}
\end{equation}
{{</m>}}
where
{{<m>}}
\begin{equation}
    \Phi_\mu = \left( -\int \dd \Gamma' G(\mathbf v'), \int \dd \Gamma' \mathbf v' G(\mathbf v') \right)^{\mathrm T}.
\end{equation}
{{</m>}}
Assuming the solution in Eqn.~\eqref{chap:collective-sec:dispersion-relation-eqn:collective-mode-epsilon}, I obtain
{{<m>}}
\begin{equation}
    v^\mu k_\mu Q_{\mathbf v}   =  - \int \dd \Gamma' v^\mu v'_\mu G(\mathbf v')  Q_{\mathbf v'},
    \label{chap:collective-sec:dispersion-relation-eqn:eom-general-collective-modes-form}
\end{equation}
{{</m>}}
where
{{<m>}}
\begin{equation}
    k_\mu = \begin{pmatrix}
        \omega \\
        \mathbf k
    \end{pmatrix} = \begin{pmatrix}
        \Omega - \Phi_0 \\
        \mathbf K - \boldsymbol{\Phi}
    \end{pmatrix}.
\end{equation}
{{</m>}}
From Eqn.~\eqref{chap:collective-sec:dispersion-relation-eqn:eom-general-collective-modes-form} I have the formal solution
{{<m>}}
\begin{equation}
    Q_{\mathbf v} = - \frac{ v^\mu a_\mu }{ v^\alpha k_\alpha},
    \label{chap:collective-sec:dispersion-relations-eqn:q-expression-collective-mode}
\end{equation}
{{</m>}}
where
{{<m>}}
\begin{equation}
    a^\nu = \int \dd \Gamma_{\mathbf v} G({\mathbf v}) v^\nu Q_{\mathbf v}.
\end{equation}
{{</m>}}
Substituting Eqn.~\eqref{chap:collective-sec:dispersion-relations-eqn:q-expression-collective-mode} into Eqn.~\eqref{chap:collective-sec:dispersion-relation-eqn:eom-general-collective-modes-form}, I obtain
{{<m>}}
\begin{equation}
 v_\mu \Pi^{\mu}_{\phantom{\mu}\nu} a^\nu  = 0,
\end{equation}
{{</m>}}
where
{{<m>}}
\begin{equation}
\Pi^\mu_{\phantom{\mu}\nu} = \delta^\mu_{\phantom{\mu}\nu} + \int \dd \Gamma G(\mathbf v) \frac{v^\mu v_\nu}{\omega-  {\mathbf k}\cdot {\mathbf v} }.
\end{equation}
{{</m>}}
The dispersion relation between $\omega$ and $\mathbf k$ is obtained by solving the characteristic equation [^Izaguirre2016a]
{{<m>}}
\begin{equation}
\operatorname{det}\left( \Pi^\mu_{\phantom{\mu}\nu} \right) = 0
\label{eqn-dr-determinant-equation}
\end{equation}
{{</m>}}
since we are looking for non-trivial solutions of $a^\nu$.


[^Izaguirre2016a]: {{< ref key="Izaguirre2016a">}}