# Literature notes: prior work for "a spacetime uncertainty relation from AdS/CFT"

*Compiled 2026-10-13; revised the same day from the full texts. Companion to `2026-10-13_holography-strings-and-SUR-from-AdS-CFT.md`.*

> **Sources.** All six papers were read in full, from the PDFs in `papers/`. These were taken from arXiv's public mirror; arxiv.org itself is blocked in this environment. Equations were checked against renders of the PDF pages. Equation numbers are the papers' own.
>
> **[inference]** marks our reading or derivation; it is not a statement in the paper.
>
> Journal references not printed on the arXiv PDFs come from search listings.

| # | Paper | Version read |
|---|---|---|
| 1 | L. Cornalba, arXiv:0710.5480 | v3 (25 pp) |
| 2 | L. Cornalba, M. S. Costa, J. Penedones, arXiv:0801.3002 | v2 (42 pp) |
| 3 | J. Polchinski, arXiv:1505.08108 | v2 (13 pp) |
| 4 | N. Gaddam, N. Groenenboom, G. 't Hooft, arXiv:2012.02357 | v3 (14 pp) |
| 5 | D. Minic, hep-th/9808035 | v1 (15 pp) |
| 6 | T. Yoneya, hep-th/0004074 | v6 (45 pp) |

**Corrections to the earlier note:**
- 0710.5480 has a **single author, Cornalba**.
- The paper earlier cited as "Gaddam–Groenenboom–'t Hooft–Verlinde" is **Gaddam–Groenenboom–'t Hooft**. Verlinde appears only in its references.

---

## 1. L. Cornalba, "Eikonal Methods in AdS/CFT: Regge Theory and Multi-Reggeon Exchange"

**Bibliographic data.** arXiv:0710.5480 [hep-th, hep-ph]: v1 29 Oct 2007, v3 6 Oct 2008. The author is Cornalba alone; Costa and Penedones are acknowledged. No journal reference was found.

**Summary**
- **Setting.** Regge theory for CFT four-point functions $\langle O_1O_2O_1O_2\rangle$ in the Lorentzian limit $\sigma\to0$. Each T-channel partial wave scales as $\sigma^{1-J}$.
- **Regge pole.** A Sommerfeld–Watson transform, with harmonic analysis on the transverse $H_3$, gives a pole at $J=j(\nu)$.
- **Eikonal.** The pole is written in impact-parameter space. Multi-reggeon exchange is resummed by exponentiating the tree-level phase shift, in the manner of Amati–Ciafaloni–Veneziano.
- **Strong coupling.** For $\mathcal N=4$ at strong coupling, $j(\nu,g)$ and the residue $\beta(\nu,g)$ are fixed to leading order in string corrections by matching to Virasoro–Shapiro. This reproduces and extends Brower–Polchinski–Strassler–Tan (BPST).

**Key equations** ($d=4$)

*Kinematics:* $z=\frac\sigma4e^{\rho}$, $\bar z=\frac\sigma4e^{-\rho}$; $h^2=\frac s4e^{r}$, $\bar h^2=\frac s4e^{-r}$. Here $s=4|\mathbf y||\bar{\mathbf y}|$ is **dimensionless**, with $s/\ell^2\to S$ in the flat limit. The convention is $(-)^\alpha\equiv e^{i\pi\alpha}$.

*Impact-parameter representation (7)–(9):*
$$
A=(-)^{-\Delta_1}(-)^{-\Delta_2}\!\int_M d\mathbf y\,d\bar{\mathbf y}\;e^{-2i\mathbf x\cdot\mathbf y-2i\bar{\mathbf x}\cdot\bar{\mathbf y}}\,\mathcal B,\qquad \mathcal B=e^{-2\pi i\Gamma}.
$$
$\Gamma$ gives both the AdS phase shift and the large-spin anomalous dimension ($2\Gamma$).

*$H_3$ harmonics (11)–(16):*
$$
\Pi_E=\frac{e^{-E\rho}}{4\pi\sinh\rho},\qquad [\Box_{H_3}-E^2+1]\Pi_E=-\delta,\qquad \Pi_E=\int d\nu\,\frac{\Omega_{i\nu}}{\nu^2+E^2}.
$$

*Phase shift (29) and §5:* with $g=\ell^2/\alpha'=\sqrt\lambda$ and $1/N^2=2G/(\pi\ell^3)$,
$$
\Gamma\simeq\int d\nu\,\beta\,s^{\,j(\nu)-1}\Omega_{i\nu}(r),\qquad
\Gamma_{\rm sugra}=-\frac{2G}{\ell^3}\,s\!\int\!\frac{d\nu}{\nu^2+4}\Omega_{i\nu}(r).
$$

*Trajectory (31)–(33):*
$$
j(\pm2i,g)=2,\qquad j(\nu,g)=2-\frac{4+\nu^2}{2g}-(4+\nu^2)\sum_{n\ge2}\frac{\tilde j_n(\nu)}{g^n}.
$$

*Residue (p. 19):*
$$
\beta(\nu,g)=-\frac1{4g}(-)^{-j/2}\frac{\Gamma(1-j/2)}{\Gamma(j/2)}+\cdots
$$

