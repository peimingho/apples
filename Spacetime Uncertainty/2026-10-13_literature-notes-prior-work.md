# Literature notes: prior work for "a spacetime uncertainty relation from AdS/CFT"

*Compiled 2026-10-13. Companion to `2026-10-13_holography-strings-and-SUR-from-AdS-CFT.md`.*

> **Access caveat.** This session's network policy blocks arxiv.org and its mirrors, INSPIRE and the publishers. Only one paper (Cornalba, 0710.5480) was read in full. The others rest on abstracts, search-engine summaries, or a secondary source. The table records what was actually read.
>
> - Statements marked **[verified]** were checked against the full text or the abstract.
> - Statements marked **[snippet]** come from search summaries and may be wrong.
> - Statements marked **[ours]** are our own derivations or inferences.
>
> No equation is attributed to a paper unless it was read in the full text.

| # | Paper | What was read |
|---|---|---|
| 1 | Cornalba, arXiv:0710.5480 | **Full text (v3)** |
| 2 | Cornalba–Costa–Penedones, arXiv:0801.3002 | Abstract and metadata |
| 3 | Polchinski, arXiv:1505.08108 | Abstract, plus Polchinski's own description in his TASI review (1609.04036, §9.2) |
| 4 | Gaddam–Groenenboom–'t Hooft, arXiv:2012.02357 | Abstract-level snippets and descriptions in citing papers |
| 5 | Minic, hep-th/9808035 | Search summaries only |
| 6 | Yoneya, hep-th/0004074 | Abstract and metadata |

**Two attributions in the earlier note were wrong:**
1. **0710.5480 has a single author, L. Cornalba.** Costa and Penedones appear only in the acknowledgements.
2. **No paper by Gaddam, Groenenboom, 't Hooft *and* Verlinde was found** (a direct INSPIRE author query could not be run). The intended paper is almost certainly Gaddam–Groenenboom–'t Hooft, 2012.02357. "Verlinde" was probably a mix-up with Verlinde–Verlinde (1992) or Kiem–Verlinde–Verlinde (1995).

---

## 1. L. Cornalba, "Eikonal Methods in AdS/CFT: Regge Theory and Multi-Reggeon Exchange"

**Bibliographic data** [verified]
- arXiv:0710.5480 [hep-th, hep-ph]; v1 29 Oct 2007, v3 6 Oct 2008 ("added references and minor mistakes corrected"); 25 pp.
- Sole author: L. Cornalba (Milano-Bicocca / INFN).
- No journal reference in the arXiv metadata seen; not confirmed on INSPIRE.

**Summary** [verified]
- **Setting.** A Regge theory for CFT four-point functions $\langle O_1O_2O_1O_2\rangle$ in the Lorentzian regime $\sigma\to0$, where each T-channel partial wave behaves as $\sigma^{1-J}$ and the highest spins dominate.
- **Regge pole.** A Sommerfeld–Watson transform in complex $J$, using harmonic analysis on the transverse $H_3$, gives a Regge pole $J=j(\nu)$.
- **Eikonalization.** The pole is rewritten in impact-parameter space, and multi-reggeon exchange is resummed by exponentiating the tree-level phase shift, by analogy with Amati–Ciafaloni–Veneziano.
- **$\mathcal N=4$ SYM at strong coupling.** $j(\nu,g)$ and the residue $\beta(\nu,g)$ are fixed to leading order in string corrections by matching to the flat-space Virasoro–Shapiro amplitude. This reproduces and extends Brower–Polchinski–Strassler–Tan.

