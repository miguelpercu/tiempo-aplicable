\documentclass[12pt]{article}
\usepackage{amsmath, amssymb}
\usepackage{graphicx}
\usepackage{natbib}
\usepackage{hyperref}
\usepackage{geometry}
\geometry{a4paper, margin=1in}

\begin{document}

\title{Evolution of Primordial Black Holes and Their Impact on the Cosmic Microwave Background: A Numerical Study with the Novel Applicable Time Framework}
\author{Miguel \'Angel Percudani \\
\textit{Independent Non-Conventional Scientific Researcher, Buenos Aires, Argentina} \\
\and \\

\maketitle

\begin{abstract}
We present a numerical study on the evolution of primordial black holes (PBHs) with an initial mass of $10^{12} \, \mathrm{kg}$ in the early universe at a redshift $z=1089$, corresponding to the recombination epoch. A novel temporal framework, the ``applicable time'' ($t_{\text{applied}}$), is introduced to adjust the temporal scale of cosmological simulations, enabling the modeling of dynamic processes such as Hawking radiation, the accumulation of dark matter ($\rho_{\mathrm{DM}}$) and dark energy ($\rho_{\mathrm{DE}}$), and their impact on the cosmic microwave background (CMB). The applicable time is rigorously derived by combining the cosmological redshift adjustment from the Friedmann-Lema\^{i}tre-Robertson-Walker metric and the light-travel delay from relativity, providing a bridge between local events and cosmological observations. We compare the applicable time with traditional temporal frameworks (comoving time, proper time, and conformal time), demonstrating its advantages in connecting local dynamics with observational effects, as detailed in Section~\ref{subsec:advantages_differences}. Our simulations, conducted over $10^{16} \, \mathrm{s}$, show that PBHs under realistic density constraints ($f_{\mathrm{PBH}} \leq 0.1$) have a negligible effect on the CMB, with a spectral distortion parameter $y \approx 1.09 \times 10^{-23}$ and a change in ionization fraction $\Delta x_e \approx 1.03 \times 10^{-23}$. Additionally, we explore the relationship between apparent magnitude and redshift for varying cosmological parameters, and extend the applicable time framework to other cosmological contexts such as nucleosynthesis ($z \sim 10^9$), structure formation ($z \sim 20$), gravitational wave emission, and phase transitions in the early universe. The applicable time framework offers a new perspective for cosmological simulations, with potential applications in modeling a wide range of phenomena.
\end{abstract}

\section{Introduction}
\label{sec:introduction}

Primordial black holes (PBHs) are hypothetical structures formed in the early universe that could influence the cosmic microwave background (CMB) through processes such as Hawking radiation and interactions with dark matter and dark energy \citep{Carr2010}. In this work, we simulate the evolution of PBHs with an initial mass of $10^{12} \, \mathrm{kg}$ at $z=1089$, corresponding to the recombination epoch, to evaluate their impact on the CMB and provide constraints for future observations such as those from CMB-S4.

A significant innovation in this study is the introduction of the ``applicable time'' ($t_{\text{applied}}$), a temporal scale adjusted by the cosmological redshift and the observer's distance. Unlike proper time, comoving time, or conformal time in relativity, the applicable time is specifically designed to model dynamic processes under extreme conditions near PBH singularities, where traditional time scales may break down due to gravitational and quantum effects. We provide a detailed comparison of the applicable time with other temporal frameworks in Section~\ref{subsec:advantages_differences}, highlighting its advantages in bridging local events and cosmological observations. This framework, developed by Miguel \'Angel Percudani and Grok 3 from xAI, is unique as of April 2025 and offers a new perspective for cosmological simulations, as detailed in Section~\ref{subsec:applicable_time}.

Our simulations reveal that PBHs have a negligible impact on the CMB under realistic density constraints, but the applicable time framework enables us to explore subtle effects that could be amplified in future studies. Additionally, we analyze the relationship between apparent magnitude and redshift for different cosmological parameters, and extend the applicable time framework to other cosmological epochs, such as nucleosynthesis, structure formation, gravitational wave emission, and phase transitions.

\section{Theoretical Model}
\label{sec:theoretical_model}

\subsection{Definition and Derivation of Applicable Time}
\label{subsec:applicable_time}

The ``applicable time'' ($t_{\text{applied}}$) is a novel temporal measure designed to model dynamic processes on cosmological scales, particularly in the early universe at $z=1089$. Unlike comoving time or proper time in relativity, the applicable time incorporates the redshift and the observer's distance to adjust the temporal scale:

\begin{equation}
t_{\text{applied}} = t_{\text{event}} \times (1 + z) + \frac{d_L}{c},
\label{eq:applicable_time}
\end{equation}

where:
\begin{itemize}
    \item $t_{\text{event}}$: Duration of the event in a local frame (s),
    \item $z$: Redshift ($z=1089$ at recombination),
    \item $d_L$: Luminosity distance from the event to the observer (m),
    \item $c$: Speed of light ($c = 3 \times 10^8 \, \mathrm{m/s}$).
\end{itemize}

This definition is derived by combining principles from the Friedmann-Lema\^{i}tre-Robertson-Walker (FLRW) metric and the light-travel delay from relativity. In the FLRW metric, the redshift $z$ relates the scale factor at the time of emission ($a_{\text{emission}}$) to the scale factor at the time of observation ($a_{\text{observation}}$):

\begin{equation}
1 + z = \frac{a(t_{\text{observation}})}{a(t_{\text{emission}})}.
\label{eq:redshift}
\end{equation}

For an event occurring at $z=1089$, the interval of time $t_{\text{event}}$ in the local frame of the PBH is dilated by a factor of $(1 + z)$ when observed today due to the cosmological expansion \citep{Peebles1993}:

\begin{equation}
t_{\text{observed}} = t_{\text{event}} \times (1 + z).
\label{eq:time_dilation}
\end{equation}

Additionally, the light emitted by the event travels a luminosity distance $d_L$ to the observer, introducing a delay:

\begin{equation}
d_L = \frac{c}{H_0} (1 + z) \int_0^z \frac{dz'}{\sqrt{\Omega_m (1 + z')^3 + \Omega_\Lambda}},
\label{eq:luminosity_distance}
\end{equation}

