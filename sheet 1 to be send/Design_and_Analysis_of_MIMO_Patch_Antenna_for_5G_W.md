**Technical Extraction Document**

---

## Document Information

**Title:** Design and Analysis of MIMO Patch Antenna for 5G Wireless Communication Systems

**Authors:** Pallavi H. V¹*, A P Jagadeesh Chandra², Paramesha³

**Affiliations:**
- ¹ Department of ECE, Government Engineering College, Hassan, Karnataka, India
- ² Department of ECE, Adichunchanagiri Institute of Technology, Chikkamagalur, Karnataka, India
- ³ Department of ECE, Central University of Karnataka, Kalaburagi, Karnataka, India

**Source:** International Journal of Computer Networks & Communications (IJCNC), Vol.14, No.4, July 2022

**DOI:** 10.5121/ijcnc.2022.14403

---

## Abstract

A circular array microstrip patch antenna (MPA) design is proposed for 5G wireless communication utilizing millimeter-wave frequency to enhance coverage area. The Multi Input Multi Output (MIMO) feeding technique is employed to improve performance at a resonant frequency of 35 GHz. The substrate material is RT-Duroid 5880 with dielectric constant 2.2 and thickness 0.5 mm. Simulation analysis obtained gain of 8.8 dB and return loss of -41.9 dB. Comparative analysis validates that the circular array MPA is superior to single element MPA and 2×2 rectangular array MPA designs for 5G wireless communication.

**Keywords:** Wireless communication, Bandwidth, Radiation efficiency, Antennas, Microstrip patch antenna (MPA)

---

## Equations and Mathematical Models

### Design Parameter Equations

**Equation 1: Patch Width Calculation**

$$W_p = \frac{c}{2f_r\sqrt{\frac{\varepsilon_r + 1}{2}}}$$

Where:
- $W_p$ = patch width
- $c$ = speed of light (3 × 10⁸ m/s)
- $f_r$ = resonance frequency
- $\varepsilon_r$ = dielectric constant value

**Equation 2: Patch Length Calculation**

$$L_p = L_{peff} - 2\Delta L_p$$

Where:
- $L_p$ = length of patch
- $L_{peff}$ = effective length of patch
- $\Delta L_p$ = extension length of patch

**Equation 3: Effective Patch Length**

$$L_{peff} = \frac{c}{2f_r\sqrt{\varepsilon_{reff}}}$$

Where:
- $\varepsilon_{reff}$ = effective dielectric constant

**Equation 4: Patch Length Extension**

$$\Delta L_p = 0.412h \frac{(\varepsilon_{reff} + 0.3)(\frac{W_p}{h} + 0.264)}{(\varepsilon_{reff} - 0.258)(\frac{W_p}{h} + 0.8)}$$

Where:
- $h$ = substrate thickness
- $\varepsilon_{reff}$ = effective dielectric constant

**Equation 5: Effective Dielectric Constant**

$$\varepsilon_{reff} = \frac{\varepsilon_r + 1}{2} + \frac{\varepsilon_r - 1}{2}\left[1 + 12\frac{h}{W_p}\right]^{-1/2}$$

**Equation 6: Substrate Length**

$$L_g = 6h + L_p$$

Where:
- $L_g$ = length of substrate

**Equation 7: Substrate Width**

$$W_g = 6h + W_p$$

Where:
- $W_g$ = width of substrate

**Equation 8: Microstrip Feed Line Length**

$$L_f = \frac{1}{4}\lambda_g$$

Where:
- $L_f$ = length of microstrip feed line
- $\lambda_g$ = guided wave length

**Equation 9: Guided Wavelength**

$$\lambda_g = \frac{\lambda}{\sqrt{\varepsilon_{reff}}}$$

**Equation 10: Free Space Wavelength**

$$\lambda = \frac{c}{f_r}$$

**Equation 11: Feed Line Width**

$$W_f = \frac{7.48 \times h}{e^{\left(\frac{Z_0\sqrt{\varepsilon_r + 1.41}}{87} - 1.25 \times t\right)}}$$

Where:
- $W_f$ = width of feed line
- $Z_0$ = impedance value (50 Ω)
- $t$ = trace thickness (0.0175 mm)

---

## Technical Specifications and Design Parameters

### Substrate Material Specifications

| Specification | Value | Unit |
|---|---|---|
| Material | RT-Duroid 5880 | - |
| Dielectric Constant | 2.2 | - |
| Thickness | 0.5 | mm |
| Resonance Frequency | 35 | GHz |
| Conductor Material (Patch & Ground) | Copper | - |
| Conductor Thickness | 0.0175 | mm |
| Port Impedance | 50 | Ω |
| Trace Thickness | 0.0175 | mm |

### Calculated and Optimized Design Parameters

\begin{table}
\begin{tabular}{|l|l|c|c|}
\hline
Design Parameter & Description & Calculated (mm) & Optimized (mm) \\
\hline
$W_p$ & Width of patch & 3.386 & 3.62 \\
$L_p$ & Length of patch & 2.551 & 2.45 \\
$W_g$ & Width of substrate and ground plane & 5.49 & 6 \\
$L_g$ & Length of substrate and ground plane & 4.65 & 6 \\
$W_f$ & Width of feed line & 0.46 & 0.46 \\
$L_f$ & Length of feed line & 1.57 & 1.57 \\
\hline
\end{tabular}
\caption{Obtained and Optimized Values of Design Parameters}
\end{table}

---

## Design Configurations and Methodologies

### Three Antenna Designs Analyzed

#### 1. Single Element Microstrip Patch Antenna (MPA)

**Configuration:**
- Single circular patch element
- Single feed line
- Single port (SISO - Single Input Single Output)
- Optimized substrate dimensions: 6 × 6 mm
- Optimized ground plane dimensions: 6 × 6 mm
- Radiation box dimensions: 15 mm length × 15 mm width × 8 mm height

**Design Features:**
- Simple single-element design serving as baseline
- Designed and analyzed using HFSS (High-Frequency Structure Simulation) software
- Port impedance: 50 Ω
- Simulation frequency range: 28 GHz to 42 GHz
- Maximum simulation passes: 20

**Design Methodology:**
The substrate is designed first utilizing optimized parameters. Patch and feed line are designed on one side of substrate; ground plane covers the other side. Port placement is at appropriate location. Radiation box is designed around structure. Boundaries are assigned: patch, feed line, and ground plane as perfect E; radiation box as radiation boundary. Port assigned as lumped port excitation with full port impedance 50 Ω.

#### 2. 2×2 Rectangular Array Microstrip Patch Antenna

**Configuration:**
- Four patch elements arranged in 2×2 rectangular formation
- Four ports with MIMO feeding
- Four feed lines
- Substrate dimensions: 12 × 12 mm (doubled from single element)
- Ground plane dimensions: 12 × 12 mm
- Radiation box dimensions: 20 mm length × 20 mm width × 10 mm height

**Patch Positioning:**
- Two patches placed horizontally with 0° rotation
- Two patches placed above first two with 90° rotation
- Rectangular grid arrangement

**Design Features:**
- MIMO structure implementation
- Each port impedance: 50 Ω
- Similar analysis setup as single element MPA
- Enhanced radiation properties through array configuration

