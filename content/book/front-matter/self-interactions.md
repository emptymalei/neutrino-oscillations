---
title: "Neutrino Self-interactions"
description: "Neutrino Self-interactions"
lead: ""
date: 2020-12-27
lastmod: 2020-12-27
draft: false
images: []
menu:
  book:
    parent: "Appendices"
weight: 930
toc: true
---



## Bipolar Model

The nature of this section is to provide the linear stability analysis of bipolar model. Bipolar model is a model of neutrino oscillations with the presence of neutrino and antineutrinos. It is also called bimodal oscillations [^Samuel1996], which means two frequencies in the context. An example of such instability happens in a system composed of equal amounts of neutrinos and antineutrinos.


Neutrino oscillations has a small amplitude inside a SN core (suppressed by matter effects) [^wolf78], which basically pins down the flavour transformation. As the neutrinos reaches a further distance, matter effect could drop out. Neutrino self-interaction becomes more important. S. Samuel considers a system of neutrinos and antineutrinos with only vacuum and neutrino self-interactions [^Samuel1996]. The neutrinos and antineutrino forms a bipolar vector in flavor isospin space. The flavor isospin of neutrinos and that of antineutrinos are coupled.


The equation of motion is
{{<m>}}
\begin{align*}
   i\partial_t \rho =& \left[ -\frac{\omega_\vv}{2} \cos2\theta \sigma_3 + \frac{\omega_\vv}{2}\sin 2\theta \sigma_1 - \mu \alpha \bar \rho , \rho\right] \\
   i\partial_t \bar\rho =& \left[ \frac{\omega_\vv}{2} \cos2\theta \sigma_3 - \frac{\omega_\vv}{2}\sin 2\theta \sigma_1 + \mu \rho , \bar\rho\right].
\end{align*}
{{</m>}}
For the purpose of linear stability analysis, we assume that
{{<m>}}
\begin{align*}
   \rho =& \frac{1}{2}\begin{pmatrix}
   1 & \epsilon \\
   \epsilon^* & -1
   \end{pmatrix} \\
   \bar\rho =& \frac{1}{2}\begin{pmatrix}
   1 & \bar\epsilon \\
   \bar \epsilon^* & -1
   \end{pmatrix}.
\end{align*}
{{</m>}}
Plug them into equation of motion and set $\theta=0$, we have the linearized ones,
{{<m>}}
\begin{equation*}
   i\partial_t \begin{pmatrix}
   \epsilon \\
   \bar\epsilon
   \end{pmatrix} = \frac{1}{2}\begin{pmatrix}
   -\alpha \mu - \omega_\vv & \alpha \mu \\
   -\mu & \mu + \omega_v
   \end{pmatrix}\begin{pmatrix}
   \epsilon \\
   \bar\epsilon
   \end{pmatrix}.
\end{equation*}
{{</m>}}
To have real eigenvalues, we require
{{<m>}}
\begin{equation*}
   (-1+\alpha)^2 \mu^2 + 4(1+\alpha)\mu \omega_\vv + 4 \omega_v^2 < 0,
\end{equation*}
{{</m>}}
which is reduced to
{{<m>}}
\begin{equation*}
   \frac{ -2\omega_\vv (1+\alpha) - 4\sqrt{ \alpha } \lvert \omega_\vv \rvert  }{ (1-\alpha)^2 } < \mu < \frac{ -2\omega_\vv (1+\alpha) + 4\sqrt{ \alpha } \lvert \omega_\vv \rvert  }{ (1-\alpha)^2 }.
\end{equation*}
{{</m>}}
It is simplified to
{{<m>}}
\begin{equation*}
   \sqrt{ -2\omega_\vv }{ (1-\sqrt{\alpha})^2 } < \mu < \sqrt{ -2\omega_\vv }{ (1+\sqrt{\alpha})^2 },
\end{equation*}
{{</m>}}
assuming normal hierarchy, i.e., $\omega_\vv > 0$. We immediately notice that this can not happen.

For inverted hierarchy, we have $\omega_\vv < 0$, so that
{{<m>}}
\begin{equation*}
   \sqrt{ 2\lvert\omega_v\rvert }{ (1+\sqrt{\alpha})^2 } < \mu < \sqrt{ 2\lvert\omega_v\rvert }{ (1-\sqrt{\alpha})^2 },
\end{equation*}
{{</m>}}
Within this region, neutrinos experience exponential growth.

For completeness, we also write down the formalism in flavor isospin picture.
{{<m>}}
\begin{align}
    i\partial_t \vec s &= \vec s \times ( \eta \vec H_\vv + \alpha \mu \bar{\vec s} )\\
    i\partial_t \bar{\vec s} &= \bar{\vec s} \times ( \eta \vec H_\vv + \mu \vec s ),
    \label{chap:app-sec:bipolar-eqn:flavor-isospin-eom}
\end{align}
{{</m>}}
where $\eta$ is the hierarchy, and $\alpha$ is the ratio of neutrino number density and antineutrino number density.


[^Samuel1996]: {{< cite key="Samuel1996" >}}
[^wolf78]: {{< cite key="wolf78" >}}
[^Samuel1996]: {{< cite key="Samuel1996" >}}