**Key equations** [verified; equation numbers are the paper's; $d=4$]

*Kinematics.*
- Position space: $z=\frac\sigma4e^{\rho}$, $\bar z=\frac\sigma4e^{-\rho}$, where $\rho$ is a geodesic distance on $H_3$.
- Impact-parameter space: $h^2=\frac s4e^{r}$, $\bar h^2=\frac s4e^{-r}$, with $s=4|\mathbf y||\bar{\mathbf y}|$ **dimensionless**. In the flat limit $s/\ell^2\to S$, the flat Mandelstam variable.
- Phase convention: $(-)^\alpha\equiv e^{i\pi\alpha}$.

*Impact-parameter representation, (7)–(9).*
$$
A(\mathbf x,\bar{\mathbf x})=(-)^{-\Delta_1}(-)^{-\Delta_2}\!\int_M d\mathbf y\,d\bar{\mathbf y}\;e^{-2i\mathbf x\cdot\mathbf y-2i\bar{\mathbf x}\cdot\bar{\mathbf y}}\,\mathcal B,\qquad \mathcal B=e^{-2\pi i\Gamma(h,\bar h)}.
$$
$\Gamma$ is identified both with the AdS phase shift ($-\pi\Gamma$) and with the anomalous dimension ($2\Gamma$) of $O_1\partial\cdots\partial O_2$ at large energy and spin.

*$H_3$ harmonic analysis, (11)–(16).*
$$
\Pi_E=\frac{e^{-E\rho}}{4\pi\sinh\rho},\quad [\Box_{H_3}-E^2+1]\Pi_E=-\delta,\quad
\Omega_E=\frac{E}{2\pi}(\Pi_E-\Pi_{-E}),\quad \Pi_E=\int d\nu\,\frac{\Omega_{i\nu}}{\nu^2+E^2}.
$$

*Regge pole, (21)–(25) and (29).*
$$
\mathcal B\simeq-2\pi i\!\int d\nu\,\beta(\nu)\,s^{\,j(\nu)-1}\,\Omega_{i\nu}(r),\qquad
\Gamma(s,r)\simeq\int d\nu\,\beta(\nu)\,s^{\,j(\nu)-1}\,\Omega_{i\nu}(r).
$$
The even-signature factor sits in $\alpha(\nu)\propto(-)^{\frac{2-j}{2}}r_+/\sin(\pi j/2)$, with $\alpha=V_1\beta V_2$.

*$\mathcal N=4$ dictionary (§5).* $g=\ell^2/\alpha'=\sqrt\lambda$ and $1/N^2=2G/(\pi\ell^3)$. The phase shift is
$$
\Gamma_{\rm sugra}=-\frac{2G}{\ell^3}\,s\,\Pi_2(r)=-\frac{2G}{\ell^3}\,s\!\int\!\frac{d\nu}{\nu^2+4}\,\Omega_{i\nu}(r),\qquad
\Gamma_{\rm string}=-\frac{2G}{\ell^3}\!\int d\nu\,\beta(\nu,g)\,s^{\,j(\nu,g)-1}\,\Omega_{i\nu}(r).
$$

*Trajectory, (31)–(33).*
$$
j\to2-\frac{\alpha'}2q^2\ \ (\nu=\ell q,\ \ell\to\infty),\qquad j(\pm2i,g)=2,
$$
$$
j(\nu,g)=2-\frac{4+\nu^2}{2g}-(4+\nu^2)\sum_{n\ge2}\frac{\tilde j_n(\nu)}{g^n},
$$
where $\tilde j_n$ is an even polynomial of degree $2n-4$.

*Residue (p. 19, unnumbered).*
$$
\beta(\nu,g)=-\frac1{4g}\,(-)^{-j/2}\,\frac{\Gamma(1-j/2)}{\Gamma(j/2)}+\cdots
$$
It is fixed by matching to Virasoro–Shapiro.

**Validity** [verified]
- Lorentzian $\sigma\to0$.
- String tree level ($N\to\infty$).
- Large impact parameter.
- Leading Regge pole only, with reggeon self-interactions neglected.
- $g\to\infty$ at fixed $\nu$.

**Not in the paper** [verified by full-text search]
- Light-cone commutators, time delays, uncertainty relations.
- Heat-kernel / proper-time form.
- Transverse diffusion.
- Any discussion of $\mathrm{Im}\,\Gamma$.

**Check of our working proposal** [ours, checked by reader]

1. **Trajectory: agrees.** $j=2-\frac{\nu^2+4}{2\sqrt\lambda}+O(\lambda^{-1})$. The $O(\lambda^{-1})$ term is also $\propto(4+\nu^2)$, so the proper-time form survives at that order with a renormalized $\tau_s$.

2. **Phase-shift structure: agrees, with a correction.** Expanding $\beta$ with $\epsilon=(4+\nu^2)/2g$:
   $$
   \beta=\frac1{\nu^2+4}+\frac{i\pi-2\gamma_E}{4g}+O\!\Big(\frac{4+\nu^2}{g^2}\Big)
   \ \Rightarrow\
   \beta\,s^{j-2}\simeq\frac{e^{-(\nu^2+4)\tilde\tau_s}}{\nu^2+4},\qquad
   \tilde\tau_s=\frac{\ln s+\gamma_E-i\pi/2}{2\sqrt\lambda}.
   $$
   This gives a **complex proper-time cutoff**:
   $$
   \Gamma\simeq-\frac{2Gs}{\ell^3}\int_{\tilde\tau_s}^\infty d\tau\,e^{-3\tau}K_{H_3}(\tau;r),\qquad
   K_{H_3}=\int d\nu\,\Omega_{i\nu}\,e^{-\tau(1+\nu^2)}.
   $$
   - $\mathrm{Re}\,F$ is our proper-time-cutoff propagator with $\ln s\to\ln s+\gamma_E$.
   - $\mathrm{Im}\,\Gamma=-\frac{2Gs}{\ell^3}\frac{\pi}{4\sqrt\lambda}e^{-3\tau_s}K_{H_3}(\tau_s;r)<0$, so $|\mathcal B|<1$ (absorption).
   - The paper's $\Pi_2$ is our $\Pi_3$.

3. **Sign and normalization.** The physical eikonal phase is $\delta\equiv-2\pi\Gamma_{\rm Cornalba}=+4\pi G\,s\,\Pi/\ell^3$. It equals our $4\pi G_5\,S\,\Pi_3/R$ once $s=\ell^2S$. The sign difference with our note is only a convention for $\Gamma$.

4. **Open scale issue.** With $s/\ell^2\to S$, $s^{j-2}\to(\ell^2S)^{-\alpha'q^2/2}$, whereas Virasoro–Shapiro gives $(\alpha'S/4)^{-\alpha'q^2/2}$. The ratio $(4g)^{-\alpha'q^2/2}$ is not addressed by the matching. If this factor belongs in $\beta$, then $\tau_s\propto\ln(s/4\sqrt\lambda)$ and $\langle b^2\rangle=3\alpha'\ln(s/4\sqrt\lambda)$. **Check against BPST (hep-th/0603115).**

**Relevance.** This is the input for Step 3 of our proposal, the stringy smoothing. On novelty: nothing here pre-empts the light-cone commutator or uncertainty-relation interpretation.

---

## 2. L. Cornalba, M. S. Costa, J. Penedones, "Eikonal Methods in AdS/CFT: BFKL Pomeron at Weak Coupling"

**Bibliographic data** [verified at metadata level]
- arXiv:0801.3002 [hep-th]; v1 19 Jan 2008, v2 30 Sep 2008.
- JHEP **06** (2008) 048. The DOI is presumably 10.1088/1126-6708/2008/06/048 (not confirmed).

**Summary** [verified, abstract]
- Planar $\mathcal N=4$ correlators $\langle O_1O_2O_1^*O_2^*\rangle$ in the Lorentzian regime dual to high-energy scattering in AdS.
- The planar amplitude is dominated by **one Regge pole for all $\lambda$**: graviton exchange in AdS at strong coupling, the hard BFKL pomeron at weak coupling.
- The authors work at weak coupling in position space. They use the conformal symmetry of the transverse $\mathbb E_2$, whose holographic image is $H_3$, so one formalism covers both regimes. Impact factors are tightly fixed by conformal invariance.
- They propose ("suggest", not derive) an AdS eikonal resummation of multi-pomeron exchange that implements AdS unitarity and differs from 4d eikonal exponentiation.

**Not verified:** all equations, the $\nu$ normalization of the weak-coupling $j(\nu)$, the impact factors, and the resummation formula.

For orientation, here is the standard LO BFKL form from general literature (not checked in this paper):
$$
\omega=\bar\alpha\,\chi(\nu_B),\qquad \bar\alpha=\frac{\lambda}{4\pi^2},\qquad \chi(\nu_B)=2\psi(1)-\psi(\tfrac12+i\nu_B)-\psi(\tfrac12-i\nu_B).
$$
With the $H_3$ normalization one expects $\nu=2\nu_B$. Intercepts: $j(0)\simeq1+\frac{\lambda}{\pi^2}\ln2$ at weak coupling, and $j(0)\simeq2-2/\sqrt\lambda$ at strong coupling.

**Relevance** [ours]
- It confirms that the $H_3$ impact-parameter language is defined at every coupling, from transverse conformal symmetry alone. That is the basis for an all-$\lambda$ version of $F$.
- Obstacles at weak coupling:
  1. The intercept is $\approx1$, so the phase scales as $s^{\bar\alpha\chi}$ rather than $s^1$. The "commutator" picks up an energy-dependent effective $G$.
  2. $H_3$ is kinematic (operator/dipole scale), not a local bulk, so $X^\pm$ as bulk positions is only an interpretation.
  3. The resummation is conjectural.
  4. Cuts may spoil a simple single-pole picture.
- On novelty: the abstract does not mention commutators, time delays or uncertainty relations.

---

## 3. J. Polchinski, "Chaos in the black hole S-matrix"

**Bibliographic data** [verified]
- arXiv:1505.08108 [hep-th, gr-qc]; 13 pp, 2 figures.
- v2 comment: "correction to eq. 2.18 and added clarification (new footnote 6)".
- No journal reference found; the work is cited as arXiv-only in his 2016 TASI review.

**Abstract** [verified, quoted]
> "Recent work by Shenker, Stanford, and Kitaev has related the black hole horizon geometry to chaotic behavior. We extend this from eternal black holes to black holes that form and then evaporate. This leads to an identity for the change in the black hole S-matrix (over times shorter than the scrambling time) due an addition infalling particle, elaborating an idea of 't Hooft. There is a calculable effect on the outgoing particles that grows exponentially in time, reflecting the Lyapunov behavior, until the calculation breaks down roughly a scrambling time after the extra particle is thrown in."

**Polchinski's own gloss** [verified, TASI review 1609.04036, §9.2]
- 't Hooft's calculable S-matrix, "which moreover has stringy properties", comes from scattering right- and left-moving near-horizon modes.
- But by the adiabatic principle there should be no right-movers for an old black hole, "so this S-matrix should not exist".
- It can instead be given "a more limited interpretation in terms of chaos, using the out-of-time order property".
- Conclusion: "chaos again leads to the necessity of the firewall."

**Not verified:** the form of the commutation relations or S-matrix identity (eq. 2.18 is central and was corrected in v2), whether AdS appears (the framing suggests asymptotically flat space), and whether stringy corrections are treated.

**Relevance** [ours]
- It supports reading 't Hooft's algebra as a statement about out-of-time-order correlators. That is the thermal leg of our proposal (§3.2), with validity $t\lesssim t_*$.
- **Caveat for us:** if the algebra has meaning only out of time order, the bound $\Delta X^+\Delta X^-\ge4\pi G|F|$ must specify the state and operator ordering in which the variances are taken.
- On novelty: no light-cone uncertainty relation and no CFT Regge input appear in the verified material.
- The closer precedent for stringy smearing of the OTOC is Shenker–Stanford, *Stringy effects in scrambling* (JHEP 1505 (2015) 132).

---

## 4. N. Gaddam, N. Groenenboom, G. 't Hooft, "Quantum gravity on the black hole horizon"

**Bibliographic data** [snippet]
- arXiv:2012.02357 [hep-th]; v1 4 Dec 2020, v3 8 Jan 2022.
- JHEP **01** (2022) 023, DOI 10.1007/JHEP01(2022)023 (as cited by later papers).

**Summary** [snippet, abstract level]
- Scattering on a Schwarzschild horizon in a partial-wave basis, for impact parameters $b\lesssim R_S$ (with $b\gg\ell_{\rm Pl}$).
- An infinite set of virtual gravitons exchanged on the horizon is summed non-perturbatively in $\hbar$ and $\gamma\sim M_{\rm Pl}/M_{\rm BH}$. This generalizes the Dray–'t Hooft shockwave and 't Hooft's S-matrix.
- One version of the abstract states that the required energy is $s\gg\gamma^2M_{\rm Pl}^2$, not necessarily Planckian. Hence "infalling observers experience no firewalls". This was not checked against v3.
- Later papers describe it as reproducing 't Hooft's S-matrix mode by mode (eikonal resummation, even Regge–Wheeler gauge). They also say the Eisenbud–Wigner time delay equals the scrambling time when $E\sim M_{\rm BH}$.

**For orientation only** ('t Hooft's standard form, recalled and **not** checked in this paper):
$$
u^-_{\rm out}(\Omega)=8\pi G\!\int d^2\Omega'\,f(\Omega,\Omega')\,p^-_{\rm in}(\Omega'),\qquad (1-\Delta_\Omega)f=\delta^2(\Omega,\Omega'),
$$
$$
[u^+_{\ell m},u^-_{\ell'm'}]=\frac{8\pi i G}{\ell^2+\ell+1}\,\delta_{\ell\ell'}\delta_{mm'}\quad(R_S=1).
$$

**Related papers** [snippet; IDs and journal data unverified]
- Gaddam–Groenenboom, *Soft graviton exchange and the information paradox*, arXiv:2012.02355. Pure-phase "black hole eikonal" S-matrix from soft-graviton ladders.
- Gaddam–Groenenboom, *2→2N scattering: eikonalisation and the Page curve*, arXiv:2110.14673, JHEP 01 (2022) 146.
- Gaddam–Groenenboom, *A toolbox for black hole scattering*, arXiv:2207.11277. Near-horizon graviton propagator for all partial waves.
- Betzios–Gaddam–Papadoulaki, *The black hole S-matrix from quantum mechanics*, arXiv:1607.07885, JHEP 11 (2016) 131. 't Hooft's S-matrix as inverted harmonic oscillators, one per $(\ell,m)$.
- Groenenboom, *All elastic amplitudes in the (black hole) eikonal phase*, arXiv:2512.09445.
- Older background: Verlinde–Verlinde, hep-th/9110017; Kiem–Verlinde–Verlinde, hep-th/9502074. KVV find that, for an outside observer, the position of infalling matter becomes increasingly uncertain near the horizon. This is the closest older precedent for "uncertainty from horizon backreaction".

**Relevance** [ours]
- It is a QFT-in-Schwarzschild derivation of 't Hooft's horizon algebra, which supports the step "eikonal phase ⇔ algebra of $u^\pm$".
- Transverse-kernel dictionary: $(1-\Delta_{S^2})^{-1}$ (eigenvalues $\ell^2+\ell+1$) ↔ our $(-\Box_{H_3}+3)^{-1}$.
- **Differences from our program:** asymptotically flat, not AdS; pure gravity, with no stringy or Regge corrections; no CFT input; no uncertainty relation stated. Normalization conventions ($\kappa^2=32\pi G$, factors of $R_S$) must be matched before quoting numbers.

---

## 5. D. Minic, "On the Space-Time Uncertainty Principle and Holography"

**Bibliographic data** [snippet; consistent across sources]
- arXiv:hep-th/9808035; submitted 6 Aug 1998; preprint PSU/TH/204; 15 pp.
- Phys. Lett. B **442** (1998) 102–108, DOI 10.1016/S0370-2693(98)01203-9.

**Summary** [snippet]
- The paper collects further evidence for the Li–Yoneya claim (hep-th/9806240) that the spacetime uncertainty principle implies holography. It does so in Matrix theory and in AdS/CFT.
- Central statement: the SUR ties the **UV behaviour of the boundary Dp-brane world-volume theory** to the **IR behaviour of the bulk**, and this UV/IR link implies holography (Susskind–Witten).
- The stated origin is the opposite scaling of the longitudinal (time-including) and transverse directions of strings and D-branes.
- Form used: $\Delta T\,\Delta X\gtrsim\ell_s^2$ (paraphrase). The Matrix-theory form $\Delta X_T\,\Delta t\gtrsim\ell_p^3/R$ is stated in Li–Yoneya; whether Minic writes it is not confirmed.

**Not verified:** any explicit $N$, $g_s$ or $\lambda$ dependence; a covariant ($\Delta X^+\Delta X^-$) form; whether his $\Delta X$ is radial or transverse.

**Relevance** [ours]
- Our §3.0(a), "the time–radial SUR ⇔ boundary Heisenberg with the stringy UV/IR relation", is the same physics. It should be credited to Li–Yoneya (1998) and Minic (1998).
- Our exact cancellation $\Delta T_p\Delta Z_p=\Delta t\,\Delta r$ (no AdS radius $R$ left) may answer an objection Yoneya raised in 2000 [snippet]: that the UV/IR relation uses the curvature scale $R$, while the SUR uses only $\ell_s$.
- No sign of our §3.0(b), the Lorentz-covariant hyperbola.

---

## 6. T. Yoneya, "String Theory and the Space-Time Uncertainty Principle"

**Bibliographic data** [verified at metadata level]
- arXiv:hep-th/0004074; submitted 11 Apr 2000; v6 (Mar 2001) corrects typos; 45 pp.
- Prog. Theor. Phys. **103** (2000) 1081–1125, DOI 10.1143/PTP.103.1081. Invited paper.

**Summary** [verified, abstract]
- **Review.** It reviews the origin and derivation of the SUR, $\Delta T\,\Delta X\gtrsim\ell_s^2$, "in a reasonably self-contained way".
- **High-energy scattering.** It argues that high-energy string scattering, with all loop orders Borel-summed, is consistent with the SUR.
- **Central claim.** 10d string theories have a characteristic scale equal to the 11d Planck length, $g_s^{1/3}\ell_s$, where stringy effects take over from classical supergravity. The argument needs no D-branes.
- **D-branes and black holes.** It reinterprets the SUR for D-branes and black holes.
- **Noncommutativity.** It proposes a noncommutative reading of the Schild-gauge string action, with the time coordinate and the space coordinates failing to commute.

**Not verified:**
- which derivation of the SUR is used (conformal invariance, modular invariance, extremal length);
- the numerical constant on its right-hand side;
- whether the body discusses generalized conformal symmetry or AdS/CFT and UV/IR.

The sentence "the space-time uncertainty relation naturally explains the UV/IR relation used … by Susskind and Witten" may belong to Li–Yoneya (1998) rather than this paper. Check it.

**Relevance** [ours]
- Our §3.4 crossover, $\Delta t\,\Delta r^7\gtrsim G_{10}$ meeting $\Delta t\,\Delta r\gtrsim\alpha'$ at $\Delta r\sim g_s^{1/3}\ell_s=\ell_{11}$, has the same endpoint as this paper's central claim. **Assume it is already here (and in Li–Yoneya)** until checked.
- The symmetry argument $\Delta t\,\Delta U\ge\mathcal F(g_{\rm eff}^2)$ should be compared with Jevicki–Yoneya, *Space-time uncertainty principle and conformal symmetry in D-particle dynamics* (hep-th/9805069), and its follow-ups (Jevicki–Kazama–Yoneya; Yoneya's work on generalized conformal symmetry and Matrix theory).

---

## Consequences for the working note

1. **Attributions corrected:** 0710.5480 is by Cornalba alone. "Gaddam–Groenenboom–'t Hooft–Verlinde" should read Gaddam–Groenenboom–'t Hooft (2012.02357).
2. **Points that are probably prior art:**
   - §3.0(a), the time–radial SUR as boundary Heisenberg: Li–Yoneya and Minic (1998).
   - The D0 crossover in §3.4: Yoneya (2000) and Li–Yoneya.
3. **Main proposal (§3.1–3.2), status of novelty:** none of the six papers derives a light-cone commutator or uncertainty relation from CFT Regge data with stringy smoothing.
   - Ingredients that exist: the CFT Regge phase shift (Cornalba; Cornalba–Costa–Penedones), 't Hooft's horizon algebra in flat space (Gaddam–Groenenboom–'t Hooft; KVV), and its out-of-time-order reading (Polchinski).
   - This is not a full literature search. Also check Shenker–Stanford (2014), He–Raclariu–Zurek (arXiv:2305.14411, shockwave and soft/memory commutators), and recent work on 't Hooft commutators in AdS.
4. **Physics corrections to §3.1 Step 3:**
   - $\tau_s\to(\ln s+\gamma_E)/(2\sqrt\lambda)$; the full cutoff is complex, $\tilde\tau_s=(\ln s+\gamma_E-i\pi/2)/(2\sqrt\lambda)$.
   - Sign convention: $\delta=-2\pi\Gamma_{\rm Cornalba}$.
   - Open: possible $\ln(4\sqrt\lambda)$ shift in the scale of $s$ (check BPST).
5. **Conceptual caveat (Polchinski):** state the ordering and state in which $\Delta X^\pm$ are defined (OTOC vs. time-ordered).

## To do

1. **Get the full texts** of items 2–6. Either allow `arxiv.org` in the environment's Network access settings, or add the PDFs to Google Drive or this folder.
2. Then verify:
   - Polchinski eq. (2.18);
   - Gaddam–Groenenboom–'t Hooft's commutator normalization;
   - Minic's covariant/radial form;
   - Yoneya's AdS/CFT section and the $\ell_{11}$ argument;
   - Cornalba–Costa–Penedones's weak-coupling $j(\nu)$ normalization.
3. Resolve the $(4g)^{-\alpha'q^2/2}$ scale issue against BPST (hep-th/0603115).

## Links

- Cornalba, [arXiv:0710.5480](https://arxiv.org/abs/0710.5480)
- Cornalba–Costa–Penedones, [arXiv:0801.3002](https://arxiv.org/abs/0801.3002)
- Polchinski, [arXiv:1505.08108](https://arxiv.org/abs/1505.08108); TASI review [arXiv:1609.04036](https://arxiv.org/abs/1609.04036)
- Gaddam–Groenenboom–'t Hooft, [arXiv:2012.02357](https://arxiv.org/abs/2012.02357)
- Minic, [hep-th/9808035](https://arxiv.org/abs/hep-th/9808035)
- Yoneya, [hep-th/0004074](https://arxiv.org/abs/hep-th/0004074)
- Related:
  - Li–Yoneya, [hep-th/9806240](https://arxiv.org/abs/hep-th/9806240)
  - Jevicki–Yoneya, [hep-th/9805069](https://arxiv.org/abs/hep-th/9805069)
  - Kiem–Verlinde–Verlinde, [hep-th/9502074](https://arxiv.org/abs/hep-th/9502074)
  - Verlinde–Verlinde, [hep-th/9110017](https://arxiv.org/abs/hep-th/9110017)
  - BPST, [hep-th/0603115](https://arxiv.org/abs/hep-th/0603115)