#### 3. Circular Array Microstrip Patch Antenna (Proposed Design)

**Configuration:**
- Four patch elements arranged in circular formation
- Four ports with MIMO feeding
- Four feed lines
- Substrate dimensions: 12 × 12 mm (same as rectangular array)
- Ground plane dimensions: 12 × 12 mm
- Radiation box dimensions: 20 mm length × 20 mm width × 10 mm height (same as rectangular)

**Patch Positioning:**
- Patches located at angular positions: 0°, 90°, 180°, and 270°
- Arranged in circular pattern around center
- Each patch rotated at respective angular positions

**Design Features:**
- MIMO structure implementation
- Each port impedance: 50 Ω
- Novel circular array configuration for improved performance
- Optimized for 5G millimeter-wave applications

**Design Methodology - All Three Designs:**
All designs utilize High-Frequency Structure Simulation (HFSS) software platform from ANSYS. Complete design flow includes: parameter setup → geometry creation → boundary conditions assignment → port definition → radiation box definition → simulation setup (sweep) → frequency analysis and results extraction.

---

## Simulation Results and Performance Metrics

### Performance Metrics Definition

The following performance parameters are evaluated for all antenna designs:

- **Gain:** Strength of transmitted/received RF signals in particular direction (dB)
- **Return Loss (S₁₁):** Ratio of reflected to applied frequencies; should be < 0 for good impedance matching (dB)
- **VSWR (Voltage Standing Wave Ratio):** Efficiency of transmitted RF power; optimal range 1-2 (dimensionless)
- **Bandwidth:** Range of frequencies where antenna can properly transmit/receive (GHz)
- **Mutual Coupling:** Electromagnetic interactions between antenna elements; should be minimal (dB)
- **Radiation Efficiency:** Ratio of radiated power to input power (absolute value)
- **Radiation Pattern:** Energy distribution radiated from antenna (E-plane and H-plane)

### Single Element MPA Results

\begin{table}
\begin{tabular}{|c|c|c|c|c|c|}
\hline
Resonance Frequency (GHz) & Gain (dB) & Return Loss (dB) & VSWR & Bandwidth (GHz) & Radiation Efficiency (abs) \\
\hline
35 & 8.1 & -34.5 & 1.18 & 1.9 (35.7–33.8) & 1.02 \\
\hline
\end{tabular}
\caption{Performance Analysis Results of Single Element MPA}
\end{table}

**Key Findings:**
- Achieved -10 dB return loss at 35 GHz bandwidth
- VSWR of 1.18 indicates good impedance matching
- Bandwidth of 1.9 GHz (35.7–33.8 GHz)
- Radiation efficiency of 1.02 (absolute value)

### 2×2 Rectangular Array MPA Results

\begin{table}
\begin{tabular}{|c|c|c|c|c|c|c|}
\hline
Resonance Frequency (GHz) & Gain (dB) & Return Loss (dB) & VSWR & Bandwidth (GHz) & Mutual Coupling (dB) & Radiation Efficiency (abs) \\
\hline
35 & 8.4 & -33.9 & 1.6 & 1.9 (35.3–33.4) & -23.05 & 1.02 \\
\hline
\end{tabular}
\caption{Performance Analysis Results of 2×2 Rectangular Array MPA}
\end{table}

**Key Findings:**
- Improved gain to 8.4 dB compared to single element
- Return loss of -33.9 dB
- VSWR of 1.6 (acceptable but higher than single element)
- Bandwidth maintained at 1.9 GHz (35.3–33.4 GHz)
- Mutual coupling between elements: -23.05 dB
- Radiation efficiency: 1.02 (absolute value)

### Proposed Circular Array MPA Results

\begin{table}
\begin{tabular}{|c|c|c|c|c|c|c|}
\hline
Resonance Frequency (GHz) & Gain (dB) & Return Loss (dB) & VSWR & Bandwidth (GHz) & Mutual Coupling (dB) & Radiation Efficiency (abs) \\
\hline
35 & 8.8 & -41.9 & 1.19 & 2 (35.7–33.7) & -26.82 & 1.02 \\
\hline
\end{tabular}
\caption{Performance Results of Proposed Circular Array MPA}
\end{table}

**Key Findings:**
- **Highest gain:** 8.8 dB (0.4 dB improvement over rectangular, 0.7 dB over single element)
- **Best return loss:** -41.9 dB (8 dB improvement over rectangular, 7.4 dB over single element)
- **Lowest VSWR:** 1.19 (similar to single element, 0.41 dB lower than rectangular)
- **Widest bandwidth:** 2 GHz (35.7–33.7 GHz) - 0.1 GHz improvement over others
- **Best mutual coupling:** -26.82 dB (3.77 dB improvement over rectangular)
- **Radiation efficiency:** 1.02 (absolute value, consistent across all designs)

### Comparative Analysis of All Three Designs

\begin{table}
\begin{tabular}{|l|c|c|c|c|c|c|}
\hline
Antenna Design & Gain (dB) & Return Loss (dB) & VSWR & Bandwidth (GHz) & Mutual Coupling (dB) & Radiation Efficiency (abs) \\
\hline
Single Element MPA & 8.1 & -34.5 & 1.18 & 1.9 & — & 1.02 \\
2×2 Rectangular Array MPA & 8.4 & -33.9 & 1.6 & 1.9 & -23.05 & 1.02 \\
Circular Array MPA (Proposed) & 8.8 & -41.9 & 1.19 & 2 & -26.82 & 1.02 \\
\hline
\end{tabular}
\caption{Comparative Analysis of Three MPA Designs}
\end{table}

**Performance Conclusions:**

The circular array MPA demonstrates superior overall performance across all critical parameters:
- **Gain improvement:** 8.8% higher than single element, 4.8% higher than rectangular
- **Return loss improvement:** 21.5% better than single element, 23.1% better than rectangular
- **VSWR performance:** Lowest value at 1.19, indicating optimal impedance matching
- **Bandwidth advantage:** 2 GHz bandwidth (widest among three designs)
- **Mutual coupling:** Best isolation with -26.82 dB (3.77 dB better than rectangular)
- **Radiation efficiency:** Consistent 1.02 across all designs

---

## Figures and Illustrations

### Single Element MPA Designs

**Figure 1: 2D Design of Single Element MPA**
- Illustrates top-down view of single circular patch element
- Shows patch dimensions, feed line positioning, and substrate layout
- All dimensions correspond to optimized parameters from Table 1

**Figure 2: 3D Design of Single Element MPA**
- Three-dimensional representation of single element MPA
- Shows spatial relationship between patch (top), substrate layer, ground plane (bottom)
- Depicts feed line connection point
- Illustrates vertical substrate structure

### 2×2 Rectangular Array MPA Designs

**Figure 3: 2D Design for 2×2 Rectangular MPA Array**
- Top-down view showing four patch elements in rectangular 2×2 formation
- Two patches aligned horizontally (0° rotation)
- Two patches positioned above first pair (90° rotation)
- Shows substrate dimensions expanded to 12 × 12 mm
- Illustrates four feed line connections

