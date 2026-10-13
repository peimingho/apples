# Holography, Hagedorn strings, and a spacetime uncertainty relation from AdS/CFT

*Record of a discussion, 2026-10-13.*

Conventions: $\ell_s=\sqrt{\alpha'}$, $D$ = number of noncompact spacetime dimensions, $G_D\sim g_s^2\ell_s^{D-2}$, $16\pi G_{10}=(2\pi)^7g_s^2\alpha'^4$.
For AdS$_5\times S^5$: $R^2/\alpha'=\sqrt\lambda$, $g_s=\lambda/4\pi N$, $G_{10}=\pi^4R^8/2N^2$, $G_5=\pi R^3/2N^2$, and $x\equiv ER$.

---

## Q1. Holography (finitely many states) vs. Hagedorn growth (infinitely many states)?

**Answer:** the two do not conflict. The Hagedorn degeneracy is a density *in energy*, computed at $g_s=0$. The holographic bound counts the states that *fit in a region without collapsing*, and it has content only when $G\neq0$.

### 1.1 What each statement says

For the closed superstring, $\alpha'M^2/4=N$ and $c=12$ on each side:

$$
d(N)\simeq e^{4\pi\sqrt{2N}}\ \Rightarrow\ \rho(E)\sim E^{-a}e^{\beta_HE},\qquad \beta_H=2\pi\sqrt{2\alpha'}\quad(\text{bosonic: }4\pi\sqrt{\alpha'}).
$$

- Every level has finite degeneracy. The total is infinite only because $E$ is unbounded.
- The same holds for a free field in a box, $S_{\rm QFT}\sim(VE^{D-1})^{1/D}$.

The holographic statement is $\log\dim\mathcal H_{\rm region}\le A/4G_D$, enforced by the collapse bound

$$
E\le E_{\max}(R)=\frac{(D-2)\Omega_{D-2}}{16\pi G_D}R^{D-3}.
$$

It does **not** say the total Hilbert space is finite.

### 1.2 At $g_s=0$ the bound is vacuous

$$
\frac{A}{4G_D}\sim g_s^{-2}(R/\ell_s)^{D-2}\to\infty .
$$

### 1.3 At $g_s\neq0$

Take the string entropy at the largest energy the region can hold:

$$
\frac{S_{\rm str}}{S_{\rm BH}}=\frac{\beta_HE_{\max}(R)}{\Omega_{D-2}R^{D-2}/4G_D}=\frac{(D-2)\beta_H}{4\pi R}=\frac{D-2}{D-3}\frac{T_{\rm Hawking}(R)}{T_H}\sim\frac{\ell_s}{R}.
$$

- Saturation occurs at $r_s\sim\ell_s$, the string/black-hole correspondence point, where $S\sim g_s^{-2}$, $M\sim1/(g_s^2\ell_s)$ and $N\sim g_s^{-4}$.
- At fixed mass, $S_{\rm BH}(M)\propto M^{(D-2)/(D-3)}$ beats $\beta_HM$. The Hagedorn exponential is therefore not the asymptotic density of states of interacting string theory.
- Confining a long string in a box of size $R\gg\ell_s$ changes its entropy only to $S\simeq\beta_HE[1+O(\ell_s^2/R^2)]$. Finiteness comes from the gravitational energy cap, not from the extent of strings.

### 1.4 Where fuzziness enters

The stringy fuzziness relations are

$$
\Delta X\gtrsim\frac{\hbar}{\Delta p}+\alpha'\frac{\Delta p}{\hbar},\qquad\Delta X\,\Delta T\gtrsim\alpha'.
$$

- A string at level $N$ has size $R_N\sim\ell_sN^{1/4}$, plus a spread $\alpha'\ln(1/\epsilon)$ that depends on the resolution $\epsilon$ (UV/IR mixing).
- The holographic capacity of a string-scale cell is $S_{\rm BH}(\ell_s)\sim g_s^{-2}$. This equals the entropy of a string at the correspondence point, so the Hagedorn degeneracy is what fills that capacity at weak coupling.