**Validity.** Lorentzian $\sigma\to0$; string tree level; large impact parameter; leading pole only; $g\to\infty$ at fixed $\nu$.

**Not in the paper:**
- commutators, time delays, uncertainty relations;
- the heat-kernel or proper-time form;
- transverse diffusion;
- any discussion of $\mathrm{Im}\,\Gamma$.

**Check of our proposal** [inference]

1. **Trajectory.** It agrees with ours, $j=2-\frac{\nu^2+4}{2\sqrt\lambda}$. The $O(1/\lambda)$ term is also $\propto(4+\nu^2)$, so the proper-time form survives at that order.

2. **Residue.** Expanding $\beta$ gives
   $$
   \beta=\frac1{\nu^2+4}+\frac{i\pi-2\gamma_E}{4g}+\dots
   \ \Rightarrow\
   \beta s^{j-2}\simeq\frac{e^{-(\nu^2+4)\tilde\tau_s}}{\nu^2+4},\qquad
   \tilde\tau_s=\frac{\ln s+\gamma_E-i\pi/2}{2\sqrt\lambda}.
   $$
   - The real part is our proper-time-cutoff propagator with $\ln s\to\ln s+\gamma_E$.
   - $\mathrm{Im}\,\Gamma\propto-\frac{\pi}{4\sqrt\lambda}e^{-3\tau_s}K_{H_3}$, which is negative (absorption).

3. **Sign convention.** $\delta=-2\pi\Gamma_{\rm Cornalba}$ is the physical eikonal phase.