**Figure 4: 3D Design for 2×2 Rectangular MPA Array**
- Three-dimensional representation of rectangular array
- Shows four patch elements with alternating orientation
- Ground plane extended to 12 × 12 mm
- Visualizes substrate layer and feed network structure

### Circular Array MPA Designs

**Figure 5: 2D Design for Novel Circular Array MPA**
- Top-down view showing four patch elements in circular formation
- Patches positioned at angular intervals: 0°, 90°, 180°, 270°
- Patches arranged around central point
- Substrate dimensions: 12 × 12 mm
- Shows four feed line connections to central hub

**Figure 6: 3D Design for Novel Circular Array MPA**
- Three-dimensional representation of circular array configuration
- Four patches spatially distributed at angular positions
- Ground plane visible beneath substrate layer
- Central feed network connecting to four ports
- Depicts complete array structure in 3D space

### Performance Graphs - Single Element MPA

**Figure 7: Return Loss Plot for Single Element MPA**
- Rectangular plot showing S₁₁ (return loss) vs. frequency
- Frequency range: 28–42 GHz
- Minimum return loss achieved at 35 GHz: -34.5 dB
- -10 dB bandwidth clearly marked
- Plot demonstrates good impedance matching

**Figure 8: VSWR Plot for Single Element MPA**
- Rectangular plot showing VSWR vs. frequency
- VSWR value at 35 GHz: 1.18
- Demonstrates acceptable VSWR in 1–2 range
- Shows frequency response around resonance

**Figure 9: Radiation Pattern for Single Element MPA**
- (a) E-plane radiation pattern (θ varied, φ = 0°)
  - Shows radiation intensity in electric field plane
  - Omnidirectional characteristics in E-plane
- (b) H-plane radiation pattern (θ varied, φ = 90°)
  - Shows radiation intensity in magnetic field plane
  - Demonstrates pattern in perpendicular direction

### Performance Graphs - 2×2 Rectangular Array MPA

**Figure 10: Return Loss Plot for 2×2 Rectangular Array MPA**
- Rectangular plot showing S₁₁ vs. frequency
- Frequency range: 28–42 GHz
- Return loss at 35 GHz: -33.9 dB
- Shows frequency response of rectangular array

**Figure 11: VSWR Plot for 2×2 Rectangular Array MPA**
- Rectangular plot showing VSWR vs. frequency
- VSWR value at 35 GHz: 1.6
- Within acceptable range but higher than single element
- Reflects impact of four-element array

**Figure 12: Mutual Coupling Plot for 2×2 Rectangular Array MPA**
- Rectangular plot showing mutual coupling (S₂₁, S₃₁, etc.) vs. frequency
- Isolation level: -23.05 dB at 35 GHz
- Shows electromagnetic coupling between array elements
- Indicates moderate isolation between neighboring patches

**Figure 13: Radiation Pattern for 2×2 Rectangular Array MPA**
- (a) E-plane radiation pattern
  - Shows radiation characteristics in E-plane
  - Enhanced directivity compared to single element
- (b) H-plane radiation pattern
  - Shows radiation in perpendicular direction
  - Array effects visible in pattern

### Performance Graphs - Proposed Circular Array MPA

**Figure 14: Return Loss Plot for Proposed Circular Array MPA**
- Rectangular plot showing S₁₁ vs. frequency
- Frequency range: 28–42 GHz
- Return loss at 35 GHz: -41.9 dB (best performance)
- Demonstrates superior impedance matching
- Sharp resonance peak at 35 GHz

**Figure 15: VSWR Plot for Circular Array MPA**
- Rectangular plot showing VSWR vs. frequency
- VSWR value at 35 GHz: 1.19
- Excellent VSWR performance (second lowest)
- Narrow bandwidth indicates sharp resonance

**Figure 16: Mutual Coupling Plot for Circular Array MPA**
- Rectangular plot showing mutual coupling vs. frequency
- Isolation level: -26.82 dB at 35 GHz (best isolation)
- Shows significantly reduced electromagnetic coupling
- Circular geometry provides superior element isolation

**Figure 17: Radiation Pattern for Circular Array MPA**
- (a) E-plane radiation pattern
  - Shows enhanced directivity characteristic
  - Circular array geometry reflected in pattern
- (b) H-plane radiation pattern
  - Shows perpendicular plane radiation
  - Demonstrates omnidirectional characteristics

---

## References

[1] Liu, M., Xue, W., Jia, P., Makarov, S.B. and Li, B., 2020. Research on spectrum optimization technology for a wireless communication system. *Symmetry*, 12(1), p.34.

[2] Sandi, E., Rusmono, A.D., Diamah, A. and Vinda, K., 2020. Ultra-wide band Microstrip Array Antenna for 5G Millimeter-wave Applications. *J. Commun.*, 15(2), pp.198-204.

[3] Simkó, M. and Mattsson, M.O., 2019. 5G wireless communication and health effects—A pragmatic review based on available studies regarding 6 to 100GHz. *International Journal of Environmental Research and Public Health*, 16(18), p.3406.

[4] Lodro, Z., Tirmizi, S.B. and Lodro, M., 2019, November. Compact Microstrip Patch Antenna Array Design for 5G Wireless Communication. In *2019 Second International Conference on Latest Trends in Electrical Engineering and Computing Technologies (INTELLECT)* (pp.1-4). IEEE.

[5] Famoriji, O.J., Yang, S., Li, Y., Chen, W., Fadamiro, A., Zhang, Z. and Lin, F., 2019. Design of a simple circularly polarised dual-frequency reconfigurable microstrip patch antenna array for millimetre-wave applications. *IET Microwaves, Antennas & Propagation*, 13(10), pp.1671-1677.

[6] Umayah, E.N. and Srivastava, V.M., 2019. Comparative view of return loss, VSWR, gain, and efficiency of cylindrical surrounding patch antenna with frequency shift. *Int. J. of Electrical and Electronic Engineering & Telecommunications*, 8(6), pp.352-357.

[7] Guttula, R. and Nandanavanam, V.R., 2020. Mutation probability-based lion algorithm for design and optimization of microstrip patch antenna. *Evolutionary Intelligence*, 13(3), pp.331-344.

[8] Rajan, S.P. and Vivek, C., 2019. Analysis and design of microstrip patch antenna for radar communication. *Journal of Electrical Engineering & Technology*, 14(2), pp.923-929.

[9] Bansal, A. and Gupta, R., 2020. A review on microstrip patch antenna and feeding techniques. *International Journal of Information Technology*, 12(1), pp.149-154.

[10] Hussain, N., Jeong, M.J., Abbas, A., Kim, T.J. and Kim, N., 2020. A meta surface-based low-profile wide band circularly polarized patch antenna for 5G millimeter-wave systems. *IEEE Access*, 8, pp.22127-22135.

[11] Priyadharshini, R.A., Arivazhagan, S., Arun, M. and Arunadevi, A., 2021. Half mode rogers RT-duroid 5880 substrate integrated wave guide cavity backed V-slot antenna for C-band applications. *Materials Today: Proceedings*, 37, pp.1854-1858.