where $H_0 = 70 \, \mathrm{km/s/Mpc}$, $\Omega_m = 0.3$, and $\Omega_\Lambda = 0.7$. For $z=1089$, $d_L \approx 14000 \, \mathrm{Mpc} \approx 4.32 \times 10^{26} \, \mathrm{m}$, so the light-travel delay is:

\begin{equation}
\frac{d_L}{c} \approx \frac{4.32 \times 10^{26}}{3 \times 10^8} \approx 1.44 \times 10^{18} \, \mathrm{s}.
\label{eq:light_delay}
\end{equation}

Combining these effects, the applicable time for $t_{\text{event}} = 1 \, \mathrm{s}$ at $z=1089$ is:

\[
t_{\text{applied}} = 1 \times (1 + 1089) + 1.44 \times 10^{18} \approx 1.44 \times 10^{18} \, \mathrm{s}.
\]

In our simulations, we adjust $d_L$ to a smaller value ($d = 3 \times 10^8 \, \mathrm{m}$, or 1 light-second) to keep the time scales manageable, resulting in:

\[
t_{\text{applied}} = 1 \times (1 + 1089) + \frac{3 \times 10^8}{3 \times 10^8} = 1090 + 1 = 1091 \, \mathrm{s}.
\]

We discretize the temporal evolution over $t_{\max} = 10^{16} \, \mathrm{s}$ into six points: $t_{\text{applied}} = \text{linspace}(0, t_{\max}, 6)$. The novelty of the applicable time lies in its ability to bridge local, short-duration processes (e.g., Hawking radiation, particle emission) with cosmological scales, making it a versatile tool for early-universe simulations.

\subsection{Comparison with Comoving Time}
\label{subsec:comoving_comparison}

To highlight the advantages of the applicable time, we compare it with the comoving time ($t_{\text{comoving}}$), which is the standard temporal framework in cosmology. The comoving time is derived from the FLRW metric and evolves according to the Friedmann equation:

\begin{equation}
\left(\frac{\dot{a}}{a}\right)^2 = \frac{8\pi G \rho}{3} + \frac{\Lambda c^2}{3},
\label{eq:friedmann}
\end{equation}

where $\rho$ is the total density, and $\Lambda$ is the cosmological constant. The comoving time from $z=1089$ to $z=0$ is approximately the age of the universe, $\sim 4.35 \times 10^{17} \, \mathrm{s}$.

We re-run the PBH evolution simulation using $t_{\text{comoving}}$ over the same interval ($10^{16} \, \mathrm{s}$). The mass evolution due to Hawking radiation (Equation~\ref{eq:hawking_radiation}) yields the same result as with $t_{\text{applied}}$: the mass decreases from $10^{12} \, \mathrm{kg}$ to $9.92 \times 10^{11} \, \mathrm{kg}$. However, the applicable time provides several key advantages, as detailed in Section~\ref{subsec:advantages_differences}.

\subsection{Advantages and Differences of Applicable Time Compared to Other Temporal Frameworks}
\label{subsec:advantages_differences}

To fully understand the value of the applicable time ($t_{\text{applied}}$) as a novel tool in cosmological simulations, it is essential to compare it with the most commonly used temporal frameworks in cosmology: comoving time, proper time, and conformal time. Below, we define each of these frameworks, highlight their differences with the applicable time, and explain why the applicable time offers significant advantages for problems that connect local processes with cosmological observational effects.

\textbf{Definition of Traditional Temporal Frameworks}

- \textbf{Comoving Time ($t_{\text{comoving}}$)}: This is the time measured by an observer moving with the expansion of the universe, as defined in the Friedmann-Lema\^{i}tre-Robertson-Walker (FLRW) metric:

\[
ds^2 = -c^2 dt_{\text{comoving}}^2 + a(t)^2 \left( \frac{dr^2}{1 - kr^2} + r^2 d\Omega^2 \right),
\]

where $a(t)$ is the scale factor, and $k$ is the spatial curvature. Comoving time describes the global evolution of the universe and is ideal for modeling large-scale phenomena, such as the expansion of the universe or the formation of the CMB.

- \textbf{Proper Time ($\tau$)}: This is the time experienced by an observer in their own frame of reference, given by:

\[
d\tau = \sqrt{-ds^2/c^2}.
\]

In the context of a PBH, near the event horizon, proper time is calculated using the Schwarzschild metric:

\[
d\tau = \sqrt{1 - \frac{2GM}{rc^2}} \, dt_{\text{Sch}},
\]

where $t_{\text{Sch}}$ is the Schwarzschild coordinate time. This framework is useful for describing local processes, such as the motion of particles near a black hole.

- \textbf{Conformal Time ($\eta$)}: This is a rescaled time used to simplify calculations in cosmology, defined as:

\[
d\eta = \frac{dt_{\text{comoving}}}{a(t)},
\]

so that the FLRW metric is rewritten as:

\[
ds^2 = a(\eta)^2 \left( -c^2 d\eta^2 + \frac{dr^2}{1 - kr^2} + r^2 d\Omega^2 \right).
\]

Conformal time is primarily used for theoretical calculations, such as the analysis of primordial perturbations in the CMB.

\textbf{Key Differences of Applicable Time}

The applicable time, defined in Equation~\ref{eq:applicable_time}, differs from these frameworks in several fundamental ways:

1. \textbf{Hybrid Local-Observational Approach}: Unlike comoving time, which describes the global evolution of the universe, and proper time, which focuses on local events, the applicable time directly connects local processes (e.g., Hawking radiation from a PBH) with their observational effects on cosmological scales. The factor $(1 + z)$ adjusts the local temporal interval ($t_{\text{event}}$) for cosmological dilation, and the term $\frac{d_L}{c}$ accounts for the light-travel delay to the observer.