### 1.5 AdS check: phases of AdS$_5\times S^5$ at strong coupling

Regimes as $x=ER$ increases (Banks–Douglas–Horowitz–Martinec):

| Range of $x$ | Dominant phase | $S(x)$ |
|---|---|---|
| $x\lesssim\lambda^{5/2}$ | graviton gas | $x^{9/10}$ |
| $\lambda^{5/2}\lesssim x\lesssim N^2\lambda^{-7/4}$ | Hagedorn strings | $\lambda^{-1/4}x$ |
| $N^2\lambda^{-7/4}\lesssim x\lesssim N^2$ | small 10d black hole | $N^{-2/7}x^{8/7}$ |
| $x\gtrsim N^2$ | large AdS black hole | $N^{1/2}x^{3/4}$ |

- The Hagedorn window ends where the 10d black hole has $r_s\sim\ell_s$.
- In free SYM, Hagedorn growth holds only for $ER\ll N^2$.

---

## Q2. Size–energy relation of strings, and which scale dominates the entropy of AdS

### 2.1 Flat space

**Typical (entropy-dominant) size.** From the closed-string modes with thermal occupation at worldsheet inverse temperature $\beta_{\rm ws}=\pi\sqrt{c/6N}$:

$$
\langle(\delta X^i)^2\rangle=\alpha'\sum_{n\ge1}\frac{\langle N_n\rangle+\langle\tilde N_n\rangle+1}{n}
\ \Rightarrow\
\boxed{\langle R^2\rangle\simeq\frac{(D-1)\pi^2\alpha'^2}{3\beta_H}E+(D-1)\alpha'\ln\frac1\epsilon}
$$

This is a random walk, $R\sim\ell_s(E\ell_s)^{1/2}=\ell_sN^{1/4}$.

**Maximal and minimal size.**

- Maximum, a folded string at its turning point: $\ell_{\max}=\pi\alpha'E$. This saturates the GUP.
- Minimum: $\sim\ell_s$.

**Entropy at fixed $E$ and $R$.** $S(E,R)=\beta_HE-\Phi(R^2/\langle R^2\rangle)$, with $\Phi(y)\propto y$ for $y\gg1$ and $\propto 1/y$ for $y\ll1$. At $\ell_{\max}$, $\Phi=O(\beta_HE)$, so fully stretched strings carry no entropy.

### 2.2 AdS: the harmonic trap

Each unit of string length costs energy $T\sqrt{-g_{tt}}\simeq T(1+r^2/2R^2)$.

**Maximal extent becomes logarithmic.** From $E=2TR\sinh(\ell/R)$:

$$
\ell_{\max}=R\,\mathrm{arcsinh}\frac{\pi\alpha'E}{R}\ \to\ R\ln\frac{2\pi\alpha'E}{R}.
$$

This matches the logarithmic behaviour of GKP spinning strings.

**Thermal scalar in the trap.** The winding mode $\chi$ obeys

$$
\Big[-\nabla^2+\frac{\beta^2-\beta_H^2}{4\pi^2\alpha'^2}+\omega^2r^2\Big]\chi=0,\qquad \omega=\frac{\beta}{2\pi\alpha' R}.
$$

The Hagedorn temperature shifts to

$$
T_H^{\rm AdS}=T_H+\frac{d}{8\pi R}\ \Rightarrow\ T_HR=\frac{\lambda^{1/4}}{2\sqrt2\pi}+\frac1{2\pi}+\dots=\sqrt{\frac g{2\pi}}+\frac1{2\pi}+\dots
$$

- Check against the QSC: at $\sqrt g=1.8$ the formula gives $0.877$, compared with $T_H=0.8817$ from the QSC numerics (arXiv:2109.09761).
- The entropy cost of the trap is $S\simeq(\beta_H-\pi\alpha'd/R)E$.

**Typical size saturates.**

$$
\boxed{\langle x_i^2\rangle_{\rm AdS}\simeq\min\Big(\frac{\pi^2\alpha'^2E}{3\beta_H},\ \frac{\pi\alpha'R}{\beta_H}\Big)}
$$

- In the AdS directions the size saturates at $\rho\sim(\ell_sR)^{1/2}$ once $ER\gtrsim\frac3\pi\sqrt\lambda$.
- On $S^5$ the string is smeared over the whole sphere once $ER\gtrsim\lambda^{3/4}$.
- Self-gravity relative to the trap is $\sim\frac\pi2x\sqrt\lambda/N^2$, which is negligible throughout the Hagedorn window.

### 2.3 Which scale dominates

| Range of $x$ | Phase | $TR$ | Size |
|---|---|---|---|
| $\lesssim\lambda^{5/2}$ | 10d gas | $x^{1/10}$ | $\sim R$ |
| $\lambda^{5/2}$ to $N^2\lambda^{-7/4}$ | long string, plus gas at $T_H$ | $T_HR$ | $(\ell_sR)^{1/2}$, smeared on $S^5$ |
| $N^2\lambda^{-7/4}$ to $N^2$ | 10d black hole | $(N^2/x)^{1/7}$ | $r_s=R(x/N^2)^{1/7}$ |
| $\gtrsim N^2$ | AdS$_5$ black hole | $(4x/3\pi^4N^2)^{1/4}$ | $r_h\gtrsim R$ |

- **Gas to strings:** the gas hands over to strings exactly when its temperature reaches $T_H$.
- **Strings in AdS are always saturated:** because $\lambda^{5/2}\gg\lambda^{3/4}\gg\lambda^{1/2}$, every string that dominates the entropy is in the saturated regime.
- **Black holes, local view** (Susskind 1993). With $dS=2\pi\,dE_R$ and local energy $E_{\rm loc}=E_R/\rho$, the condition $S=\beta_HE_R/\rho_c=2\pi E_R$ is equivalent to $\rho_c=\beta_H/2\pi$, i.e. Unruh temperature $=T_H$. The energy per string-scale cell of the horizon is then $\sim1/(g_s^2\ell_s)$, the correspondence-point mass.
- **Conclusion:** once $x\gtrsim\lambda^{5/2}$, the entropy is carried at the **local string scale**. Only the dilute gas stores its entropy below $T_H$.
- **AdS with an infrared cutoff:** $S_{\max}=\pi N^2(r_c/R)^3$, i.e. $N^2$ per boundary cell. It is dominated by the UV of the CFT.

---

## Q3. Deriving a spacetime uncertainty relation (SUR) from AdS/CFT: suggestions

### 3.0 What symmetry fixes

Use Poincaré AdS with $r=R^2/z$.

**(a) The time–radial pair is boundary Heisenberg.** The proper product reduces to a coordinate product, $\Delta T_p\Delta Z_p=\Delta t\,\Delta r$, and

$$
\Delta T_p\Delta Z_p\ge\pi\alpha'\iff\Delta t\,\Delta E_W\ge\tfrac12,\qquad E_W=\frac{r}{2\pi\alpha'}.
$$

This is boundary Heisenberg plus the Peet–Polchinski stringy UV/IR relation, so it carries no new information.

**(b) Bulk Lorentz invariance forces a hyperbola.** Since $SO(1,d)\subset SO(2,d)$, a bound with one length must be $\Delta X^+\Delta X^-\ge\ell^2$, not a box. In boundary variables:

$$
\Delta x^+\Delta x^-\ge(\ell^2/R^2)z^2 .
$$

The task is to compute $\ell$ from CFT data: $\lambda$ through the gap and Regge slope, and $C_T\propto N^2$ through $G$.

### 3.1 Main proposal: a light-cone commutator from the CFT Regge (eikonal) limit

1. **Eikonal form (Cornalba–Costa–Penedones–Schiappa).** In impact-parameter space,
   $$
   \langle O_1O_2O_2O_1\rangle\to\int e^{-2\pi i\Gamma(s,L)},\qquad 2\pi\Gamma=4\pi G_5\,s\,\frac{\Pi_3(L)}{R},\qquad \Pi_3=\frac{e^{-2L}}{4\pi\sinh L}.
   $$
2. **Algebra ('t Hooft; Verlinde–Verlinde; Kiem–Verlinde–Verlinde).** With $s=2p^+p^-$, the S-matrix $\exp[i\int P^+(8\pi GF)P^-]$ gives
   $$
   [X^+(y),X^-(y')]=8\pi iG\,F(y,y')\ \Rightarrow\ \Delta X^+\Delta X^-\ge4\pi G\,|F| .
   $$
   The $X^-$ shift is generated by ANEC/light-ray operators (Afkhami-Jeddi–Hartman–Kundu–Tajdini 2017).
3. **Stringy smoothing.** With $j(\nu)=2-\frac{\nu^2+4}{2\sqrt\lambda}+O(\lambda^{-1})$:
   $$
   \Gamma\propto Gs\int d\nu\,\Omega_{i\nu}(L)\,s^{j(\nu)-2}\Big[\frac1{\nu^2+4}+\frac{i\pi}{4\sqrt\lambda}+\dots\Big],
   $$
   $$
   \boxed{\mathrm{Re}\,F_\lambda(s;L)=\frac1R\int_{\tau_s}^\infty d\tau\,e^{-3\tau}K_{H_3}(\tau;L),\qquad \tau_s=\frac{\ln\tilde s}{2\sqrt\lambda}=\frac{\alpha'\ln\tilde s}{2R^2}}
   $$
   with $K_{H_3}=(4\pi\tau)^{-3/2}\frac{L}{\sinh L}e^{-\tau-L^2/4\tau}$. The imaginary part, $\mathrm{Im}\,F\propto\lambda^{-1/2}e^{-3\tau_s}K_{H_3}(\tau_s;L)$, describes tidal string excitation, i.e. decoherence.
4. **Proposed SUR:** $\Delta X^+\Delta X^-\ge4\pi G\,\mathrm{Re}F_\lambda(s;L)$. Its three regimes:
   - **$b\gtrsim R$:**
     $$
     \frac{\Delta X^+\Delta X^-}{R^2}\ge\frac{\pi}{2N^2}\frac{e^{-2L}}{\sinh L}.
     $$
   - **$b\ll R$ (10d):** the supergravity profile $f_8=1/(2\pi^4b^6)$ is smoothed below $b\sim\sqrt{2\alpha'\ln\tilde s}$, giving
     $$
     \Delta X^+\Delta X^-\big|_{b\to0}\simeq\frac{\pi^3}{3}\frac{g_s^2\alpha'}{\ln^3\tilde s}=\frac{\pi\lambda^2}{48N^2}\frac{\alpha'}{\ln^3\tilde s}.
     $$
   - **$\ln\tilde s\gtrsim\sqrt\lambda$:** the effective coupling becomes $G_{\rm eff}=G\tilde s^{\,j_0-2}$ with $j_0-2=-2/\sqrt\lambda$. The transverse spread $\langle b^2\rangle=3\alpha'\ln\tilde s$ becomes ballistic, $\langle b\rangle\simeq(\alpha'/R)\ln\tilde s$.

### 3.2 Thermal version: the horizon algebra from the OTOC

$$
[U(\vec x),V(\vec x')]=8\pi iG\,F^{(\beta)}_\lambda(t;\vec x-\vec x'),\qquad \tilde s\propto e^{2\pi t/\beta}.
$$

- **Supergravity profile:** $(-\partial^2+\mu^2)f=\delta$, with $\mu=2\pi/(\beta v_B)$ and $v_B^2=d/2(d-1)$.
- **Stringy corrections (Shenker–Stanford):** $\lambda_L=\frac{2\pi}\beta[1-O(\lambda^{-1/2})]$, and the transverse spread grows diffusively, $b^2\sim\alpha'(2\pi t/\beta)$.
- **Payoff:** a CFT-derived, string-corrected trans-Planckian cutoff near the scrambling time.

### 3.3 Complementary planar check

Use the bulk-point limit (Maldacena–Simmons-Duffin–Zhiboedov) with the AdS Virasoro–Shapiro amplitude (Alday–Hansen–Silva).

- The Gross–Mende saddle gives $\Delta T\Delta X_L\gtrsim\alpha'[1+O(\alpha'/R^2)]$.
- Test: is the region over which the bulk-point singularity is smoothed boost-covariant (a hyperbola) rather than a box?

### 3.4 Matrix-model alternative (D0/BFSS)

Generalized conformal symmetry is $t\to t/\zeta$, $U\to\zeta U$, $g^2_{YM}\to\zeta^3g^2_{YM}$. Any SUR must then take the form

$$
\Delta t\,\Delta U\ge\mathcal F(g_{\rm eff}^2),\qquad g_{\rm eff}^2=\frac{g^2_{YM}N}{U^3}.
$$

- Stretched strings: $\mathcal F=\pi$.
- Supergravity probes: $\mathcal F\propto g_{\rm eff}$.
- The gravitational bound $\Delta t\,\Delta r^7\gtrsim G_{10}$ meets $\Delta t\,\Delta r\gtrsim\alpha'$ at $\Delta r\sim g_s^{1/3}\ell_s=\ell_{11}$, the Li–Yoneya scale.
- $\mathcal F$ can be measured from BFSS Monte Carlo data.

### 3.5 Next steps

1. Rederive $\mathrm{Re}F_\lambda$ from the Cornalba–Costa–Penedones Regge-theory phase shift (0710.5480). Check its $\lambda\to\infty$ limit against the AHKT shock.
2. Prove that $\exp(iP^+FP^-)$ factorizes on the two-probe space to $O(\lambda^{-1/2})$, and identify $X^\pm$ with light-ray operators.
3. Work out the three regimes, keeping the 10d/5d crossover at $b\sim R$ explicit.
4. Do the thermal version and compute the scrambling-time cutoff.
5. Optionally, use the QSC $j(\nu)$ at finite coupling to get an all-$\lambda$ SUR.

**Pitfalls**

- $X^\pm$ are relational, defined through the probes.
- The algebra is valid only where the eikonal approximation holds and $|\mathrm{Im}\,\Gamma|\ll1$.
- Multi-Pomeron exchange and black-hole formation set in when $|\Gamma|\sim1$.

**Prior work to check:** Polchinski, *Chaos in the black hole S-matrix* (2015); Gaddam–Groenenboom–'t Hooft–Verlinde; Minic (1998); Yoneya (2000).

---

## References

- [Harmark & Wilhelm, QSC Hagedorn temperature (arXiv:2109.09761)](https://arxiv.org/abs/2109.09761)
- [Harmark, curvature corrections to the Hagedorn temperature via the thermal scalar (JHEP 2024)](https://doaj.org/article/09d0d050c1ab459199cdf960f81346c5)
- [Cornalba, Costa, Penedones — Eikonal Methods in AdS/CFT: Regge Theory and Multi-Reggeon Exchange (arXiv:0710.5480)](https://arxiv.org/abs/0710.5480)
- [Cornalba, Costa, Penedones — Eikonal Methods in AdS/CFT: BFKL Pomeron at Weak Coupling (arXiv:0801.3002)](https://arxiv.org/abs/0801.3002)
- Other works cited from memory and not re-verified:
  - Susskind (hep-th/9309145); Horowitz–Polchinski (1996, 1997); Chen–Maldacena–Witten (2021).
  - Banks–Douglas–Horowitz–Martinec (1998); Aharony–Marsano–Minwalla–Papadodimas–Van Raamsdonk (2003).
  - Karliner–Klebanov–Susskind (1988); Peet–Polchinski (1998); Jevicki–Yoneya (1998).
  - Brower–Polchinski–Strassler–Tan (2006); Costa–Gonçalves–Penedones (2012).
  - Afkhami-Jeddi–Hartman–Kundu–Tajdini (2017); Kiem–Verlinde–Verlinde (1995); Shenker–Stanford (2014).
  - Maldacena–Simmons-Duffin–Zhiboedov (2015); Alday–Hansen–Silva (2022).