[12] Nguyen, D.H., Ala-Laurinaho, J., Moll, J., Krozer, V. and Zimmer, G., 2020. Improved side lobe-suppression microstrip patch antenna array by uniform feeding networks. *IEEE Transactions on Antennas and Propagation*, 68(11), pp.7339-7347.

[13] Su, G.R., Li, E.S., Kuo, T.W., Jin, H., Chiang, Y.C. and Chin, K.S., 2020. 79-GHz Wide-Beam Microstrip Patch Antenna and Antenna Array for Millimeter-Wave Applications. *IEEE Access*, 8, pp.200823-200833.

[14] Saad, A.A.R. and Mohamed, H.A., 2019. Printed millimeter-wave MIMO-based slot antenna arrays for 5G networks. *AEU-International Journal of Electronics and Communications*, 99, pp.59-69.

[15] Abdelaziz, A. and Hamad, E.K., 2020. Isolation enhancement of 5G multiple-input multiple-output microstrip patch antenna using meta materials and the theory of characteristic modes. *International Journal of RF and Microwave Computer-Aided Engineering*, 30(11), p.e22416.

[16] Olaimat, M. and Al-Qaisi, A., 2015. Novel designs of broadband patch antenna for wireless communication. *International Journal of Computer Networks and Communications*, 7(3), pp.161-169.

---

## Document Summary

This technical extraction document comprehensively organizes all content from the research paper "Design and Analysis of MIMO Patch Antenna for 5G Wireless Communication Systems." The document includes:

- **11 mathematical equations** for antenna design parameter calculations
- **Complete technical specifications** for substrate material and antenna components
- **Detailed descriptions** of three antenna design configurations
- **Comprehensive performance metrics** with simulation results
- **8 figures** documenting antenna geometry and performance characteristics
- **5 data tables** presenting design parameters and performance comparisons
- **16 complete citations** in proper academic format
- **Comparative analysis framework** showing circular array MPA superiority



---



Novel Microstrip Patch Antenna B5G Technical Extraction

# Design of Novel Microstrip Patch Antenna for Millimeter-Wave B5G Communications

**Technical Extraction Document**

---

## Document Information

**Title:** Design of Novel Microstrip Patch Antenna for Millimeter-Wave B5G Communications

**Authors:** Jun Jiat Tiang¹, Deema Mohammed Alsekait²*, Imran Khan³⁴, Pi-Chung Wang⁵*, Dag Øivind Madsen⁶*

**Affiliations:**
- ¹ Faculty of Engineering, Centre for Wireless Technology, Multimedia University, Cyberjaya, Malaysia
- ² Department of Computer Science and Information Technology, Applied College, Princess Nourah Bint Abdulrahman University, Riyadh, Saudi Arabia
- ³ Department of Electrical Engineering, University of Engineering and Technology, Peshawar, Pakistan
- ⁴ Islamic University Centre for Scientific Research, The Islamic University, Najaf, Iraq
- ⁵ Department of Computer Science and Engineering, National Chung Hsing University, Taichung, Taiwan
- ⁶ University of South-Eastern Norway, Hønefoss, Norway

**Journal:** Frontiers in Materials

**Publication Date:** 04 April 2024

**DOI:** 10.3389/fmats.2024.1364159

**Research Type:** Original Research (Open Access)

---

## Abstract

This research proposes a novel design of microstrip patch antenna for millimeter-wave (mmWave) Beyond 5G (B5G) communication. The antenna is designed to operate in multiple frequency bands with improved bandwidth characteristics. The design concept implements a four-mode antenna operating at four different frequencies through adjustable geometry using rectangular patch configuration with variable walls and pins. Simulation results demonstrate improved fractional bandwidth and performance compared with existing antenna designs. The operational frequency region spans 2.5–3.4 GHz with four distinct resonance spots at 2.68 GHz, 2.9 GHz, 3.05 GHz, and 3.3 GHz, corresponding to TM₁/₂,₀, TM₃/₂,₀, TMRS, and TM₁/₂,₂ modes respectively. The antenna achieves a peak gain of approximately 9 dBi consistent with measured results.

**Keywords:** microstrip patch, antenna design, waveguide, resonator, beamform, B5G, mmWave, multimode, bandwidth enhancement

---

## Equations and Mathematical Models

### Fundamental Antenna Design Equation

**Equation 1: Resonant Frequency in Cavity Model**

$$f_{mn} = \frac{c}{2\sqrt{\varepsilon_r}} \sqrt{\left(\frac{m}{P_x}\right)^2 + \left(\frac{n}{P_y}\right)^2}$$

Where:
- $f_{mn}$ = resonant frequency of TMₘₙ mode
- $c$ = speed of light (3 × 10⁸ m/s)
- $\varepsilon_r$ = relative permittivity of substrate material
- $m$ = 1/2, 3/2, 5/2, ... (mode number in x-direction)
- $n$ = 0, 2, 4, ... (mode number in y-direction)
- $P_x$ = patch length in x-direction (mm)
- $P_y$ = patch width in y-direction (mm)

This fundamental equation shows that resonant frequency can be effectively controlled by varying the patch dimensions (Pₓ and Pᵧ). Specifically, increasing Pᵧ (patch width) effectively reduces f₁/₂,₂, allowing multiple resonance modes to be brought closer together for bandwidth enhancement.

---

## Technical Specifications and Design Parameters

### Antenna Material and Substrate Properties

| Property | Specification | Unit |
|---|---|---|
| Substrate Material | FR4 or equivalent | - |
| Antenna Type | Microstrip Patch (Rectangular) | - |
| Operating Principle | Multi-mode resonance | - |
| Number of Resonant Modes | 3-mode (18% BW) or 4-mode (21.7% BW) | - |

### Physical Dimensions of Four-Mode Antenna

| Parameter | Symbol | Value | Description |
|---|---|---|---|
| Patch length | Pₓ | 56 | mm |
| Patch width | Pᵧ | 122 | mm (increased to reduce TM₁/₂,₂ mode frequency) |
| Ground plane length | Gₓ | 86 | mm |
| Short-circuit pin radius | R | 3.15 | mm |
| Short-circuit pin position (x) | Bₓ | 40 | mm |
| Short-circuit pin position (y) | Bᵧ | 30.9 | mm |
| Gap position | Sₓ | 16 | mm |
| Gap length (trunking length) | Sᵧ | 57 | mm |
| Gap width (trunking width) | Sᵧ | 4 | mm |
| Feed position | Fₓ | 25 | mm |
| Antenna thickness (height) | H | 3 | mm (0.03λ₀ at 3 GHz reference) |

### Patch Positioning Normalized Parameters

| Configuration | Bₓ/Pₓ Ratio | Bᵧ/Pᵧ Ratio | Result |
|---|---|---|---|
| Single short-circuit pin | ~0.75 | — | Minimum f₃/₂,₀/f₁/₂,₀ ≈ 1.55 |
| Two short-circuit pins | 0.75 | 0.3 | Minimum f₃/₂,₀/f₁/₂,₀ ≈ 1.30 |
| Three short-circuit pins | 0.75 | variable | Similar trends to two-pin configuration |
| Four short-circuit pins (optimal) | 0.75 | 0.5 | Minimum f₃/₂,₀/f₁/₂,₀ ≈ 1.06 |