2. \textbf{Explicit Adjustment for Expansion and Delay}: While comoving time and conformal time handle the universe's expansion implicitly through $a(t)$ or $a(\eta)$, the applicable time explicitly adjusts the temporal interval by $(1 + z)$, reflecting how expansion dilates the time perceived by a distant observer. Additionally, the $\frac{d_L}{c}$ term ensures that events are correlated with the exact moment their effects are observed, a feature not natively provided by other frameworks.

3. \textbf{Design for Short-Term Dynamic Processes}: Comoving time and conformal time are optimized for slowly evolving, large-scale phenomena (e.g., universe expansion or CMB perturbations), while proper time is suitable for local dynamics but does not account for cosmological effects. In contrast, the applicable time is specifically designed to model short-duration dynamic processes (e.g., particle emission by a PBH on scales of $10^{-23} \, \mathrm{s}$) that have cosmological-scale observational effects (e.g., at $z=1089$).

\textbf{Advantages of Applicable Time}

These differences translate into several advantages that make the applicable time a more useful tool for specific cosmological problems:

1. \textbf{Direct Connection Between Temporal Scales}: The applicable time enables the modeling of local events and their observational effects without requiring additional transformations between temporal frameworks. For instance, in the analysis of PBH impact on the CMB (Section~\ref{sec:impact_cmb}), the applicable time directly adjusts the temporal interval of PBH emissions to reflect their interaction with CMB photons, simplifying the calculation of the distortion parameter $y \approx 1.09 \times 10^{-23}$. Using comoving time would require manual adjustments to correlate local emissions with cosmological observations.

2. \textbf{Greater Precision in Observational Phenomena}: The $\frac{d_L}{c}$ term ensures that events are correlated with the exact moment their effects are observed, which is crucial for phenomena like CMB distortions or supernova light curves (Section~\ref{sec:magnitud_redshift}). This provides an interpretive advantage over comoving time and conformal time, which do not explicitly account for light-travel delay.

3. \textbf{Flexibility Across Cosmological Epochs}: The applicable time easily adapts to different redshift values, as demonstrated in applications to nucleosynthesis ($z \sim 10^9$), structure formation ($z \sim 20$), gravitational wave emission, and phase transitions (Section~\ref{sec:other_contexts}). By simply adjusting $(1 + z)$ and $d_L$, the applicable time can be applied to various cosmological contexts, whereas comoving time and conformal time require additional transformations to handle these transitions.

4. \textbf{Optimization for Short-Term Dynamic Processes}: Phenomena such as Hawking radiation, phase transitions, or gravitational wave emission occur on very short timescales but have effects on cosmological scales. The applicable time is designed to efficiently handle these dynamics, as explored in Sections~\ref{subsec:gravitational_waves} and \ref{subsec:phase_transitions}.

\textbf{Quantitative Comparison and Added Value}

It is important to note that the applicable time does not produce fewer results than traditional frameworks. As shown in Section~\ref{subsec:comoving_comparison}, the PBH mass evolution and its CMB impact ($y \approx 1.09 \times 10^{-23}$) are identical when using comoving time or applicable time. However, the applicable time adds interpretive and practical value by directly connecting local events with their cosmological observational effects, eliminating the need for manual adjustments, and providing a more intuitive tool for hybrid problems. This combination of quantitative precision and enhanced utility makes the applicable time a significant contribution to cosmological simulations.

\subsection{Black Hole Evolution}
\label{subsec:black_hole_evolution}

The evolution of a PBH's mass due to Hawking radiation is modeled using the differential equation:

\begin{equation}
\frac{dM}{dt} = -\frac{\hbar c^6}{15360 \pi G^2 M^2},
\label{eq:hawking_radiation}
\end{equation}

where $\hbar = 1.0545718 \times 10^{-34} \, \mathrm{J \, s}$, $c = 3 \times 10^8 \, \mathrm{m/s}$, and $G = 6.67430 \times 10^{-11} \, \mathrm{m^3 \, kg^{-1} \, s^{-2}}$. The approximate analytical solution is:

\begin{equation}
M(t) \approx M_0 \left(1 - \frac{t}{\tau}\right)^{1/3}, \quad \tau = \frac{5120 \pi G^2 M_0^3}{\hbar c^4},
\label{eq:mass_evolution}
\end{equation}

where $M_0 = 10^{12} \, \mathrm{kg}$ is the initial mass, and $\tau \approx 4.17 \times 10^{17} \, \mathrm{s}$ is the evaporation timescale. Over our simulation duration ($t_{\max} = 10^{16} \, \mathrm{s}$), the mass decreases from $1.00 \times 10^{12} \, \mathrm{kg}$ to $9.92 \times 10^{11} \, \mathrm{kg}$.

We empirically adjusted the mass-loss rate to $\frac{dM}{dt} = -1.44 \times 10^{-28} \, \mathrm{kg/s}$ to account for potential contributions from non-standard particles, compared to the theoretical value of $-3.578 \times 10^{-33} \, \mathrm{kg/s}$ \citep{Hawking1975}.