4. **Open: the scale of $s$.** Matching $s^{j-2}$ to Virasoro–Shapiro leaves a factor $(4g)^{-\alpha'q^2/2}$. This could shift $\tau_s$ to $\propto\ln(s/4\sqrt\lambda)$. Check against BPST.

---

## 2. L. Cornalba, M. S. Costa, J. Penedones, "Eikonal Methods in AdS/CFT: BFKL Pomeron at Weak Coupling"

**Bibliographic data.** arXiv:0801.3002v2 (30 Sep 2008); JHEP 06 (2008) 048.

**Summary.** The paper studies the planar $\langle O_1O_2O_1^\star O_2^\star\rangle$, mainly for $O_1={\rm Tr}Z^2$ and $O_2={\rm Tr}W^2$, in the Lorentzian Regge limit. It reads the correlator as an AdS "S-matrix" in which CFT positions play the role of AdS momenta. Using the transverse conformal group $SO(1,1)\times SO(3,1)$ acting on $\mathbb E_2\leftrightarrow H_3$, it:
- recasts BFKL in position space;
- shows that only the conformal-spin $n=0$ kernel couples to scalars;
- fixes the impact factors by conformal invariance and computes them at leading order;
- reproduces the $j=1$ Regge behaviour of the known $g^4$ correlator.

It then speculates on an AdS (5d) eikonal resummation of multi-pomeron exchange.

**Key equations** ($g^2=\lambda$, $\ell=\sqrt{\alpha'g}$, $G=\pi\ell^3/2N^2$)

*Regge pole (5).*
$$
\hat A\simeq2\pi i\!\int d\nu\,(-)^{j}\alpha(\nu,g)\,|4x\bar x|^{1-j}\,\Omega_{i\nu}(x,\bar x)
$$
- $(\square_{H_3}+\nu^2+1)\Omega_{i\nu}=0$ and $\Omega_{i\nu}=\frac{\nu\sin\nu\rho}{4\pi^2\sinh\rho}$.
- Exchanged dimensions are $2+i\nu$ (footnote 2).

*Impact-parameter form (10).*
$$
\hat A=\frac{4|x\bar x|^4}{\pi^2}\!\int_M dy\,d\bar y\,e^{-2ix\cdot y-2i\bar x\cdot\bar y}e^{-2\pi i\Gamma},\qquad
\Gamma_{\rm planar}\simeq N^{-2}\!\int d\nu\,\beta\,|4y\bar y|^{j-1}\Omega_{i\nu}.
$$
Here $s=|4y\bar y|$ and $\cosh r=-y\cdot\bar y/|y\bar y|$. The unitarity condition is $\mathrm{Im}\,\Gamma\le0$.

*Strong coupling (quoted from BPST and Cornalba).*
$$
j=2-\frac{4+\nu^2}{2g}+\dots
$$
The constraint $j(\pm2i)=2$ is asserted "for any value of $g$". The residue is $\beta\simeq-\pi/(4+\nu^2)$ (11), which is real.

*Weak coupling.*
- The correlator is (7), $\hat A\simeq-\frac{g^4}{8\pi^2}\frac{z\bar z}{(z-\bar z)^2}\log^2\frac{\bar z}z$, which corresponds to $j=1$.
- The trajectory is quoted from BFKL:
$$
j(\nu,g)=1+\frac{g^2}{4\pi^2}\Big[2\Psi(1)-\Psi\big(\tfrac{1+i\nu}2\big)-\Psi\big(\tfrac{1-i\nu}2\big)\Big],\qquad j(0)=1+\frac{g^2\ln2}{\pi^2}.
$$
  In terms of the standard BFKL variable, $\nu=2\nu_B$ [inference].
- Residue and impact factors:
$$
\alpha=-\frac{i}{4\pi}V\,\frac{\tanh(\pi\nu/2)}{\nu}\,\bar V\ \ (8,33),\qquad V=\frac{\pi g^2}{2\cosh(\pi\nu/2)}\ \ (9),\qquad \beta\simeq-\frac{ig^4}{\pi}\frac{\tanh(\pi\nu/2)}{\nu(1+\nu^2)^2}\ \ (11).
$$
- The impact factors are fixed by conformal invariance, $V=V(u)/z_{13}^2$ (27). At leading order, $V(u)=\frac{g^2}{4\pi^3}u^2[1-\delta(u)]$ for ${\rm Tr}Z^2$.

*AdS eikonal (12).* This is $\hat A_{\rm eik}$, the exponentiation of $\Gamma_{\rm planar}$ inside the $y,\bar y$ integral.
- It follows geodesic motion in AdS$_5$, not 4d momentum space.
- The authors note that 4d eikonalization of BFKL fails and needs pomeron self-interactions (saturation).
- They say multi-pomeron interactions have "never been analyzed" with (12), and that the relation to 4d is "an important unresolved issue".

**Validity.** Planar; $x,\bar x\to0$; leading order ($g^2$ impact factors, leading-log trajectory). At weak coupling the eikonal is explicitly speculative.

**Not in the paper:** commutators, time delays or uncertainty relations. It cites the shock-wave paper but has no such discussion.

**Relevance** [inference]
- **Support.** It confirms our strong-coupling $j(\nu)$, the $H_3$ normalization ($-\square\Omega=(1+\nu^2)\Omega$) and the $e^{-2\pi i\Gamma}$ convention.
- **Ready-made all-coupling form.** $\Gamma=N^{-2}\int d\nu\,\beta(\nu,\lambda)s^{j(\nu,\lambda)-1}\Omega_{i\nu}$, with the two limits above as endpoints.
- **Obstacles to an all-$\lambda$ light-cone commutator:**
  1. At weak coupling, leading order, $\beta$ is imaginary and $s^{j-1}=s^0$. The phase is pure absorption, so a commutator $\propto\mathrm{Re}\,\Gamma$ starts only at $O(g^2)$. It grows as $s^{\bar\alpha\chi}$, not $s$, so the shock structure $G\,p\,F$ is lost.
  2. The leading-order BFKL $j(\pm2i)=1+\frac{g^2}{4\pi^2}(4\ln2-4)\neq2$. It is valid only near $\nu\approx0$, so the full curve is needed (e.g. from the QSC).
  3. At weak coupling $H_3$ is kinematic, so $X^\pm$ as bulk positions is only an interpretation.
  4. The weak-coupling eikonal is speculative.

---

## 3. J. Polchinski, "Chaos in the black hole S-matrix"

**Bibliographic data.** arXiv:1505.08108v2, 1 Jun 2015; 13 pp. No journal reference; his 2016 TASI review cites it as arXiv only. The v2 comment reads "correction to eq. 2.18 and added clarification (new footnote 6)". What changed in (2.18) is unknown, since only v2 was read.

**Summary**
- **Extension.** The Shenker–Stanford–Kitaev picture (horizon ↔ Lyapunov growth) is extended from eternal black holes in cavities to black holes that form and evaporate, in asymptotically flat $D$ dimensions.
- **Assumptions.** An S-matrix exists, and effective field theory (EFT) is valid outside the horizon.
- **Result.** The Dray–'t Hooft shock-wave shift becomes an identity between S-matrix elements with and without one extra massless infalling particle. Outgoing modes emitted later are shifted by $\propto e^{2\pi t/\beta}$, up to the scrambling time.
- **§3.** The identity is invisible in the EFT (Hawking) vacuum and exists only because an S-matrix was assumed. It is a restatement of the AMPS firewall argument: chaos and the firewall are "two sides of the same coin (or horizon)".

**Key equations**

*Chaos diagnostic and redshift.*
$$
Z^{-1}\mathrm{Tr}\,e^{-\beta H}[\hat W(t),\hat V(0)][\hat W(t),\hat V(0)]^\dagger\ \ (1.3),\qquad \frac{d\tau}{dt}\propto e^{-2\pi t/\beta}\ \ (1.4)
$$
The growth rate is twice the Lyapunov exponent because the commutator is squared. The quasinormal modes are the Ruelle resonances.

*Shock wave.*
$$
ds^2=2g_{uv}dv\,(du-F\,dv)+r^2d\Omega^2_{D-2}\ \ (2.9),\qquad u=-e^{2\pi(r^*-t)/\beta},\ v=e^{2\pi(r^*+t)/\beta}\ \ (2.10),
$$
$$
g_{uv}(0,0)\Big(-\nabla^2_{D-2}+\tfrac{(D-3)(D-2)}2\Big)\Delta u=-16\pi G\,r_s^2\!\int\! dv\,\partial_vh\,\partial_vh\ \ (2.12),
$$
$$
\tilde h'(u,\theta)=h'(u-\Delta u(\theta),\theta)\ \ (2.13),\qquad \Delta t=e^{2\pi(t-r^*)/\beta}\Delta u\ \ (2.14).
$$

*Exchange relation (2.17)*, from Kiem–Verlinde–Verlinde, which the paper calls "the commutator":
$$
a_{\tilde h',\alpha'}\,a^\dagger_{h,\alpha}=a^\dagger_{\tilde h,\alpha}\,a_{h',\alpha'}.
$$

*Identity (2.18).* The in-operator $a^\dagger_h$ is commuted leftward past the outgoing modes $k,\dots,m$, which become $\tilde h'$, but "only as far as we trust" (2.17):
$$
\langle0|a_{\tilde h'_1}\cdots a_{\tilde h'_m}\,a^\dagger_{h}\,a^\dagger_{h_1}\cdots a^\dagger_{h_n}|0\rangle
=\langle0|a_{\tilde h'_1}\cdots a_{\tilde h'_{k-1}}\,a^\dagger_{\tilde h}\,a_{h'_k}\cdots a_{h'_m}\,a^\dagger_{h_1}\cdots a^\dagger_{h_n}|0\rangle .
$$
(Mode labels $\alpha$ are suppressed.)

*Equation (2.20).* Squaring and tracing over modes emitted after $t_{\rm scr}$ gives a unitarity-preserving reduced "\$-matrix" for the radiation emitted before $t_{\rm scr}$.

**Regime**
- Effects must lie between $G\,r_s^{2-D}$ and $O(1)$.
- The scrambling time is set by $t_1-t_0\gtrsim\frac\beta{2\pi}\ln\frac{r_s^{D-3}}{EG}$.
- At $t_{\rm scr}$ the collision energy is $E_{\rm coll}\sim\sqrt{r_s^{4-D}/G}$ (2.19). The impact parameter is $\sim r_s$, so gravity stays weak.
- The infaller is massless.

**Strings and AdS**
- One sentence on strings: "stringy corrections to the Lyapunov exponent" may appear (citing Shenker–Stanford). Nothing is computed.
- AdS is not used.

**Relevance** [inference]
- **Novelty.** No uncertainty relation, no $[X^+,X^-]$, no AdS/CFT or Regge input. It does not pre-empt our proposal.
- **Inputs it supplies:**
  - the $D$-dimensional transverse operator $-\nabla^2_{D-2}+\frac{(D-3)(D-2)}2$, whose analogue for us is $\Pi_3$ on $H_3$;
  - the exponent $2\pi/\beta$;
  - the window $t\lesssim t_{\rm scr}$, where $\Delta u\sim|u|$ corresponds to an eikonal phase $p_u\Delta u\sim1$, i.e. our $|\Gamma|\sim1$ edge.
- **Normalization.** His $16\pi G\,r_s^2/g_{uv}$ and our $8\pi GF$ use different conventions ($2g_{uv}du\,dv$ versus $-dx^+dx^-$, and packet normalizations). Redo the shock in our conventions before quoting $4\pi G|F|$.
- **State and ordering (Polchinski's own point).** There is "no relation analogous to Eq. (2.20)" in the near-horizon EFT vacuum, which is invariant under small shifts of $u$. **So $\Delta X^+\Delta X^-\ge4\pi G|F|$ cannot be a variance in the Hartle–Hawking or Unruh state.** It must be stated for amplitudes or out-of-time-order correlators, and the thermal $[U,V]$ only for $t\lesssim t_{\rm scr}$.

---

## 4. N. Gaddam, N. Groenenboom, G. 't Hooft, "Quantum gravity on the black hole horizon"

**Bibliographic data.** arXiv:2012.02357v3 (8 Jan 2022), Utrecht; JHEP 01 (2022) 023. The propagator (2.4) is derived in the companion Gaddam–Groenenboom, arXiv:2012.02355.

**Summary**
- **Process.** $2\to2$ scattering of a massless scalar on the Schwarzschild horizon, in a partial-wave basis, for $L_{\rm Pl}\ll b\le R_S$.
- **Reduction.** Working in Regge–Wheeler gauge, the theory reduces on the sphere to a 2d theory for each $(\ell,m)$.
- **Resummation.** Ladders of soft ($k=0$) virtual gravitons are resummed to all orders in $\gamma\sim M_{\rm Pl}/M_{\rm BH}$, and hence in $\hbar$. Each partial wave gives a pure eikonal phase.
- **Result.** A second-quantized form of 't Hooft's S-matrix, but with $\ell^2+\ell+2$ where 't Hooft has $\ell^2+\ell+1$.
- **Energy condition.** The required energy is not Planckian: $s\gg\gamma^2M_{\rm Pl}^2$.

**Key equations**

*Setup.* $S=\frac12\int\sqrt{-g}\,(R/8\pi G-\nabla\phi\cdot\nabla\phi)$ with $\kappa=\sqrt{8\pi G}$ and $\gamma=\sqrt{8\pi G}/R_S$. In Kruskal coordinates the background is $g^0=-2A\,dx\,dy+r^2d\Omega^2$, with
$$
xy=2R_S^2(1-r/R_S)\,e^{r/R_S-1}\quad(2.1).
$$

*Graviton propagator (2.3)–(2.4).* $\mathcal P^{abcd}=\frac14f_\ell(k^2)(\eta^{ac}\eta^{bd}+\eta^{ad}\eta^{bc})$, with
$$
f_\ell(k^2)=-\frac{4R_S^2}{\lambda+1}-\frac{2R_S^4k^4}{(\lambda+1)(\lambda-3)(k^2+R_S^{-2}\lambda)},\qquad \lambda=\ell^2+\ell+1 .
$$
Only $f_\ell(0)=-4R_S^2/(\lambda+1)$ is used. The paper reads it as an effective 2d graviton mass from horizon curvature.

*Near-horizon action (2.5).*
$$
S_{\rm hor}=\tfrac14\!\int\! d^2k\,\mathfrak h\,\mathcal P^{-1}\mathfrak h-\tfrac12\!\int\! d^2p\,\phi\,(p^2+\lambda/R^2)\,\phi+\gamma\!\int\!\delta^{(2)}(k+p_1+p_2)\,\mathfrak h_{ab}(k)\,p_1^ap_2^b\,\phi_0\phi .
$$

*Ladder sum (3.1)–(3.4).*
$$
iM_n=4s\frac{(i\chi)^n}{n!},\qquad \chi=-\tfrac14\gamma^2s\,f_\ell(0),\qquad iM=4s\,(e^{i\chi}-1),
$$
with $s=p^1_xp^2_y$. The reader notes an internal sign inconsistency in the middle expression of (3.1); the tree level agrees with the right-hand side.

*In–out relation (3.5).*
$$
y_{\rm out}=\tilde\lambda\,p_{\rm in},\qquad \tilde\lambda=\frac{8\pi G}{\ell^2+\ell+2}.
$$
- The authors say this differs from 't Hooft "in the pre-factor" and that "both results are indeed correct".
- Restricting the graviton to shock-wave profiles recovers $\ell^2+\ell+1$ (shown in the companion paper). Equation (3.5) instead includes "arbitrary off-shell graviton fluctuations".

**Other statements in the paper**
- Low $\ell$ dominates, unlike flat space where large $\ell$ dominates.
- "No momentum is transferred to or from the infalling observer."
- Strings appear only as a future direction: transverse momentum transfer "may be tractable by including a B-field", citing de Haro's *Noncommutative black hole algebra*.
- **Future work** listed: a CFT calculation of (3.4) for small black holes in AdS/CFT.

**Not in the paper:** a commutator, scrambling or time delay, an uncertainty relation, AdS/CFT, the Regge trajectory, or out-of-time-order correlators. The word "firewall" does not appear in v3.

**Relevance** [inference]
- **Implied commutator.** With canonical $[x_{\rm in},p_{\rm in}]=i$, (3.5) implies
  $$
  [x_{\rm in},y_{\rm out}]=\frac{8\pi iG}{\ell^2+\ell+2}\qquad\text{vs. 't Hooft's}\qquad \frac{8\pi iG}{\ell^2+\ell+1}.
  $$
  The ratio is $1/2$ at $\ell=0$, $3/4$ at $\ell=1$, and tends to 1 as $\ell\to\infty$.
- **Consequence for $F$.** The normalization of $F$ in $[X^+,X^-]=8\pi iGF$ depends on whether the shock-wave or the soft off-shell kernel is used. The difference is $O(1)$ at low $\ell$, which dominates. Whether an analogous shift arises in AdS (for $\Pi_3$) is unchecked.
- **Regime differences.** Pure Einstein gravity, asymptotically flat 4d, leading order in $s$; no stringy corrections.
- **Positive role.** The paper's listed future work (the AdS/CFT computation) is close to our program. Its non-Planckian energy condition supports a thermal $[U,V]$ without Planckian $s$.

---

## 5. D. Minic, "On the Space-Time Uncertainty Principle and Holography"

**Bibliographic data.** hep-th/9808035v1 (6 Aug 1998), preprint PSU/TH/204, 15 pp; Phys. Lett. B **442** (1998) 102–108.

**Summary.** A short, heuristic note supporting Li–Yoneya (hep-th/9806240): **the spacetime uncertainty principle implies holography**. That is the opposite direction to our program, which goes from AdS/CFT to an uncertainty relation.
- §2 reviews the spacetime uncertainty relation and an M-theory version.
- §3 (Matrix theory) obtains Bekenstein–Hawking scaling from Jevicki–Yoneya conformal symmetry plus the BBPT probe action, using virial and scaling arguments.
- §4 asserts that the Susskind–Witten UV–IR relation "is nothing but" the spacetime uncertainty relation, then repeats the Susskind–Witten counting.
- §5 speculates on background-independent holography via Crane–Baez 2-Hilbert spaces (13).

**Key equations**

*The relation itself (1).* From $\Delta T\Delta E\ge\hbar$ and $\Delta E\sim\hbar\,\Delta X/l_s^2$:
$$
\Delta T\,\Delta X\ge l_s^2 .
$$
- There is no $\pi$, and $T$ is "longitudinal (including time)".
- It is tied to the scalings $X\to\lambda X$ (2) and $\sigma\to\lambda^{-1}\sigma$ (3), read as "UV on world-volume = IR in target space".

*Covariant and Matrix-theory forms.*
$$
[X_\mu,X_\nu]^2\sim I\quad(6),\qquad \Delta X_-\,\Delta X_a\,\Delta X_+\sim l_{11}^3\quad(7),
$$
with $\alpha'=l_{11}^3/R$. Setting $\Delta X_-\sim R$ recovers (1).

*Couplings.*
- D0 scaling $X\to g_s^{1/3}X$, $t\to g_s^{-1/3}t$ (5).
- The paper prints "the scale $g_s^{-1/3}l_s$ is … the 11-d Planck length"; this is a typo for $g_s^{1/3}l_s$.

*Generalized conformal symmetry (8a,b), Jevicki–Yoneya SU(1,1).*
- Dilatation: $\delta_DX=X$, $\delta_Dt=-t$, $\delta_Dg_s=3g_s$.
- Special conformal: $\delta_KX=2tX$, $\delta_Kt=-t^2$, $\delta_Kg_s=6tg_s$.

*BBPT probe action (9a).*
$$
S=-\int\frac{dt}{g_sh(r)}\Big(\sqrt{1-h v^2}-1\Big),\qquad h=\frac{15N}{2g_s^5r^7}\ \text{(as printed)}.
$$

*Susskind–Witten counting.*
$$
N_{\rm dof}\sim\frac{N^2}{\delta^3}\ \ (10),\qquad R_b=l_s(g_sN)^{1/4}\ \ (12).
$$
More generally $N^{d/2}$ degrees of freedom for a $d$-dimensional CFT.

**Not in the paper:** no AdS radial coordinate, no Poincaré metric, no proper-versus-coordinate intervals, no W-boson masses or Peet–Polchinski. The identification of UV–IR with the uncertainty relation is made **only through the scaling (2)–(3)**.

**Relevance** [inference]
- **Our observation (a) is not here.** Minic and Li–Yoneya *assert* the qualitative UV–IR ↔ uncertainty-relation identification. Our identity $\Delta T_p\Delta Z_p=\Delta t\,\Delta r$, together with $E_W=r/2\pi\alpha'$, is a precise version of that assertion. Cite them for the assertion.
- **Our observation (b) is not stated.** However, (7) at fixed $\Delta X_a$ reads $\Delta X_+\Delta X_-\sim l_{11}^3/\Delta X_a$, which is invariant under longitudinal boosts. This is a hyperbola in flat 11d light-cone variables and worth citing as a precedent.
- (8a) is the generalized conformal symmetry used in our D0 section, and (5) gives $l_{11}=g_s^{1/3}l_s$.

---

## 6. T. Yoneya, "String Theory and the Space-Time Uncertainty Principle"

**Bibliographic data.** hep-th/0004074v6 (30 Mar 2001), 45 pp; Prog. Theor. Phys. **103** (2000) 1081–1125, DOI 10.1143/PTP.103.1081.

**Summary.** The review argues that the spacetime uncertainty relation $\Delta X\Delta T\gtrsim\ell_s^2$ is a universal, non-perturbative principle encoding worldsheet conformal symmetry.
- **§2:** two derivations; compatibility with Lorentz invariance; rejection of the "generalized uncertainty principle" form.
- **§3:** Borel-summed high-energy scattering.
- **§4:** combines the relation with a black-hole bound to obtain the M-theory scale; D-particles and generalized conformal symmetry; black-hole entropy, holography, UV–IR.
- **§5:** Schild-gauge noncommutativity.
- **§6:** dualities and an 11d form.

**Key equations**

*The relation (2.1)–(2.2).* From $\Delta E\Delta t\gtrsim1$ and the longitudinal extension $\Delta X\sim\ell_s^2\Delta E$:
$$
\Delta X\,\Delta T\gtrsim\ell_s^2 .
$$
**No constant is given.** In Yoneya's words, the principle "has yet only been qualitatively formulated. We cannot give a rigorous definition for the uncertainties ΔX and ΔT."

*Rejected generalized uncertainty principle (2.4).*
$$
|\delta x||\delta p|\gtrsim1+\ell_s^2|\delta p|^2 .
$$
It is rejected as non-universal; among other reasons, its minimal length would contradict the scale $g_s^{1/3}\ell_s$.

*Extremal-length derivation (§2.3).*
- Extremal length (2.7) and its reciprocity (2.8): $\lambda_\Omega(\Gamma)\lambda_\Omega(\Gamma^*)=1$.
- The path-integral factor $\exp[-\ell_s^{-2}(A^2/\lambda(\Gamma)+B^2/\lambda(\Gamma^*))]$ gives $\Delta A\,\Delta B\sim\ell_s^2$.
- It is "a natural generalization of modular invariance, or of open-closed string duality", and is independent of $g_s$.

*Lorentz invariance (§2.2).*
- Illustrative constraint (2.5): $\frac12[X^\mu,X^\nu]^2\sim\ell_s^4$.
- Its decomposition (2.6): $\sqrt{\langle-[X^0,X^i]^2\rangle}=\sqrt{\frac12\langle-[X^i,X^j]^2\rangle+\ell_s^4}\gtrsim\ell_s^2$.
- The relation holds in all frames "after averaging over the spatial directions".

*High-energy scattering (§3).* The Borel-summed amplitudes (3.15)–(3.16) give $\Delta T\Delta X\gtrsim\frac12\sqrt{f^2+f'^2}$ (3.21), which is $O(1)$ in string units.

*M-theory scale from gravitational collapse (§4.1).* The "black-hole uncertainty relation" is
$$
\delta T\,(\delta X)^7\gtrsim G_{10}\sim g_s^2\ell_s^8\ \ (4.1).
$$
Combined with $\Delta T\sim\ell_s^2/\Delta X$ (4.2), this gives
$$
(\Delta X_c)^6\sim g_s^2\ell_s^6\ \ (4.3),\qquad \Delta X_c\sim g_s^{1/3}\ell_s,\quad \Delta T_c\sim g_s^{-1/3}\ell_s\ \ (4.4),\qquad \ell_M=g_s^{1/3}\ell_s\ \ (4.5),
$$
"without invoking D-branes and string dualities directly". Fig. 1 shows the crossing of the two curves.

*D-particles (§4.2).*
- From the uncertainty relation, $\Delta X\gtrsim\sqrt v\,\ell_s$ (4.6); from wave-packet spreading, $\Delta X_w\sim(g_s/v)\ell_s$ (4.7).
- Together: $\Delta X\sim g_s^{1/3}\ell_s$ (4.8) and $\Delta T\sim g_s^{-1/3}\ell_s$ (4.9).
- A holographic count gives one bit per $\ell_{11}^9$.
- Saturation is expected only for BPS systems or systems with generalized conformal symmetry; D0–anti-D0 does not saturate.

*Generalized conformal symmetry (4.10)–(4.12).* The D0 matrix action (4.10) is invariant under
$$
X\to\lambda X,\quad t\to\lambda^{-1}t,\quad g_s\to\lambda^3g_s\ \ (4.11),\qquad
\delta_KX=2\epsilon tX,\quad \delta_Kt=-\epsilon t^2,\quad \delta_Kg_s=6\epsilon tg_s\ \ (4.12),
$$
with $\ell_s$ fixed; together with time translations these form $SO(2,1)$.
- "The product δXδt of small variations is invariant under the above transformations, suggesting that the generalized conformal symmetry may be a part of a more general set of transformations which characterize the algebraic structure associated with the space-time uncertainty relations."
- The two-body effective action is (4.13), whose leading term is $v^4/r^7$.

*AdS/CFT and UV–IR (§4.3).*
- "The space-time uncertainty relation for open strings mediating D-branes leads to a similar relation that a small spatial uncertainty ΔX in the bulk corresponds to large uncertainties ΔT along the time-like direction on the brane at the boundary." The two "seem to be equivalent".
- A "small discrepancy": UV–IR involves $R_{\rm ads}\sim(g_sN)^{1/4}\ell_s$, while the uncertainty relation involves only $\ell_s$.
- He resolves it "as suggested essentially in" Peet–Polchinski, with $\Delta T\sim\Delta X_{\rm brane}/\sqrt{g_sN}$ (4.18). This gives $\Delta X_{\rm bulk}\Delta X_{\rm brane}\sim R_{\rm ads}^2$, the relation used by Susskind–Witten and Peet–Polchinski.
- He then counts $N_{\rm dof}\sim N^2L^3/R_c^3$.
- Black-hole entropy: $S\sim R_SM$ (4.14)–(4.17), linked to complementarity.
- Holography and UV–IR are "macroscopic"; the uncertainty relation is "microscopic".
- The sentence "naturally explains the UV/IR relation … Susskind and Witten", which a search snippet had attributed to this paper, is **not** in it.

*Schild-gauge noncommutativity (§5),* with $\lambda=4\pi\alpha'$.
- Introducing $b_{\mu\nu}$, the constraint gives $b_{0i}^2=\lambda^2+\frac12b_{ij}^2\ge\lambda^2$, so the time–space components dominate.
- In the gauge $\partial_\sigma X^0=0$:
$$
\Big[X^0,\int d\sigma\,S_{ri}\,\partial_\sigma X^i\Big]=i\lambda\ \Rightarrow\ |\Delta X^0|\,|\Delta\vec X|\gtrsim\lambda\ \ (5.12).
$$

*11d forms (6.3)–(6.4).*
$$
\Delta T\,\Delta\vec X\,\Delta X_{11}\gtrsim\ell_M^3\sim G_{11},\qquad \Delta T\,(\Delta X)^8\gtrsim\ell_M^9 .
$$

**Relevance** [inference]
- **(a) Partly anticipated.** §2.1 already presents the uncertainty relation as Heisenberg applied to string extension. §4.3 calls it "equivalent" to UV–IR for open strings stretched to D-branes, crediting Peet–Polchinski. Absent from the paper: Poincaré coordinates, the exact identity $\Delta T_p\Delta Z_p=\Delta t\,\Delta r$ with $R$ cancelling, $E_W=r/2\pi\alpha'$, and any constant. Our identity is the exact, $R$-free bulk version of his "seem to be equivalent". It also answers his "small discrepancy" directly: no $R_{\rm ads}$ appears.
- **(b) Not stated.** His covariant form (2.5)–(2.6) differs from ours. The §5 footnote says the worldsheet bivector can be rotated into a timelike 2-plane with "only one independent Lorentz invariant". On that plane the invariant is $\propto(\Delta X^+\Delta X^-)^2$, so it is compatible with (b), but the light-cone form and the uniqueness argument are ours.
- **(c) Already there, essentially verbatim:** the crossover (4.1)–(4.5) and Fig. 1, independently confirmed in (4.6)–(4.9). Differences: his $\Delta X$ is a flat-space resolution rather than a radial $\Delta r$, and no $N$ appears. The general form $\Delta t\,\Delta U\ge\mathcal F(g_{\rm eff}^2)$ with $g_{\rm eff}^2=g_{YM}^2N/U^3$ is **not** in the paper.
- **No constant.** Our $\pi\alpha'$ is a convention; Minic and Yoneya both write $\ell_s^2$.

---

## Consequences for the working note

**1. Prior art**

| Item in the working note | Status in the literature | What remains new |
|---|---|---|
| §3.0(a): time–radial uncertainty ⇔ boundary Heisenberg | Qualitative versions in Li–Yoneya, Minic, Yoneya (2000) §4.3 | The exact identity $\Delta T_p\Delta Z_p=\Delta t\,\Delta r$, which resolves Yoneya's "$R_{\rm ads}$ discrepancy" |
| §3.0(b): Lorentz-covariant hyperbola | Precedents in Minic (7) (boost-invariant at fixed $\Delta X_a$) and Yoneya (2000) §5 (one invariant on a timelike 2-plane) | The explicit statement and uniqueness argument |
| §3.4: D0 crossover at $\ell_{11}$ | Yoneya (2000) (4.1)–(4.5), essentially verbatim | The form $\Delta t\,\Delta U\ge\mathcal F(g_{\rm eff}^2)$, which is not in Yoneya (2000), Minic or Li–Yoneya |
| §3.1–3.2: light-cone commutator from CFT Regge data with stringy smoothing | **Not found in any of the six papers** | The proposal itself |

Ingredients for §3.1–3.2 exist separately in the literature:
- the CFT Regge phase (Cornalba; Cornalba–Costa–Penedones);
- 't Hooft's horizon algebra in flat space (Gaddam–Groenenboom–'t Hooft; Kiem–Verlinde–Verlinde);
- its S-matrix and out-of-time-order reading (Polchinski).

**2. Physics corrections to adopt**
1. $\tau_s\to(\ln s+\gamma_E)/2\sqrt\lambda$. The full cutoff is complex, $\tilde\tau_s=(\ln s+\gamma_E-i\pi/2)/2\sqrt\lambda$. Sign convention: $\delta=-2\pi\Gamma_{\rm Cornalba}$.
2. **Normalization of $F$:** shock-wave versus soft off-shell kernels differ by $O(1)$ at low $\ell$ ($\ell^2+\ell+1$ vs. $\ell^2+\ell+2$). Fix conventions by redoing the shock in our coordinates. Polchinski's $16\pi G\,r_s^2/g_{uv}$ is another normalization to match.
3. **State and ordering:** state $\Delta X^+\Delta X^-\ge4\pi G|F|$ for amplitudes or out-of-time-order correlators, not as variances in the Hartle–Hawking or Unruh state. The thermal $[U,V]$ is valid only for $t\lesssim t_{\rm scr}$.
4. **All-$\lambda$ extension:** at weak coupling the leading phase is purely absorptive and $j\approx1$. A real commutator starts only at $O(g^2)$ and grows as $s^{\bar\alpha\chi}$. The finite-coupling trajectory $j(\nu)$ is needed beyond $\nu\approx0$.

**3. Still open**
- The $(4g)^{-\alpha'q^2/2}$ scale issue: check BPST, hep-th/0603115.
- What changed in Polchinski's (2.18) between v1 and v2.
- Whether an $\ell^2+\ell+2$-type shift appears for the AdS kernel $\Pi_3$.
- A wider literature search: Shenker–Stanford (2014), He–Raclariu–Zurek (2305.14411), and recent work on 't Hooft commutators in AdS.

## Links
- Cornalba, [arXiv:0710.5480](https://arxiv.org/abs/0710.5480)
- Cornalba–Costa–Penedones, [arXiv:0801.3002](https://arxiv.org/abs/0801.3002)
- Polchinski, [arXiv:1505.08108](https://arxiv.org/abs/1505.08108); TASI review [arXiv:1609.04036](https://arxiv.org/abs/1609.04036)
- Gaddam–Groenenboom–'t Hooft, [arXiv:2012.02357](https://arxiv.org/abs/2012.02357); companion [arXiv:2012.02355](https://arxiv.org/abs/2012.02355)
- Minic, [hep-th/9808035](https://arxiv.org/abs/hep-th/9808035)
- Yoneya, [hep-th/0004074](https://arxiv.org/abs/hep-th/0004074)
- Related:
  - Li–Yoneya, [hep-th/9806240](https://arxiv.org/abs/hep-th/9806240)
  - Jevicki–Yoneya, [hep-th/9805069](https://arxiv.org/abs/hep-th/9805069)
  - Kiem–Verlinde–Verlinde, [hep-th/9502074](https://arxiv.org/abs/hep-th/9502074)
  - BPST, [hep-th/0603115](https://arxiv.org/abs/hep-th/0603115)