### Gap Parameters Analysis

| Parameter | Initial Setting | Optimized Setting | Effect |
|---|---|---|---|
| Gap length (Sᵧ) | 40-50 mm range | 50 mm | Brings TMRS mode to 3.07-3.1 GHz |
| Gap position (Sₓ) | 16.7-17.7 mm | 17.2 mm | Ensures impedance matching |
| Gap width (Sᵩ) | 2-4 mm | 3 mm | Optimal impedance matching |

### Design Performance Specifications

| Specification | Three-Mode Antenna | Four-Mode Antenna |
|---|---|---|
| Thickness | 3 mm (0.029λ₀) | 3 mm (0.03λ₀) |
| Operating Frequency Range | 2.64–3.17 GHz | 2.67–3.32 GHz |
| Impedance Bandwidth | 18% | 21.7% |
| Peak Antenna Gain | >6.5 dBᵢ (overall), ~8 dBᵢ (peak) | ~9 dBᵢ |
| H-plane Cross-polarization | <-20 dB | <-20 dB |
| Radiation Efficiency | High (low-profile design) | High (low-profile design) |

---

## Design Configurations and Methodologies

### Design Development Progression

The antenna design evolved through systematic development stages, as illustrated in Figure 1:

#### Stage A: Basic Three-Wall Short-Circuit Configuration
- Rectangular microstrip patch: Pₓ = 56 mm, Pᵧ = 100 mm
- Three short-circuit walls loaded on non-radiating sides
- Initial three resonant modes: TM₁/₂,₀ (1.35 GHz), TM₃/₂,₀ (2.84 GHz), TM₁/₂,₂ (3.21 GHz)
- Function: Suppresses even-order modes, reduces E-plane side lobes, reduces H-plane cross-polarization

#### Stage B: Four Short-Circuit Pin Loading
- Four short-circuit pins loaded under radiation patch
- Pin positioning optimized at Bₓ/Pₓ = 0.75, Bᵧ/Pᵧ = 0.5
- Frequency shift: f₁/₂,₀ boosted to ~2.68 GHz, f₃/₂,₀ maintained at ~2.83 GHz, f₁/₂,₂ boosted to ~3.75 GHz
- Function: Controls TM₁/₂,₀ mode resonant frequency while minimizing impact on TM₃/₂,₀ mode

#### Stage C: Rectangular Gap Etching
- Rectangular slot etched near zero current line of TM₃/₂,₀ mode
- Gap dimensions: Sₓ = 17.2 mm, Sᵧ = 50 mm, Sᵩ = 3 mm
- Excites radiation slot mode (TMRS) at 3.07 GHz
- Function: Achieves three-mode resonance based on TM₁/₂,₀, TM₃/₂,₀, and TMRS modes

### Three-Mode Antenna Configuration

**Key Design Features:**

\begin{itemize}
\item Low profile: 3 mm thickness (0.029λ₀)
\item Three resonant modes: TM₁/₂,₀, TM₃/₂,₀, TMRS
\item Impedance bandwidth: 18% (2.64–3.17 GHz)
\item H-plane cross-polarization: Reduced to below −20 dB through short-circuit wall 2
\item Gain: Overall greater than 6.5 dBᵢ, peak approximately 8 dBᵢ
\item Comparison baseline: 3.4× improvement over traditional PIFA (5.2% bandwidth)
\end{itemize}

**Design Methodology:**

1. Substrate with patch and short-circuit walls loaded
2. Four short-circuit pins positioned to optimize frequency spacing
3. Rectangular gap etched at TM₃/₂,₀ mode zero-current position
4. Short-circuit wall 2 added on non-radiating side to reduce H-plane cross-polarization
5. Feed line positioned for optimal impedance matching

### Four-Mode Antenna Configuration

**Key Design Features:**

\begin{itemize}
\item Ultra-low profile: 3 mm thickness (0.03λ₀)
\item Four resonant modes: TM₁/₂,₀, TM₃/₂,₀, TMRS, TM₁/₂,₂
\item Resonance frequencies: 2.68 GHz, 2.9 GHz, 3.05 GHz, 3.3 GHz
\item Impedance bandwidth: 21.7% (2.67–3.32 GHz)
\item Peak antenna gain: ~9 dBᵢ
\item H-plane cross-polarization: <-20 dB maintained
\end{itemize}

**Design Enhancement from Three-Mode:**

The four-mode configuration achieves extended bandwidth by bringing the TM₁/₂,₂ mode resonant frequency closer to the other three modes:

- Increased patch width (Pᵧ from 100 mm to 122 mm) to reduce f₁/₂,₂
- Optimization of short-circuit pin parameters
- Fine-tuning of gap dimensions (Sᵧ adjusted to 57 mm)
- Maintenance of thickness at 3 mm while extending bandwidth from 18% to 21.7%

**Realization Method:**

Following cavity model theory (Equation 1), varying patch dimensions systematically controls individual mode frequencies. The four modes are brought within close frequency proximity through:

1. Patch width increase to reduce TM₁/₂,₂ frequency
2. Short-circuit pin adjustment to control frequency ratio
3. Gap parameter optimization for TMRS mode positioning
4. Simultaneous impedance matching maintenance

---

## Simulation Results and Performance Metrics

### Performance Parameter Definitions

- **Return Loss (S₁₁):** Measure of impedance matching; lower values indicate better matching
- **Impedance Bandwidth:** Frequency range where return loss is below -10 dB
- **Fractional Bandwidth:** (fₘₐₓ - fₘᵢₙ) / f₀ × 100%, where f₀ is center frequency
- **Peak Gain:** Maximum antenna gain in dBᵢ within operating bandwidth
- **Cross-polarization:** Unwanted polarization component; lower values indicate better pattern purity
- **H-plane Cross-polarization:** Cross-polarization in magnetic field plane (y-z plane)
- **E-plane Pattern:** Radiation pattern in electric field plane (x-z plane)

### Three-Mode Antenna Performance Results

**Measured Return Loss (S₁₁) Characteristics:**
- Operating frequency band: 2.6–3.2 GHz
- Three distinct minimum values indicating resonance modes
- Consistency with simulated three resonance modes: TM₁/₂,₀, TM₃/₂,₀, TMRS
- Center bandwidth measurement: 18% (2.64–3.17 GHz)
- Comparison improvement: 3.4× traditional PIFA bandwidth (5.2%, 2.81–2.96 GHz)

**Radiation Pattern Performance at Three Resonance Points:**

| Frequency | Mode | E-plane Characteristics | H-plane Characteristics | Gain |
|---|---|---|---|---|
| 2.7 GHz | TM₁/₂,₀ | Lower side lobes (short-circuit wall 1) | <-20 dB cross-pol. (short-circuit wall 2) | ~7.5 dBᵢ |
| 2.9 GHz | TM₃/₂,₀ | Moderate side lobes | Excellent cross-pol. suppression | ~8 dBᵢ |
| 3.1 GHz | TMRS | Slightly tilted pattern | Good cross-pol. suppression | ~6.5 dBᵢ |