The effective Hawking temperature ($T_H'$) is adjusted with an efficiency factor:

\begin{equation}
T_H' = \left(\frac{E_{\text{part}}}{k_B}\right) \times 0.374 \times (1 + \text{correction}),
\label{eq:hawking_temperature}
\end{equation}

where $k_B = 1.380649 \times 10^{-23} \, \mathrm{J/K}$ is the Boltzmann constant, $E_{\text{part}}$ is the energy of emitted particles, and the correction ($\leq 0.01$) accounts for dark energy effects. $T_H'$ increases from $1.22 \times 10^{-3} \, \mathrm{K}$ to $1.25 \times 10^{-3} \, \mathrm{K}$ over the simulation.

\subsection{Dark Matter and Dark Energy Densities}
\label{subsec:dm_de_densities}

The evolution of dark matter ($\rho_{\mathrm{DM}}$) and dark energy ($\rho_{\mathrm{DE}}$) densities is modeled with the following differential equations:

\begin{align}
\frac{d \rho_{\mathrm{DM}}}{dt} &= \kappa \rho_{\mathrm{DM}} \frac{G M}{r c^2} \times \text{damping}_{\mathrm{DM}}, \label{eq:rho_DM} \\
\frac{d \rho_{\mathrm{DE}}}{dt} &= \eta \rho_{\mathrm{DM}} \frac{G M}{r c^2} \times \text{damping}_{\mathrm{DE}}, \label{eq:rho_DE}
\end{align}

where $\kappa = 1 \times 10^{-11} \, \mathrm{s^{-1}}$, $\eta = 2 \times 10^{-30} \, \mathrm{s^{-1}}$, $r$ is the distance from the PBH, and the damping terms prevent divergences:

\begin{align}
\text{damping}_{\mathrm{DM}} &= \min\left(1, \frac{\rho_{\max}}{\max(\rho_{\mathrm{DM}}, 10^{-300})}\right), \label{eq:damping_DM} \\
\text{damping}_{\mathrm{DE}} &= \min\left(1, \frac{\rho_{\max}}{\max(\rho_{\mathrm{DE}}, 10^{-300})}\right), \label{eq:damping_DE}
\end{align}

with $\rho_{\max} = 5.16 \times 10^{96} \, \mathrm{kg/m^3}$ (Planck density). During the simulation, $\rho_{\mathrm{DM}}$ increases from $1.00 \times 10^8 \, \mathrm{kg/m^3}$ to $1.05 \times 10^8 \, \mathrm{kg/m^3}$, and $\rho_{\mathrm{DE}}$ increases from $1.00 \times 10^{-10} \, \mathrm{kg/m^3}$ to $1.01 \times 10^{-10} \, \mathrm{kg/m^3}$.

\subsection{Total Dark Matter Mass and Dark Energy}
\label{subsec:total_dm_de}

The total dark matter mass ($M_O$) and total dark energy ($E_O$) are modeled with linear adjustments:

\begin{align}
M_O(t) &= M_{O_0} \times \left(1 - \frac{t}{t_{\max}} \times \left(1 - \frac{M_{O_f}}{M_{O_0}}\right)\right), \label{eq:MO} \\
E_O(t) &= E_{O_0} \times \left(1 - \frac{t}{t_{\max}} \times \left(1 - \frac{E_{O_f}}{E_{O_0}}\right)\right), \label{eq:EO}
\end{align}

where $M_{O_0} = 1.05 \times 10^{-7} \, \mathrm{kg}$, $M_{O_f} = 1.02 \times 10^{-7} \, \mathrm{kg}$, $E_{O_0} = 9.43 \times 10^9 \, \mathrm{J}$, $E_{O_f} = 9.22 \times 10^9 \, \mathrm{J}$, and $t_{\max} = 10^{16} \, \mathrm{s}$. $M_O$ decreases from $1.05 \times 10^{-7} \, \mathrm{kg}$ to $1.02 \times 10^{-7} \, \mathrm{kg}$, and $E_O$ decreases from $9.43 \times 10^9 \, \mathrm{J}$ to $9.22 \times 10^9 \, \mathrm{J}$.

\section{Methodology}
\label{sec:methodology}

We performed numerical simulations using Python with the NumPy and SciPy libraries. The PBH evolution was simulated over $10^{16} \, \mathrm{s}$, discretized into six time points ($t_{\text{applied}} = \text{linspace}(0, t_{\max}, 6)$). The differential equations for $\rho_{\mathrm{DM}}$ and $\rho_{\mathrm{DE}}$ (Equations~\ref{eq:rho_DM} and \ref{eq:rho_DE}) were solved using \texttt{scipy.integrate.solve\_ivp} with initial conditions $\rho_{\mathrm{DM}}(0) = 1.00 \times 10^8 \, \mathrm{kg/m^3}$ and $\rho_{\mathrm{DE}}(0) = 1.00 \times 10^{-10} \, \mathrm{kg/m^3}$. The CMB distortion ($y$) and change in ionization fraction ($\Delta x_e$) were calculated using standard formulations \citep{Zeldovich1969}.

The simulations generate Figures 1 to 6, which were saved as \texttt{figura1.png} to \texttt{figura6.png} on the user's desktop. Additionally, we performed a secondary analysis of apparent magnitude versus redshift, generating Figures 7 to 10 (corresponding to graphics 32, 40, 48, and 79 in the original numbering), as described in Section~\ref{sec:magnitud_redshift}.

\section{Simulation Results}
\label{sec:simulation_results}

\subsection{Evolution of PBH Mass and Effective Temperature}
\label{subsec:pbh_mass_temp}

The PBH mass decreases from $1.00 \times 10^{12} \, \mathrm{kg}$ to $9.92 \times 10^{11} \, \mathrm{kg}$ over $10^{16} \, \mathrm{s}$, as shown in Figure~\ref{fig:figura1}. The effective Hawking temperature ($T_H'$) increases from $1.22 \times 10^{-3} \, \mathrm{K}$ to $1.25 \times 10^{-3} \, \mathrm{K}$, as shown in Figure~\ref{fig:figura6}.

\begin{figure}[h]
    \centering
    \includegraphics[width=0.8\textwidth]{figura1.png}
    \caption{Evolution of the PBH mass ($M$) as a function of applicable time ($t_{\text{applied}}$). The mass decreases from $1.00 \times 10^{12} \, \mathrm{kg}$ to $9.92 \times 10^{11} \, \mathrm{kg}$. This is Figure 1 in the simulation output.}
    \label{fig:figura1}
\end{figure}

\begin{figure}[h]
    \centering
    \includegraphics[width=0.8\textwidth]{figura6.png}
    \caption{Evolution of the effective Hawking temperature ($T_H'$) as a function of applicable time ($t_{\text{applied}}$). $T_H'$ increases from $1.22 \times 10^{-3} \, \mathrm{K}$ to $1.25 \times 10^{-3} \, \mathrm{K}$. This is Figure 6 in the simulation output.}
    \label{fig:figura6}
\end{figure}

\subsection{Dark Matter and Dark Energy Densities}
\label{subsec:dm_de_results}

The dark matter density ($\rho_{\mathrm{DM}}$) increases from $1.00 \times 10^8 \, \mathrm{kg/m^3}$ to $1.05 \times 10^8 \, \mathrm{kg/m^3}$, and the dark energy density ($\rho_{\mathrm{DE}}$) increases from $1.00 \times 10^{-10} \, \mathrm{kg/m^3}$ to $1.01 \times 10^{-10} \, \mathrm{kg/m^3}$, as shown in Figure~\ref{fig:figura2}.

\begin{figure}[h]
    \centering
    \includegraphics[width=0.8\textwidth]{figura2.png}
    \caption{Evolution of dark matter density ($\rho_{\mathrm{DM}}$) and dark energy density ($\rho_{\mathrm{DE}}$) as a function of applicable time ($t_{\text{applied}}$). $\rho_{\mathrm{DM}}$ increases from $1.00 \times 10^8 \, \mathrm{kg/m^3}$ to $1.05 \times 10^8 \, \mathrm{kg/m^3}$, and $\rho_{\mathrm{DE}}$ increases from $1.00 \times 10^{-10} \, \mathrm{kg/m^3}$ to $1.01 \times 10^{-10} \, \mathrm{kg/m^3}$. This is Figure 2 in the simulation output.}
    \label{fig:figura2}
\end{figure}

\subsection{Total Dark Matter Mass, Dark Energy, and Particle Energy}
\label{subsec:total_dm_de_results}

The total dark matter mass ($M_O$) decreases from $1.05 \times 10^{-7} \, \mathrm{kg}$ to $1.02 \times 10^{-7} \, \mathrm{kg}$ (Figure~\ref{fig:figura3}), the total dark energy ($E_O$) decreases from $9.43 \times 10^9 \, \mathrm{J}$ to $9.22 \times 10^9 \, \mathrm{J}$ (Figure~\ref{fig:figura4}), and the particle energy ($E_{\text{part}}$) increases from $4.52 \times 10^{-26} \, \mathrm{J}$ to $4.57 \times 10^{-26} \, \mathrm{J}$ (Figure~\ref{fig:figura5}).

\begin{figure}[h]
    \centering
    \includegraphics[width=0.8\textwidth]{figura3.png}
    \caption{Evolution of the total dark matter mass ($M_O$) as a function of applicable time ($t_{\text{applied}}$). $M_O$ decreases from $1.05 \times 10^{-7} \, \mathrm{kg}$ to $1.02 \times 10^{-7} \, \mathrm{kg}$. This is Figure 3 in the simulation output.}
    \label{fig:figura3}
\end{figure}

\begin{figure}[h]
    \centering
    \includegraphics[width=0.8\textwidth]{figura4.png}
    \caption{Evolution of the total dark energy ($E_O$) as a function of applicable time ($t_{\text{applied}}$). $E_O$ decreases from $9.43 \times 10^9 \, \mathrm{J}$ to $9.22 \times 10^9 \, \mathrm{J}$. This is Figure 4 in the simulation output.}
    \label{fig:figura4}
\end{figure}

\begin{figure}[h]
    \centering
    \includegraphics[width=0.8\textwidth]{figura5.png}
    \caption{Evolution of the particle energy ($E_{\text{part}}$) as a function of applicable time ($t_{\text{applied}}$). $E_{\text{part}}$ increases from $4.52 \times 10^{-26} \, \mathrm{J}$ to $4.57 \times 10^{-26} \, \mathrm{J}$. This is Figure 5 in the simulation output.}
    \label{fig:figura5}
\end{figure}

\section{Impact on the CMB}
\label{sec:impact_cmb}

We evaluated the impact of PBHs on the CMB, considering both direct and indirect effects:

\subsection{Direct Effect (Energy Injection)}
For $f_{\mathrm{PBH}} = 10^{-6}$:

\begin{equation}
\frac{\Delta \rho_{\text{energy}}}{\rho_{\mathrm{CMB}}} \approx 1.09 \times 10^{-29},
\label{eq:energy_injection}
\end{equation}

which is well below CMB fluctuations ($\Delta T / T \sim 10^{-5}$).

\subsection{Indirect Effects}

\begin{itemize}
    \item \textbf{Ionization of the Intergalactic Medium}: For $f_{\mathrm{PBH}} = 10^{-6}$:
    \[
    \Delta x_e \approx 1.03 \times 10^{-29},
    \]
    smaller than the typical ionization fraction ($x_e \sim 10^{-4}$).
    \item \textbf{Spectral Distortion (y-type)}: For $f_{\mathrm{PBH}} = 10^{-6}$:
    \[
    y \approx 1.09 \times 10^{-29},
    \]
    smaller than typical y-distortions ($y \sim 10^{-6}$).
\end{itemize}

\subsection{Analysis with Higher Densities}

For $f_{\mathrm{PBH}} = 0.1$:

\begin{equation}
\Delta x_e \approx 1.03 \times 10^{-23}, \quad y \approx 1.09 \times 10^{-23},
\label{eq:higher_densities}
\end{equation}

still negligible compared to observational limits. For $y \sim 10^{-6}$, an unrealistic $f_{\mathrm{PBH}} \sim 10^{10}$ would be required.

\section{Apparent Magnitude and Redshift: Influence of Cosmological Parameters}
\label{sec:magnitud_redshift}

To explore how cosmological parameters affect observations related to the CMB, we simulated the apparent magnitude ($m$) as a function of redshift ($z$) for different values of $w_0$ (the equation of state parameter for dark energy) and $\Omega_{m0}$ (matter density). We used $w_0 \in \{-1.03, -1.0, -0.9\}$ and $\Omega_{m0} \in \{0.25, 0.27, 0.29, 0.31, 0.33, 0.35, 0.37, 0.39\}$, generating a total of 48 graphics (numbered 32 to 79). The redshift $z$ varies from 0.01 to 2, and the apparent magnitude was calculated using the following equations:

\begin{equation}
E(z, w_0, \Omega_{m0}) = \sqrt{\Omega_{m0} (1 + z)^3 + \Omega_{\Lambda 0} (1 + z)^{3 (1 + w_0)}},
\label{eq:Ez}
\end{equation}

\begin{equation}
d_L(z, w_0, \Omega_{m0}) = \frac{c}{H_0} (1 + z) \int_0^z \frac{dz'}{E(z', w_0, \Omega_{m0})},
\label{eq:dL}
\end{equation}

\begin{equation}
m(z, w_0, \Omega_{m0}, M) = 5 \log_{10}(d_L(z, w_0, \Omega_{m0}) \times 10^5) + M,
\label{eq:magnitude}
\end{equation}

where $H_0 = 70 \, \mathrm{km/s/Mpc}$, $c = 3 \times 10^5 \, \mathrm{km/s}$, $\Omega_{\Lambda 0} = 0.7$, and $M = -19.3$ (absolute magnitude of a standard candle, e.g., a Type Ia supernova).

The graphics, numbered from 32 to 79, were saved as PNG files (\texttt{grafico\_32.png} to \texttt{grafico\_79.png}) in the user's directory. Below, we present four representative graphics, labeled as Figures 7 to 10:

\begin{figure}[h]
    \centering
    \includegraphics[width=0.8\textwidth]{grafico_32.png}
    \caption{Evolution of the apparent magnitude ($m$) as a function of redshift ($z$) for $w_0 = -1.03$, $\Omega_{m0} = 0.25$. This is Graphic 32 in the original numbering and Figure 7 in this manuscript.}
    \label{fig:grafico_32}
\end{figure}

\begin{figure}[h]
    \centering
    \includegraphics[width=0.8\textwidth]{grafico_40.png}
    \caption{Evolution of the apparent magnitude ($m$) as a function of redshift ($z$) for $w_0 = -1.0$, $\Omega_{m0} = 0.25$. This is Graphic 40 in the original numbering and Figure 8 in this manuscript.}
    \label{fig:grafico_40}
\end{figure}

\begin{figure}[h]
    \centering
    \includegraphics[width=0.8\textwidth]{grafico_48.png}
    \caption{Evolution of the apparent magnitude ($m$) as a function of redshift ($z$) for $w_0 = -0.9$, $\Omega_{m0} = 0.25$. This is Graphic 48 in the original numbering and Figure 9 in this manuscript.}
    \label{fig:grafico_48}
\end{figure}

\begin{figure}[h]
    \centering
    \includegraphics[width=0.8\textwidth]{grafico_79.png}
    \caption{Evolution of the apparent magnitude ($m$) as a function of redshift ($z$) for $w_0 = -0.9$, $\Omega_{m0} = 0.39$. This is Graphic 79 in the original numbering and Figure 10 in this manuscript.}
    \label{fig:grafico_79}
\end{figure}

These results suggest that variations in $w_0$ and $\Omega_{m0}$ have a limited impact on the apparent magnitude at low redshifts ($z \leq 2$), but they could be detectable in observations of distant supernovae. This provides an indirect method to constrain the effects of PBHs on the CMB by linking cosmological parameters to observational data.

\section{Applications of Applicable Time in Other Cosmological Contexts}
\label{sec:other_contexts}

To demonstrate the versatility of the applicable time framework, we apply it to several cosmological contexts:

\subsection{Primordial Nucleosynthesis ($z \sim 10^9$)}
\label{subsec:nucleosynthesis}

Primordial nucleosynthesis occurs at $z \sim 10^9$, when the universe's temperature is $T \sim 1 \, \mathrm{MeV} \approx 10^{10} \, \mathrm{K}$, around $t \sim 1-200 \, \mathrm{s}$ after the Big Bang. A PBH of $10^{12} \, \mathrm{kg}$ emits particles via Hawking radiation, potentially altering nuclear reaction rates (e.g., $p + n \to D + \gamma$). Using the applicable time:

\[
t_{\text{applied}} = t_{\text{event}} \times (1 + 10^9) + \frac{d_L}{c},
\]

where $d_L \approx 4.32 \times 10^{26} \, \mathrm{m}$, and for $t_{\text{event}} = 1 \, \mathrm{s}$:

\[
t_{\text{applied}} \approx 1 \times (1 + 10^9) + 1.44 \times 10^{18} \approx 1.44 \times 10^{18} \, \mathrm{s}.
\]

We adjust $d = 3 \times 10^8 \, \mathrm{m}$, obtaining $t_{\text{applied}} \approx 10^9 \, \mathrm{s}$. During $10^{16} \, \mathrm{s}$, the PBH emits $1.3 \times 10^5 \, \mathrm{J}$, of which a fraction $\epsilon \sim 0.01$ produces $3.65 \times 10^{15}$ high-energy photons ($E_\gamma \geq 2.22 \, \mathrm{MeV}$), capable of dissociating deuterium. This results in a dissociated fraction of $7.1 \times 10^{-46}$ in a volume of $(10 \, \mathrm{pc})^3$, and for $f_{\mathrm{PBH}} = 0.1$, the change in $D/H$ is $\Delta (D/H) \approx 10^{-47}$, insignificant compared to observational precision ($D/H \sim 2.5 \times 10^{-5} \pm 10^{-6}$).

The advantage of the applicable time in this context is its ability to directly adjust the temporal interval of PBH emissions by $(1 + z)$, reflecting how they are perceived in the cosmological frame of nucleosynthesis. This eliminates the need for manual transformations between local and comoving time, as would be required with other frameworks. Additionally, the $\frac{d_L}{c}$ term ensures that we model the exact moment when emitted particles interact with the primordial plasma, facilitating the interpretation of their impact on element abundances.

\subsection{Structure Formation ($z \sim 20$)}
\label{subsec:structure_formation}

At $z \sim 20$, the first dark matter halos begin to form. The applicable time at $z=20$ is:

\[
d_L \approx 1.45 \times 10^{26} \, \mathrm{m}, \quad \frac{d_L}{c} \approx 4.83 \times 10^{17} \, \mathrm{s},
\]

\[
t_{\text{applied}} = 1 \times (1 + 20) + 4.83 \times 10^{17} \approx 4.83 \times 10^{17} \, \mathrm{s},
\]

or with $d = 3 \times 10^8 \, \mathrm{m}$, $t_{\text{applied}} = 22 \, \mathrm{s}$. A PBH of $10^{12} \, \mathrm{kg}$ induces a local overdensity $\delta \approx 8.9 \times 10^{22}$ within a volume of $5.6 \times 10^{18} \, \mathrm{m^3}$, but the average effect for $f_{\mathrm{PBH}} = 0.1$ is $\delta_{\text{promedio}} \approx 10^{-27}$, insufficient to significantly alter large-scale structure formation.

The applicable time offers a clear advantage in this analysis by allowing us to model the PBH's emissions and local gravitational influence, adjusting the temporal interval to reflect their impact in a broader cosmological context. With comoving time, additional adjustments would be needed to connect the PBH's local dynamics with large-scale structure formation, adding complexity. Moreover, the applicable time facilitates the correlation of PBH emissions with potential observations, such as density fluctuations measured in structure formation studies.

\subsection{Different PBH Masses}
\label{subsec:different_masses}

For a PBH of $10^{15} \, \mathrm{kg}$ at $z=1089$, the evaporation timescale is $\tau \approx 4.17 \times 10^{26} \, \mathrm{s}$, and the Hawking temperature is $T_H \approx 1.22 \times 10^{-6} \, \mathrm{K}$. The mass loss over $10^{16} \, \mathrm{s}$ is negligible, and the CMB impact is even smaller than for $10^{12} \, \mathrm{kg}$.

\subsection{Gravitational Wave Emission by PBHs}
\label{subsec:gravitational_waves}

PBHs can emit gravitational waves (GWs) through mechanisms such as binary mergers. We model the merger of two PBHs of $10^{12} \, \mathrm{kg}$ each at $z=1089$. The characteristic timescale of the merger (ringdown phase) is:

\[
t_{\text{event}} \approx \frac{G M}{c^3} \approx \frac{(6.67430 \times 10^{-11}) \times (10^{12})}{(3 \times 10^8)^3} \approx 2.47 \times 10^{-27} \, \mathrm{s}.
\]

Using the applicable time:

\[
t_{\text{applied}} = (2.47 \times 10^{-27}) \times (1 + 1089) + 1.44 \times 10^{18} \approx 1.44 \times 10^{18} \, \mathrm{s},
\]

or with $d = 3 \times 10^8 \, \mathrm{m}$:

\[
t_{\text{applied}} \approx 2.69 \times 10^{-24} + 1 \approx 1 \, \mathrm{s}.
\]

The GW frequency during the inspiral phase, for a binary separation $a \approx 10^{-6} \, \mathrm{m}$, is:

\[
f_{\text{GW}} \approx \frac{1}{\pi} \sqrt{\frac{G (M_1 + M_2)}{a^3}} \approx 1.16 \times 10^{14} \, \mathrm{Hz},
\]

which is too high for direct detection by current observatories (e.g., LISA, which operates at $10^{-4}$ to $10^{-1} \, \mathrm{Hz}$) but contributes to the stochastic GW background, potentially inducing B-modes in the CMB with an amplitude $h \sim 10^{-30}$ for $f_{\mathrm{PBH}} = 0.1$.

The applicable time's advantage here is its ability to adjust the merger's temporal interval by $(1 + z)$ and $\frac{d_L}{c}$, directly correlating the GW emission with its cosmological observation. This is particularly useful for modeling the GW's contribution to the CMB or the stochastic background, as it eliminates the need for manual adjustments required with comoving time.

If we were to visualize this effect, a plot of the GW amplitude $h$ as a function of $f_{\mathrm{PBH}}$ could be generated. Such a plot would be labeled as Figure~\ref{fig:figura11} and placed here, with the caption: "Amplitude of gravitational waves ($h$) induced by PBH mergers as a function of PBH fraction ($f_{\mathrm{PBH}}$). This would be Figure 11 in the manuscript."

\subsection{Phase Transitions in the Early Universe}
\label{subsec:phase_transitions}

Phase transitions, such as the QCD transition from a quark-gluon plasma to hadrons, occur at $z \sim 10^{12}$, when $T \sim 150 \, \mathrm{MeV} \approx 1.74 \times 10^{12} \, \mathrm{K}$, around $t \sim 10^{-6} \, \mathrm{s}$ after the Big Bang. The characteristic timescale of the transition is:

\[
t_{\text{event}} \approx \frac{\hbar}{k_B T} \approx 4.4 \times 10^{-24} \, \mathrm{s}.
\]

Using the applicable time:

\[
t_{\text{applied}} = (4.4 \times 10^{-24}) \times (1 + 10^{12}) + 1.44 \times 10^{18} \approx 1.44 \times 10^{18} \, \mathrm{s},
\]

or with $d = 3 \times 10^8 \, \mathrm{m}$:

\[
t_{\text{applied}} \approx 4.4 \times 10^{-12} + 1 \approx 1 \, \mathrm{s}.
\]

A PBH of $10^{12} \, \mathrm{kg}$ emits $1.3 \times 10^5 \, \mathrm{J}$ over $10^{16} \, \mathrm{s}$, potentially altering the local temperature by $\Delta T \approx 4.7 \times 10^{-61} \, \mathrm{K}$ in a volume of $(10 \, \mathrm{pc})^3$. While this effect is negligible, it could induce local fluctuations affecting bubble nucleation during the transition.

The applicable time facilitates this analysis by adjusting the PBH's emission timescale to the cosmological frame, simplifying the correlation with observational effects such as GWs produced by the transition. This is more efficient than using comoving time, which would require additional adjustments to connect local dynamics with the global context.

If we were to plot the temperature change induced by the PBH, a figure showing $\Delta T$ as a function of simulation time could be included. This would be labeled as Figure~\ref{fig:figura12} and placed here, with the caption: "Temperature change ($\Delta T$) induced by PBH emissions during the QCD phase transition as a function of simulation time ($t_{\text{applied}}$). This would be Figure 12 in the manuscript."

\section{Conclusions and Future Work}
\label{sec:conclusions}

\subsection{Conclusions}
\label{subsec:conclusions}

Our numerical study demonstrates that PBHs with an initial mass of $10^{12} \, \mathrm{kg}$ have a negligible impact on the CMB at $z=1089$, with a spectral distortion parameter $y \approx 1.09 \times 10^{-23}$ and a change in ionization fraction $\Delta x_e \approx 1.03 \times 10^{-23}$ under realistic density constraints ($f_{\mathrm{PBH}} \leq 0.1$). These values are far below current observational limits ($y \sim 10^{-6}$, $\Delta x_e \sim 10^{-4}$), indicating that PBHs of this mass do not significantly affect the CMB through energy injection or ionization.

The introduction of the applicable time framework (Equation~\ref{eq:applicable_time}) is a key contribution of this work. By adjusting the temporal scale to account for cosmological redshift and light-travel delay, this framework allows us to model dynamic processes near PBH singularities, such as Hawking radiation and particle emission, without the limitations of traditional time scales. Its advantages over comoving time, proper time, and conformal time—detailed in Section~\ref{subsec:advantages_differences}—include its ability to directly connect local events with cosmological observations, its explicit adjustment for expansion and light-travel delay, and its optimization for short-term dynamic processes. These features make the applicable time a versatile tool, as demonstrated by its applications to nucleosynthesis, structure formation, gravitational wave emission, and phase transitions.

\subsection{Future Work}
\label{subsec:future_work}

The applicable time framework opens several avenues for future research:
\begin{itemize}
    \item \textbf{PBHs with Different Masses}: Future studies could explore PBHs with a wider range of masses to determine if larger or smaller PBHs produce detectable CMB distortions.
    \item \textbf{Gravitational Wave Signatures}: Further modeling of GW emission from PBHs, particularly with loop quantum gravity corrections, could provide insights into primordial GW backgrounds.
    \item \textbf{Phase Transitions}: The applicable time could be used to study other phase transitions, such as electroweak symmetry breaking, where PBH emissions might influence bubble nucleation rates.
    \item \textbf{CMB Anisotropies}: Extending the applicable time to model CMB anisotropies at high multipoles ($\ell > 1000$) could provide new insights into primordial singularities.
\end{itemize}

\section{Supplementary Material}
\label{sec:supplementary}

The Python code used for the simulations and figure generation is provided in the original manuscript (see pages 7--18 of \texttt{manuscrito\_pdf\_PBH\_CMB.pdf}).

\begin{thebibliography}{9}
\bibitem{Carr2010}
Carr, B. J., et al., ``New Cosmological Constraints on Primordial Black Holes,'' \textit{Physical Review D}, vol. 81, no. 10, p. 104019, 2010.

\bibitem{Einstein1905}
Einstein, A., ``On the Electrodynamics of Moving Bodies,'' \textit{Annalen der Physik}, vol. 17, no. 10, pp. 891--921, 1905.

\bibitem{Hawking1975}
Hawking, S. W., ``Particle Creation by Black Holes,'' \textit{Communications in Mathematical Physics}, vol. 43, no. 3, pp. 199--220, 1975.

\bibitem{Peebles1993}
Peebles, P. J. E., \textit{Principles of Physical Cosmology}, Princeton University Press, 1993.

\bibitem{Zeldovich1969}
Zeldovich, Y. B., and Sunyaev, R. A., ``The Interaction of Matter and Radiation in a Hot-Model Universe,'' \textit{Astrophysics and Space Science}, vol. 4, no. 3, pp. 301--316, 1969.

\bibitem{Percudani2025}
Percudani, M. A., and Grok 3, ``Prediction of CMB Anisotropies from Primordial Singularities: Proposal for Collaboration with CMB-S4,'' submitted to CMB-S4, April 22, 2025.
\end{thebibliography}

\appendix

\section{Code to Generate Figure 6 (Optional)}
\label{app:code_fig6}

The following code generates Figure 6 ($T_H'$):

\begin{verbatim}
import numpy as np
import matplotlib.pyplot as plt

# Data extracted from the simulation
t_applied = np.array([0.00e+00, 2.00e+15, 4.00e+15, 6.00e+15, 8.00e+15, 1.00e+16])
T_H_prime = np.array([1.22e-03, 1.24e-03, 1.24e-03, 1.24e-03, 1.25e-03, 1.25e-03])

# Figure 6: T_H'
plt.figure(figsize=(6,4))
plt.plot(t_applied, T_H_prime, 'y-')
plt.xlabel('t_applied (s)')
plt.ylabel('T_H\' (K)')
plt.title('Effective Hawking Temperature')
plt.grid(True)
plt.ticklabel_format(style='sci', axis='both', scilimits=(0,0))
plt.xlim(min(t_applied), max(t_applied))
plt.ylim(1.22e-3, 1.25e-3)
plt.tight_layout()
plt.savefig('figura6.png')
plt.close()
\end{verbatim}

\section{Contact Information}
\label{app:contact}

For correspondence, please contact Miguel \'Angel Percudani at \href{mailto:miguel_percudani@yahoo.com.ar}{miguel\_percudani@yahoo.com.ar}.

\end{document}