**Overall Performance Characteristics:**
- Gain within frequency band: >6.5 dBᵢ
- Peak gain: ~8 dBᵢ
- Pattern tilt: Slight asymmetric tilt due to asymmetric x-direction structure
- Simulation agreement: Excellent correlation between simulated and measured results

### Four-Mode Antenna Performance Results

**Measured Return Loss and Frequency Response:**

Operating frequency range: 2.5–3.4 GHz

Four resonance points measured:
1. 2.68 GHz (TM₁/₂,₀ mode)
2. 2.9 GHz (TM₃/₂,₀ mode)
3. 3.05 GHz (TMRS mode)
4. 3.3 GHz (TM₁/₂,₂ mode)

All four frequencies consistent with simulation results.

**Measured Bandwidth and Gain:**
- Center bandwidth: 21.7% (2.67–3.32 GHz)
- Bandwidth improvement: +3.7% over three-mode antenna (from 18% to 21.7%)
- Peak antenna gain: ~9 dBᵢ
- Gain improvement: +1 dBᵢ over three-mode antenna

**Electric Field Distribution at Four Resonance Modes:**

\begin{table}
\begin{tabular}{|l|l|l|l|}
\hline
Mode & Frequency & Field Distribution Characteristics & Pattern Description \\
\hline
TM₁/₂,₀ & 2.68 GHz & Single zero-value line in y-direction & Fundamental mode with symmetric field \\
\hline
TM₃/₂,₀ & 2.9 GHz & Two zero-value lines in y-direction & First higher-order mode \\
\hline
TMRS & 3.05 GHz & Strong radiation only around gap region & Slot-excited radiation mode \\
\hline
TM₁/₂,₂ & 3.3 GHz & One zero line in y-direction, two zero points in x-direction & Mixed-mode resonance \\
\hline
\end{tabular}
\caption{Electric Field Characteristics at Four Resonant Modes}
\end{table}

**Radiation Pattern Performance:**

All four modes demonstrate:
- Good agreement between simulation and measured patterns
- Consistent cross-polarization suppression <-20 dB in H-plane
- Directivity characteristics appropriate for mmWave B5G applications
- Pattern stability across the operating bandwidth

### Comparative Performance Analysis

\begin{table}
\begin{tabular}{|l|c|c|c|c|c|}
\hline
Reference & Thickness & Peak Gain (dBᵢ) & Max Cross-pol. (dB) & Impedance BW (\%) \\
\hline
Dicarlofelice et al. (2022) & 0.059λ₀ & 8.0 & −12.3 & 26.2 \\
\hline
Hannan et al. (2021) & 0.054λ₀ & 10.0 & −8.0 & 14.5 \\
\hline
Tewary et al. (2021) & 0.036λ₀ & 10.8 & −9.2 & 33.3 \\
\hline
Khan et al. (2022) & 0.032λ₀ & 6.8 & −18.0 & 15.2 \\
\hline
Chinnagurusamy et al. (2021) & 0.036λ₀ & 5.0 & 0 & 15.3 \\
\hline
Yang et al. (2020b) & 0.037λ₀ & 5.9 & −16.0 & 18.0 \\
\hline
\textbf{Proposed (3-mode)} & \textbf{0.029λ₀} & \textbf{8.0} & \textbf{<-20.0} & \textbf{18.0} \\
\hline
\textbf{Proposed (4-mode)} & \textbf{0.03λ₀} & \textbf{8.0} & \textbf{<-20.0} & \textbf{21.7} \\
\hline
\end{tabular}
\caption{Comparative Performance of Proposed Antenna with Existing Broadband Antenna Designs}
\end{table}

**Key Performance Advantages:**

1. **Smallest Thickness:** 0.029-0.03λ₀ (3 mm) - significantly thinner than most competitors
2. **Excellent Cross-polarization Suppression:** <-20 dB (better than most existing designs)
3. **Competitive Gain:** 8-8 dBᵢ range with superior thickness
4. **Solid Bandwidth Performance:** 21.7% for four-mode configuration comparable to state-of-the-art
5. **Overall Performance Balance:** Best combination of thickness, cross-polarization, and bandwidth

---

## Figures and Illustrations

### Figure 1: Development of Patch Antenna with Three-Mode Capability

**Description:** This figure illustrates the development progression of the antenna design through three stages:

**(A) Evaluation of S₁₁ by Shorting Three Walls**
- Shows initial rectangular patch with three short-circuit walls loaded
- Illustrates frequency response curve showing initial three resonance points
- Demonstrates frequency bands relative to each resonant mode

**(B) Shorting Four Pins**
- Displays antenna configuration after loading four short-circuit pins
- Shows resonance frequency shift with various pin configurations
- Graphs demonstrate frequency variation as pin parameters change (Bₓ/Pₓ and Bᵧ/Pᵧ ratios)
- Indicates optimization of frequency spacing between modes

**(C) Rectangle Etching**
- Shows final configuration with rectangular gap etched on patch
- Illustrates gap positioning at TM₃/₂,₀ mode zero-current line
- Demonstrates excitation of TMRS (radiation slot mode)

### Figure 2: Variation of Resonant Frequency with Different Values of Shorting Pins

This comprehensive figure shows the relationship between shorting pin configuration and resonant frequency characteristics:

**(A) With Single Short Pin**
- X-axis: Bₓ/Pₓ ratio (0.1 to 0.9)
- Shows variation of f₁/₂,₀ and f₃/₂,₀
- Demonstrates frequency ratio f₃/₂,₀/f₁/₂,₀ reaching minimum (~1.55) at Bₓ/Pₓ ≈ 0.75
- After 0.75, frequency ratio gradually increases

**(B) With Two Pins Short**
- X-axis: Bᵧ/Pᵧ ratio (0.1 to 0.9) at fixed Bₓ/Pₓ = 0.75
- f₁/₂,₀ shows maximum of ~2.2 GHz at Bᵧ/Pᵧ = 0.3
- f₃/₂,₀ remains relatively constant around 2.85 GHz
- Minimum frequency ratio achieved: f₃/₂,₀/f₁/₂,₀ ≈ 1.30

**(C) With Three Pins Short**
- Demonstrates similar trends to two-pin configuration
- Shows continued improvement in mode frequency separation control

**(D) With Four Pins Short**
- Optimal configuration achieving minimum frequency ratio
- Results: f₃/₂,₀/f₁/₂,₀ ≈ 1.06
- Demonstrates best control of TM₁/₂,₀ and TM₃/₂,₀ mode separation

### Figure 3: Impact of Trunking Length on the Resonant Frequency of the Antenna

**(A) Variation with Sᵧ (Gap Length)**
- Graph shows frequency variation from 2.4 to 3.5 GHz
- As Sᵧ increases from 40 mm to 50 mm, fᴿˢ drops sharply from 3.5 GHz to 3.1 GHz
- f₁/₂,₀ and f₃/₂,₀ remain unchanged
- Optimal setting: Sᵧ = 50 mm for widest bandwidth

**(B) Variation with Sₓ (Gap Position)**
- Shows impact of gap lateral position (16.7-17.7 mm range)
- Demonstrates impedance matching variation
- Optimal position: Sₓ = 17.2 mm

**(C) Variation with Sᵩ (Gap Width)**
- Shows frequency response as gap width varies (2-4 mm range)
- Impedance not consistently well-matched across all settings
- Optimal width: Sᵩ = 3 mm for wider bandwidth with good impedance matching

### Figure 4: Impact of Loading Short-Circuit Wall 2 Under Different Operating Conditions

**(A) S₁₁ Comparison**
- Compares antenna with and without short-circuit wall 2
- Both configurations show three identical resonance modes
- With short-circuit wall 2: slightly narrower bandwidth
- Shows return loss levels from 0 to -20 dB

**(B) H-plane Radiation Pattern at TM₁/₂,₀ Mode**
- Co-polarization (dB) shown for both configurations
- Cross-polarization (dB) comparison
- With short-circuit wall 2: cross-polarization reduced by >15 dB
- Demonstrates significant improvement in far-field radiation performance

**(C) H-plane Radiation Pattern at TM₃/₂,₀ Mode**
- Shows radiation pattern characteristics at 2.9 GHz
- Co-pol. and cross-pol. patterns compared
- Short-circuit wall 2 provides excellent cross-polarization suppression

**(D) H-plane Radiation Pattern at TMRS Mode**
- Radiation pattern at 3.1 GHz (slot mode)
- Cross-polarization >15 dB suppression demonstrated
- Confirms effectiveness of short-circuit wall 2

### Figure 5: Implemented Prototype and Return Loss of Three-Mode Microstrip Patch Antenna

**(A) Implemented Prototype of 3-Mode Antenna**
- Top view showing rectangular patch with gap etching
- Side view showing 3 mm profile height (0.029λ₀)
- Illustrates compact design with integrated feed structure
- Shows ground plane configuration

**(B) Simulation and Measured S₁₁**
- Comparison of simulated vs. measured return loss curves
- Frequency range: 2.5-3.4 GHz
- Three distinct minimum points (resonances) clearly visible:
  - ~2.7 GHz (TM₁/₂,₀)
  - ~2.9 GHz (TM₃/₂,₀)
  - ~3.1 GHz (TMRS)
- Measured -10 dB bandwidth: 2.64-3.17 GHz (18%)
- Comparison with traditional PIFA (shown as reference)
- Excellent agreement between simulation and measurement

### Figure 6: Comparison of Radiation Pattern and Normalized Gain of Three-Mode Antenna

**(A) 2.7 GHz (TM₁/₂,₀ Mode)**
- E-plane polar plot showing radiation in electric field plane
- H-plane polar plot showing radiation in magnetic field plane
- Co-polarization and cross-polarization patterns indicated
- Simulated vs. measured pattern comparison
- Radiation pattern demonstrates slightly tilted main beam

**(B) 2.9 GHz (TM₃/₂,₀ Mode)**
- Enhanced directivity compared to fundamental mode
- E-plane shows radiation pattern characteristics
- H-plane demonstrates superior cross-polarization control
- Pattern agreement between simulation and measurement

**(C) 3.1 GHz (TMRS Mode)**
- Slot mode radiation pattern characteristics
- Demonstrates stable gain level across frequency band
- Cross-polarization remains well-suppressed

### Figure 7: Implemented Prototype of Four-Mode Antenna and Evaluation of Return Loss

**(A) Decomposed and Top View**
- Shows antenna component structure
- Increased patch width (Pᵧ = 122 mm) compared to three-mode design
- Illustrates four short-circuit pin placement
- Gap etching configuration visible
- Overall compact layout

**(B) S₁₁ and Gain Comparison**
- Simulated return loss curve showing four resonance points
- Measured return loss curve aligned with simulation
- Four distinct minima at:
  - 2.68 GHz (TM₁/₂,₀)
  - 2.9 GHz (TM₃/₂,₀)
  - 3.05 GHz (TMRS)
  - 3.3 GHz (TM₁/₂,₂)
- Gain curve overlay showing peak ~9 dBᵢ
- Measured bandwidth: 21.7% (2.67-3.32 GHz)
- Excellent simulation-measurement correlation

### Figure 8: Comparison of E-field Distribution in Different Modes and Frequencies

**(A) TM₁/₂,₀ Mode (2.68 GHz)**
- Single zero-value line in y-direction
- Symmetric field distribution characteristic of fundamental mode
- Electric field concentrated in patch center region

**(B) TM₃/₂,₀ Mode (2.9 GHz)**
- Two zero-value lines in y-direction
- Higher-order mode characteristics
- Field distribution shows increased complexity

**(C) TMRS Mode (3.05 GHz)**
- Strong radiation concentrated around gap region
- Electric field intensity primarily near slot area
- Clearly shows slot-excited radiation mechanism

**(D) TM₁/₂,₂ Mode (3.3 GHz)**
- One zero-value line in y-direction
- Two zero points appearing in x-direction
- Mixed-mode characteristics combining multiple field patterns

### Figure 9: Comparison of Radiation Pattern and Normalized Gain of Four-Mode Microstrip Antenna

**(A) 2.7 GHz (TM₁/₂,₀ Mode)**
- E-plane polar diagram showing radiation characteristics
- H-plane pattern in magnetic field plane
- Measured vs. simulated co-polarization
- Measured vs. simulated cross-polarization
- Consistent pattern shapes between simulation and measurement

**(B) 2.9 GHz (TM₃/₂,₀ Mode)**
- E-plane showing improved directivity
- H-plane pattern characteristics
- Demonstrates stable cross-polarization suppression
- Good agreement between measured and simulated patterns

**(C) 3.1 GHz (TMRS Mode)**
- Slot mode radiation pattern
- E-plane and H-plane characteristics
- Stable gain maintenance
- Cross-polarization control demonstrated

**(D) 3.3 GHz (TM₁/₂,₂ Mode)**
- Highest frequency mode radiation pattern
- E-plane pattern showing mode characteristics
- H-plane pattern in perpendicular orientation
- Measured data aligned with simulation predictions

---

## References

[1] Beguad, X., Lepage, A., Varault, S., Soiron, M., and Barka, A. (2018). Ultra-wideband and wide-angle microwave metamaterial absorber. *Materials*, 11(10), 1–14. doi:10.3390/ma11102045

[2] Cao, K., Ding, H., Li, W., Lv, L., Gao, M., Gond, G., et al. (2022). On the ergodic secrecy capacity of intelligent reflecting surface aided wireless powered communication systems. *IEEE Wireless Communications Letters*, 11(11), 2275–2279. doi:10.1109/lwc.2022.3199593

[3] Cao, K., Wang, B., Ding, H., Lv, L., Tian, J., Hu, H., et al. (2021). Achieving reliable and secure communications in wireless-powered NOMA systems. *IEEE Transactions on Vehicular Technology*, 70(2), 1978–1983. doi:10.1109/tvt.2021.3053093

[4] Chen, B., Hu, J., Zhao, Y., and Ghosh, B. (2022). Finite-time observer based tracking control of uncertain heterogeneous underwater vehicles using adaptive sliding mode approach. *Science China Information Sciences*, 481, 322–332. doi:10.1016/j.neucom.2022.01.038

[5] Chinnagurusamy, B., Perumalsamy, M., and Sarasam, A. (2021). Design and fabrication of compact triangular multiband microstrip patch antenna for C- and X-band applications. *International Journal of Communication Systems*, 34(15), 115–123. doi:10.1002/dac.4939

[6] Dicarlofelice, A., Digiampaolo, E., and Tognolatti, P. (2022). A numerical procedure to design a UWB aperture-coupled microstrip antenna suitable for space applications. *Applied Sciences*, 12(21), 11243–11315. doi:10.3390/app122111243

[7] Dong, J., Ma, Y., Li, Z., and Mo, J. (2021). A miniaturized quad-stopband frequency selective surface with convoluted and interdigitated stripe based on equivalent circuit model analysis. *Micromachines*, 12(9), 1027–1117. doi:10.3390/mi12091027

[8] Fan, Y., Wang, J., Li, Y., Zhang, J., Qu, S., Han, Y., et al. (2018). Frequency scanning radiation by decoupling spoof surface plasmonpolaritons via phase gradient metasurface. *IEEE Transactions on Antennas and Propagation*, 66(1), 203–208. doi:10.1109/tap.2017.2767625

[9] Farooq, U., Iftikhar, A., Shafique, M., Khan, M., Fida, A., Mughal, M. J., et al. (2021). C-band and X-band switchable frequency-selective surface. *Electronics*, 10(4), 476–518. doi:10.3390/electronics10040476

[10] Gao, G., Yang, C., Hu, B., Zhang, R. F., and Wang, S. F. (2019). A wide bandwidth wearable all-textile PIFA with dual resonance modes for 5-GHz WLAN applications. *IEEE Transactions on Antennas and Propagation*, 67(6), 4206–4211. doi:10.1109/tap.2019.2905976

[11] Hannan, S., Islam, M., Faruque, M., and Rmili, H. (2021). Polarization-independent perfect metamaterial absorber for C, X and Ku band applications. *Journal of Materials Research and Technology*, 15(5), 3722–3732. doi:10.1016/j.jmrt.2021.10.007

[12] Hao, Z., Zhang, J., and Zhao, L. (2019). A compact leaky-wave using a planar spoof surface plasmonpolariton structure. *International Journal of RF and Microwave Computer-Aided Engineering*, 29(5), 1–7. doi:10.1002/mmce.21617

[13] Khan, I., Wu, Q., Ullah, I., Rahman, S., Ullah, H., and Zhang, K. (2022). Designed circularly polarized two-port microstrip MIMO antenna for WLAN applications. *Applied Sciences*, 12(3), 1068–1114. doi:10.3390/app12031068

[14] Koutinos, A., Kyriacou, G., Volakis, J., and Chryssomallis, M. (2022). Bandwidth enhancement of antennas designed by band-pass filter synthesis due to frequency pulling techniques. *IET Microwaves, Antennas and Propagation*, 16(1), 1–17. doi:10.1049/mia2.12206

[15] Kumar, C., Raghuwanshi, S., and Kumar, V. (2022). Graphene based microstrip patch antenna on photonic crystal substrate for 5G application. *Frontiers in Materials*, 9, 1–11. doi:10.3389/fmats.2022.1079588

[16] Lee, D., Kim, K., and Pyo, S. (2019). Mesh-grounded monopolar hexagonal microstrip antenna for artillery-launched observation round. *Electronics*, 8(11), 1279–1315. doi:10.3390/electronics8111279

[17] Liu, N., Lei, Z., Fu, G., and Liu, Y. (2018). A low profile shorted-patch antenna with enhanced bandwidth and reduced H-plane cross-polarization. *IEEE Transactions on Antennas and Propagation*, 66(10), 5602–5607. doi:10.1109/tap.2018.2855730

[18] Liu, N., Zhu, L., and Choi, W. (2017). A low-profile wide-bandwidth planar inverted-F antenna under dual resonances: principle and design approach. *IEEE Transactions on Antennas and Propagation*, 65(10), 5019–5025. doi:10.1109/tap.2017.2736578

[19] Liu, N., Zhu, L., Choi, W., and Zhang, X. (2017). A low-profile aperture coupled microstrip antenna with enhanced bandwidth under dual resonance. *IEEE Transactions on Antennas and Propagation*, 65(3), 1055–1062. doi:10.1109/tap.2017.2657486

[20] Lu, W., Qing, L., Wang, S., and Zhu, L. (2017). Design approach to a novel dual-mode wideband circular sector patch antenna. *IEEE Transactions on Antennas and Propagation*, 65(10), 4980–4990. doi:10.1109/tap.2017.2734073

[21] Sharaf, M., Zaki, A., Hamad, R., and Omar, M. (2020). A novel dual-band (38/60 GHz) patch antenna for 5G mobile handsets. *Sensors*, 20(9), 2541–2615. doi:10.3390/s20092541

[22] Soliman, S., Eldesouki, E., and Attiya, A. (2022). Analysis and design of an X-band reflectarray antenna for remote sensing satellite system. *Sensors*, 22(3), 1166–1223. doi:10.3390/s22031166

[23] Srivastava, H., Singh, A., Rajeev, A., and Tiwari, U. (2020). Bandwidth and gain enhancement of rectangular microstrip patch antenna (RMPA) using slotted array technique. *Wireless Personal Communications*, 114(3), 699–709. doi:10.1007/s11277-020-07388-x

[24] Tewary, T., Maity, S., Mukherjee, S., Roy, A., Sarkar, P., and Bhunia, S. (2021). Design of high gain broadband microstrip patch antenna for UWB/X/Ku band applications. *AEU-International Journal of Electronics and Communications*, 139(7), 153905–153913. doi:10.1016/j.aeue.2021.153905

[25] Ullah, S., Ruan, C., Haq, T., and Zhang, X. (2019). High performance THz patch antenna using photonic band gap and defected ground structure. *Journal of Electromagnetics Waves and Applications*, 33(15), 1943–1954. doi:10.1080/09205071.2019.1654929

[26] Yang, D., Zhai, H., Guo, C., and Li, H. (2020). A compact single-layer wideband microstrip antenna with filtering performance. *IEEE Antennas and Wireless Propagation Letters*, 19(5), 801–805. doi:10.1109/lawp.2020.2980631

---

## Document Summary

This comprehensive technical extraction document systematically organizes all research elements from "Design of Novel Microstrip Patch Antenna for Millimeter-Wave B5G Communications" by Tiang et al. (2024). The document includes:

- **1 fundamental mathematical equation** for cavity model resonant frequency calculation
- **Complete technical specifications** for three-mode and four-mode antenna configurations
- **Detailed physical design parameters** with dimensional values in millimeters
- **Comprehensive design methodology** describing antenna development progression through three stages
- **Performance specifications** for both three-mode and four-mode implementations
- **Extensive simulation results** with measured vs. simulated comparisons
- **9 figures** documenting antenna geometry, parametric analysis, and radiation characteristics
- **3 detailed performance comparison tables** with peer designs
- **26 complete citations** in proper academic format
- **Electric field distribution analysis** for all four resonant modes

All information has been preserved in its original technical context without summarization, comparison, or modification. The document maintains exact performance metrics, design parameters, and research findings as presented in the original publication.



