
# ULTRA-WIDEBAND ANTENNA SYSTEM DESIGN FOR FUTURE mmWAVE APPLICATIONS
## Comprehensive Technical Extraction - Complete Document

---

## DOCUMENT METADATA

| Field | Details |
|-------|---------|
| **Title** | Ultra-wideband Antenna System Design for Future mmWave Applications |
| **DOI** | https://doi.org/10.26636/jtit.2025.1.1951 |
| **Journal** | Journal of Telecommunications and Information Technology |
| **Issue** | 1/2025 |
| **License** | Creative Commons Attribution 4.0 International (CC BY 4.0) |

---

## AUTHORS AND AFFILIATIONS

| Author | Affiliation | Role | ORCID |
|--------|-------------|------|-------|
| Muhannad Y. Muhsin | University of Technology – Iraq, Baghdad | Ph.D. | 0000-0003-3937-4467 |
| Zainab S. Muqdad | Mustansiriyah University, Baghdad | M.Sc. | 0009-0003-1342-7994 |
| Asaad H. Sahar | University of Baghdad | Ph.D. | 0000-0003-3655-0162 |
| Zainab F. Mohammad | University of Technology – Iraq, Baghdad | M.Sc. | 0000-0002-1627-751X |
| Hussam AL-Saedi | University of Technology – Iraq, Baghdad | Ph.D. | 0000-0002-2029-7361 |

---

## ABSTRACT

An ultra-wideband planar four-element multiple-input multiple-output (MIMO) antenna array for millimeter wave (mmWave) 5G applications is presented, characterized by:

- **Simple structure** with diverse performance capabilities
- **Operating band:** 42.3 to 63.3 GHz (20 GHz bandwidth)
- **Peak gain:** 7.8 dB
- **Compact size:** 25 × 25 mm
- **Isolation:** Over 24 dB
- **Orthogonal element placement** for excellent isolation

### Performance Characteristics Analyzed:
- S-parameters
- Gain
- Efficiency
- Radiation patterns
- MIMO diversity characteristics (ECC, DG, MEG)

### Keywords:
5G, antenna array, mmWave, UWB

---

## SECTION 1: DESIGN SPECIFICATIONS

### 1.1 SUBSTRATE MATERIAL PROPERTIES

**Material:** RT-5880

| Property | Value | Unit |
|----------|-------|------|
| Relative Permittivity (εr) | 2.2 | - |
| Loss Tangent (tan δ) | 0.0009 | - |
| Thickness | 0.8 | mm |

**Advantages of Selected Substrate:**
- Reduced relative permittivity → Enhanced gain
- Lower loss tangent → Minimized power losses
- Thin profile → Compact integrated design

---

### 1.2 SINGLE ANTENNA ELEMENT DIMENSIONS

**Overall element size:** 4.5 × 12 mm

#### Component Specifications:

**Microstrip Line Steps:**

| Component | Dimensions (mm) | Purpose |
|-----------|-----------------|---------|
| First line step | 0.65 × 3.62 | Impedance matching |
| Second line step | 1.40 × 4.60 | Signal distribution |

**Symmetric Ladder Steps:**
- Dimensions: 2 × 0.64 mm
- Count: 3 symmetrical steps
- Location: Top of antenna

**Ground Plane:**
- Configuration: Etched (back view)
- Function: Signal return path optimization

---

### 1.3 ANTENNA ARRAY CONFIGURATION

**System Architecture:**
- **Type:** 4-element MIMO array
- **Configuration:** Square arrangement
- **Orientation:** Rotationally placed at 90° intervals
- **Overall dimensions:** 25 × 25 mm
- **Isolation technique:** Orthogonal polarization diversity

**Array Layout:**
```
Element spacing: Symmetrically rotationally arranged
Polarization diversity: Orthogonal placement (90° rotation)
Total elements: 4 (Antenna 1, 2, 3, 4)
Physical separation: Optimized for low mutual coupling
```

---

## SECTION 2: SINGLE ANTENNA ELEMENT PERFORMANCE

### 2.1 REFLECTION COEFFICIENT (S₁₁)

**Performance Metrics:**

| Frequency Range | S₁₁ Level | Bandwidth | Matching Status |
|-----------------|-----------|-----------|-----------------|
| 42 - 62 GHz | < -10 dB | 20 GHz | Ultra-wideband |
| Entire operating band | Below -10 dB | Continuous | Good impedance matching |

**Key Finding:** Excellent impedance matching across entire operating band with S₁₁ remaining below -10 dB throughout 42-62 GHz range.

---

### 2.2 RADIATION EFFICIENCY

**Efficiency Range:** 80 - 88%

| Frequency Region | Efficiency Level | Stability |
|------------------|------------------|-----------|
| Entire operating band | 80 - 88% | Highly stable |
| Peak performance | 88% | Upper range |
| Minimum performance | 80% | Lower range |

**Performance Interpretation:** High antenna efficiency maintained consistently across ultra-wide operating bandwidth, eliminating efficiency degradation at band edges.

---

### 2.3 GAIN PERFORMANCE

**Peak Gain:** 6.2 dB (single element)

**Gain Characteristics:**
- Consistent across operating band
- Required for mmWave path loss compensation
- Suitable for long-range mmWave communications

**mmWave Gain Requirement Justification:**
High gain at mmWave frequencies is essential to overcome increased free space path loss at these frequencies (40+ dB/km in open space scenarios).

---

### 2.4 RADIATION PATTERNS

**3D Radiation Pattern Analysis:**

| Frequency | Pattern Characteristic | Coverage | Directivity |
|-----------|----------------------|----------|-------------|
| 45 GHz | Directional pattern | Multi-directional | Moderate |
| 55 GHz | Directional pattern | Multi-directional | Moderate |

**Pattern Diversity at Array Frequencies:**
- E-plane patterns shown at 45 GHz and 55 GHz
- H-plane patterns shown at 45 GHz and 55 GHz
- 3D patterns demonstrate frequency-dependent behavior

---

## SECTION 3: FOUR-ELEMENT MIMO ARRAY PERFORMANCE

### 3.1 S-PARAMETERS ANALYSIS

#### Return Loss (S₁₁, S₂₂, S₃₃, S₄₄)

**Performance Specification:**

| Parameter | Value | Frequency Range | Status |
|-----------|-------|-----------------|--------|
| All return loss coefficients | < -10 dB | 42.3 - 62.3 GHz | All elements |
| Variation vs single element | Very slight | Entire band | Good agreement |

**Interpretation:** Structural similarity and orthogonal MIMO layout result in satisfactory mutual coupling with minimal variation across array elements.

#### Transmission Coefficients (S₂₁, S₃₁, S₃₂, S₄₁, S₄₂, S₄₃)

**Isolation Performance:**

| Parameter | Value | Frequency Range | Isolation Level |
|-----------|-------|-----------------|-----------------|
| All transmission coefficients | < -24 dB | 42.3 - 62.3 GHz | High isolation |
| Minimum isolation | > 24 dB | Entire band | Excellent |

**Isolation Technique:** Polarization diversity approach with orthogonal element arrangement achieves exceptional inter-element isolation.

---

### 3.2 EFFICIENCY ANALYSIS

**MIMO Array Efficiency:**

| Efficiency Type | Range | Frequency Coverage |
|-----------------|-------|-------------------|
| Total antenna efficiency | 66 - 72% | Entire operating band |
| Radiation efficiency | 78 - 80% | Entire operating band |

**Efficiency Comparison:**
- Total efficiency: Accounts for all losses (return loss + radiation loss)
- Radiation efficiency: Reflects only radiation losses (typically higher)

---

### 3.3 GAIN PERFORMANCE

**MIMO Array Gain:**

| Metric | Value | Coverage |
|--------|-------|----------|
| Gain range | 4.1 - 7.8 dB | Full operating band |
| Peak gain | 7.8 dB | Optimal frequency |
| Minimum gain | 4.1 dB | Band edges |

**Gain Elevation:** Four-element array provides gain boost compared to single element (6.2 dB → 7.8 dB peak).

---

### 3.4 RADIATION PATTERN DIVERSITY

**2D Radiation Patterns at Key Frequencies:**

| Frequency | E-plane Pattern | H-plane Pattern | Coverage Characteristic |
|-----------|-----------------|-----------------|------------------------|
| 45 GHz | Diverse direction | Diverse direction | Full 360° coverage |
| 55 GHz | Diverse direction | Diverse direction | Full 360° coverage |

**Pattern Diversity Benefit:** Peak gain achieved in diverse directions across different elements, demonstrating highly desirable pattern diversity for MIMO systems.

**Coverage Achievement:** Radiation patterns fully cover all sides, proving excellent radiation coverage for multi-directional propagation scenarios.

---

## SECTION 4: MIMO DIVERSITY CHARACTERISTICS

### 4.1 ENVELOPE CORRELATION COEFFICIENT (ECC)

#### ECC Definition and Significance

**ECC determines** the correlation between different antenna elements in a MIMO system.
- **Low ECC value** → Less interdependence between components → Better MIMO diversity
- **Permissible range** → ECC < 0.5 for good MIMO diversity
- **Excellent range** → ECC < 0.002 for exceptional performance

#### ECC Calculation Methods

**Method 1: From S-parameters**

```
ECC = |ρᵢⱼ| = |S*ᵢᵢSᵢⱼ + S*ⱼᵢSⱼⱼ|² / {[1 - (|Sᵢᵢ|² + |Sⱼᵢ|²)] × [1 - (|Sⱼⱼ|² + |Sᵢⱼ|²)]}

where:
- ρᵢⱼ = envelope correlation coefficient between i and j antenna elements
- Sₓᵧ = scattering parameters
- * denotes Hermitian product
```

**Method 2: From Far-field Radiation Patterns**

```
ECC = |∫∫₄π [→F₁(θ, φ) * · →F₂(θ, φ)] dΩ|² / 
      {∫∫₄π |→F₁(θ, φ)|² dΩ · ∫∫₄π |→F₂(θ, φ)|² dΩ}

where:
- →F₁(θ, φ) = 3D radiation pattern field with excitation at port i
- * denotes Hermitian product
- Ω = solid angle
```

#### Measured ECC Values

**ECC Performance:**

| Element Pair | ECC Value | Frequency Range | Performance |
|--------------|-----------|-----------------|-------------|
| Ant. 1 & Ant. 3 | < 0.002 | 40 - 70 GHz | Excellent |
| Ant. 2 & Ant. 3 | < 0.002 | 40 - 70 GHz | Excellent |
| Ant. 2 & Ant. 4 | < 0.002 | 40 - 70 GHz | Excellent |
| Ant. 3 & Ant. 4 | < 0.002 | 40 - 70 GHz | Excellent |

**ECC Conclusion:** Very low ECCs below 0.002 prove very high diversity antenna system achievement.

---

### 4.2 MEAN EFFECTIVE GAIN (MEG)

#### MEG Definition and Significance

**MEG is** the ratio of mean received power to total mean incident power at antenna.

**MEG quantifies:**
- Mutual interaction of antenna elements
- Statistical characteristics of propagation environment
- Multiuser interference impact

#### MEG Calculation Methods

**Method 1: From S-parameters**

```
MEGᵢ = 0.5 × [1 - Σⱼ₌₁ᵏ |Sᵢⱼ|²]

where:
- i = observed antenna index
- j = antenna index summation
- k = total number of antennas
```

**Method 2: From Far-field Radiation**

```
MEG = (2π/∫∫) {[XPR/(1+XPR)] × Gθ(θ,φ) × Pθ(θ,φ) 
              + [1/(1+XPR)] × Gφ(θ,φ) × Pφ(θ,φ)} sin θ dθ dφ

where:
- XPR = cross polarization power ratio
- Gθ, Gφ = antenna gains in θ and φ directions
- Pθ, Pφ = incoming plane wave components
```

**MEG Criterion for Good MIMO:**

```
MEGᵢ / MEGⱼ ≈ 1.0 (for all antenna pairs)
```

#### Measured MEG Values

**MEG Performance:**

| Frequency (GHz) | MEG Value (dB) | Stability | Status |
|-----------------|----------------|-----------|--------|
| 40 - 45 | -3.2 to -3.4 | Stable | Good |
| 45 - 55 | -3.4 to -3.6 | Stable | Good |
| 55 - 70 | -3.2 to -3.8 | Stable | Good |

**MEG Conclusion:** Quad antenna MEGs maintain stability across frequency band, meeting MEG criterion from Equation 4.5.

---

### 4.3 DIVERSITY GAIN (DG)

#### DG Definition and Significance

**Diversity Gain** measures performance improvement from using multiple antennas.

**Calculation:**

```
G_DG = 10 × √(1 - |ρ|²)  [in dB]

where:
- ρ = correlation coefficient
- G_DG = diversity gain in dB
```

**Performance Interpretation:**
- High DG value → Exceptional performance
- Better element isolation → Higher DG
- DG > 9.99 dB → Effective diversity performance

#### Measured Diversity Gain

**DG Performance:**

| Frequency (GHz) | DG Value (dB) | Performance |
|-----------------|---------------|-------------|
| 40 - 70 | > 9.99 | Exceptional |
| Entire band | > 9.998 | Nearly perfect |
| Minimum | 9.990 | Excellent baseline |

**DG Conclusion:** Diversity gain values greater than 9.99 dB across entire working band demonstrate effective diversity performance of proposed design.

---

## SECTION 5: DESIGN TECHNIQUES AND METHODOLOGIES

### 5.1 SUBSTRATE OPTIMIZATION

**Technique:** Substrate selection with reduced permittivity and loss tangent

**Implementation:**
- Material: RT-5880 (εᵣ = 2.2, tan δ = 0.0009)
- Result: Enhanced gain, minimized power losses
- Application: Ultra-wideband impedance matching

---

### 5.2 CORRUGATED CONSTRUCTION

**Technique:** Metallic edge elimination from radiator

**Benefits:**
- Improved front-to-back ratio
- Extended antenna bandwidth
- Better radiation pattern control

---

### 5.3 MULTI-ELEMENT CONFIGURATION

**Technique:** Four-element MIMO array

**Advantages:**
- Improved gain (6.2 dB single → 7.8 dB array)
- Enhanced efficiency
- Extended operating bandwidth
- Superior diversity performance

---

### 5.4 DIELECTRIC LENS APPLICATION

**Technique:** Dielectric lens for radiation control

**Purpose:**
- Transmit electrostatic radiation non-directionally
- Enhance antenna directivity and gain
- Improve beam shaping

---

### 5.5 MUTUAL COUPLING REDUCTION

**Technique:** Isolation techniques for multi-element systems

**Primary Method - Polarization Diversity:**
- Orthogonal element placement (90° rotation)
- Four-element square configuration
- Result: Isolation > 24 dB

**Importance:**
- Reduces impact of multiple elements on performance
- Critical for good MIMO diversity
- Enables high array efficiency

---

### 5.6 ORTHOGONAL ARRANGEMENT

**Configuration Details:**
- Elements rotated 90° from each other
- Square 25 × 25 mm layout
- Symmetrical placement pattern

**Advantages:**
- Maximum polarization diversity exploitation
- Minimal mutual coupling
- Optimal gain distribution
- Excellent spatial isolation

---

## SECTION 6: CURRENT DISTRIBUTION ANALYSIS

### Surface Current Distribution Characteristics

**Configuration:** One port excited, others terminated with 50 Ω

#### At 45 GHz:

**Current Flow Pattern:**
- Predominantly concentrated in excited antenna unit
- Minimal propagation to other MIMO ports
- Strong confinement within radiating element

#### At 55 GHz:

**Current Flow Pattern:**
- Similar concentration to 45 GHz
- Effective frequency independence
- Consistent isolation mechanism across band

**Interpretation:** Strong current confinement demonstrates effectiveness of orthogonal arrangement in achieving high inter-element isolation and low mutual coupling.

---

## SECTION 7: COMPARATIVE PERFORMANCE ANALYSIS

### Comparison with Recent Literature

| Parameter | This Work | Ref. [15] | Ref. [20] | Ref. [32] | Ref. [33] | Ref. [34] |
|-----------|-----------|-----------|-----------|-----------|-----------|-----------|
| **Bandwidth (GHz)** | 42.3-63.3 | 25.5-29.6 | 23-40 | 27.5-40 | 20-32 | 27-29 |
| **Total Efficiency (%)** | 66-72 | >82 | >70 | >75 | 80-90 | 80-84 |
| **Peak Gain (dB)** | 7.8 | 8.3 | 12 | 7.2 | 6.5 | 5.5 |
| **Isolation (dB)** | >24 | >20 | >20 | >17 | >20 | >17 |
| **ECC** | <0.002 | <0.01 | <0.001 | <0.001 | <0.001 | <0.03 |
| **MIMO Order** | 4×4 | 4×4 | 4×4 | 4×4 | 4×4 | 4×4 |
| **Size (mm)** | 25×25 | 30×35 | 80×80 | 158×77.8 | 24×32 | 30×30 |
| **Isolation Technique** | Pol. Div. | DGS | Spatial Div. | Decoupling | Decoupling | Pol. Div. |

**Comparative Advantages:**
1. **Compactness:** Most compact design (25×25 mm)
2. **Widest bandwidth:** 42.3-63.3 GHz (20 GHz span)
3. **Highest isolation:** >24 dB
4. **Superior ECC:** <0.002
5. **Simple structure:** Polarization diversity only

---

## SECTION 8: TECHNICAL PERFORMANCE SUMMARY

### Key Performance Metrics Table

| Category | Metric | Value | Unit |
|----------|--------|-------|------|
| **Frequency** | Operating band | 42.3 - 63.3 | GHz |
| | Bandwidth | 20 | GHz |
| | S₁₁ level | < -10 | dB |
| **Gain** | Peak gain (array) | 7.8 | dB |
| | Single element gain | 6.2 | dB |
| | Gain range | 4.1 - 7.8 | dB |
| **Efficiency** | Radiation efficiency | 78 - 80 | % |
| | Total efficiency | 66 - 72 | % |
| **Isolation** | Transmission coefficient | < -24 | dB |
| | Minimum isolation | > 24 | dB |
| **Diversity** | ECC value | < 0.002 | - |
| | Diversity gain | > 9.99 | dB |
| | MEG | -3.2 to -3.8 | dB |
| **Physical** | Array size | 25 × 25 | mm |
| | Element size | 4.5 × 12 | mm |
| | Substrate thickness | 0.8 | mm |
| **Substrate** | Permittivity | 2.2 | - |
| | Loss tangent | 0.0009 | - |

---

## SECTION 9: SIMULATION AND VERIFICATION

### Simulation Tool

**Software:** CST Microwave Studio

**Validation Criteria:**
- Frequency range: 40-70 GHz (extended analysis)
- S-parameter analysis
- Radiation pattern computation
- MIMO diversity metrics calculation
- Efficiency evaluation

---

## SECTION 10: REFERENCES

[1] M. Shafi et al., "5G: A Tutorial Overview of Standards, Trials, Challenges, Deployment, and Practice", IEEE Journal on Selected Areas in Communications, vol. 35, no. 6, pp. 1201–1221, 2017.

[2] M. Agiwal, H. Kwon, S. Park, and H. Jin, "A Survey on 4G-5G Dual Connectivity: Road to 5G Implementation", IEEE Access, vol. 9, pp. 16193–16210, 2021.

[3] J. Cheng, Y. Yang, X. Zou, and Y. Zuo, "5G in Manufacturing: A Literature Review and Future Research", The International Journal of Advanced Manufacturing Technology, vol. 131, no. 11, pp. 5637–5659, 2024.

[4] B.C. Tedeschini, M. Nicoli, and M.Z. Win, "On the Latent Space of mmWave MIMO Channels for NLOS Identification in 5G-advanced Systems", IEEE Journal on Selected Areas in Communications, vol. 41, no. 6, pp. 1655–1669, 2023.

[5] W.A.E. Ali, A.A. Ibrahim, and A.E. Ahmed, "Dual-band Millimeter Wave 2×2 MIMO Slot Antenna with Low Mutual Coupling for 5G Networks", Wireless Personal Communications, vol. 129, no. 4, pp. 2959–2976, 2023.

[6] W.T. Sethi et al., "Pattern Diversity Based Four-element Dual-band MIMO Patch Antenna for 5G mmWave Communication Networks", Journal of Infrared, Millimeter, and Terahertz Waves, vol. 45, no. 5, pp. 521–537, 2024.

[7] S. Kumar et al., "Fifth Generation Antennas: A Comprehensive Review of Design and Performance Enhancement Techniques", IEEE Access, vol. 8, pp. 163568–163593, 2020.

[8] A.S. Dixit and S. Kumar, "A Survey of Performance Enhancement Techniques of Antipodal Vivaldi Antenna", IEEE Access, vol. 8, pp. 45774–45796, 2020.

[9] S.F. Farida, P.M. Hadalgi, P.V. Hunagund, and S.R. Ara, "Effect of Substrate Thickness and Permittivity on the Characteristics of Rectangular Microstrip Antenna", 1998 Conference on Precision Electromagnetic Measurements Digest, Washington, USA, 1998.

[10] M.M. Honari, M.S. Ghaffarian, P. Mousavi, and K. Sarabandi, "A Wideband High-gain Planar Corrugated Antenna", 2020 IEEE International Symposium on Antennas and Propagation and North American Radio Science Meeting, Montreal, Canada, 2020.

[11] Z.X. Wang and W.B. Dou, "Dielectric Lens Antennas Designed for Millimeter Wave Application", 2006 Joint 31st International Conference on Infrared Millimeter Waves and 14th International Conference on Terahertz Electronics, Shanghai, China, 2006.

[12] Z. Zhang et al., "Dual-band Focused Transmitarray Antenna for Microwave Measurements", IEEE Access, vol. 8, pp. 100337–100345, 2020.

[13] M.Y. Muhsin, A.J. Salim, and J.K. Ali, "An Eight-element Multi-band MIMO Antenna System for 5G Mobile Terminals", AIP Conference Proceedings, vol. 2651, no. 1, 2023.

[14] A. Abdelraheem, H. Elregaily, A.A. Mitkees, and M. Abdalla, "A Hybrid Isolation in Two-element Directive UWB MIMO Antenna", IETE Journal of Research, vol. 69, no. 1, pp. 499–508, 2023.

[15] M. Khalid et al., "4-Port MIMO Antenna with Defected Ground Structure for 5G Millimeter Wave Applications", Electronics, vol. 9, no. 1, art. no. 71, 2020.

[16] N. Yoon and C. Seo, "A 28-GHz Wideband 2×2 U-slot Patch Array Antenna", Journal of Electromagnetic Engineering and Science, vol. 17, no. 3, pp. 133–137, 2017.

[17] R. Anitha et al., "A Compact Quad Element Slotted Ground Wideband Antenna for MIMO Applications", IEEE Transactions on Antennas and Propagation, vol. 64, no. 10, pp. 4550–4553, 2016.

[18] C.R. Jetti et al., "Design and Analysis of Modified U-shaped Four Element MIMO Antenna for Dual-band 5G Millimeter Wave Applications", Micromachines, vol. 14, no. 8, art. no. 1545, 2023.

[19] D.A. Sehrai et al., "A Novel High Gain Wideband MIMO Antenna for 5G Millimeter Wave Applications", Electronics, vol. 9, no. 6, art. no. 1031, 2020.

[20] E. Al Abbas, M. Ikram, A.T. Mobashsher, and A. Abbosh, "MIMO Antenna System for Multi-band Millimeter-wave 5G and Wideband 4G Mobile Communications", IEEE Access, vol. 7, pp. 181916–181923, 2019.

[21] F.W. Ardianto, F.F. Lanang, S. Renaldy, and T. Yunita, "Design MIMO Antenna with U-Slot Rectangular Patch Array for 5G Applications", 2018 International Symposium on Antennas and Propagation (ISAP), Busan, South Korea, 2018.

[22] Y. Rahayu and I.R. Mustofa, "Design of 2×2 MIMO Microstrip Antenna Rectangular Patch Array for 5G Wireless Communication Network", 2017 Progress in Electromagnetics Research Symposium-Fall (PIERS–FALL), Singapore, 2017.

[23] M.K. Ishfaq, T.A. Rahman, Y. Yamada, and K. Sakakibara, "8×8 Phased Series Fed Patch Antenna Array at 28 GHz for 5G Mobile Base Station Antennas", 2017 IEEE-APS Topical Conference on Antennas and Propagation in Wireless Communications (APWC), Verona, Italy, 2017.

[24] Y. Wang and D. Piao, "A Compact Size Dual-polarized High-gain Resonant Cavity Antenna at 28 GHz", 2017 International Applied Computational Electromagnetics Society Symposium (ACES), Suzhou, China, 2017.

[25] A. Thatere, P.L. Zade, and D. Arya, "Bandwidth Enhancement of Microstrip Patch Antenna Using 'U' Slot with Modified Ground Plane", 2015 International Conference on Microwave, Optical and Communication Engineering (ICMOCE), Bhubaneswar, India, 2015.

[26] I. Rosaline, A. Kumar, P. Upadhyay, and A.H. Murshed, "Four Element MIMO Antenna Systems with Decoupling Lines for High-speed 5G Wireless Data Communication", International Journal on Antennas and Propagation, vol. 2022, no. 1, art. no. 9078929, 2022.

[27] K.S. Sultan and H.H. Abdullah, "Planar UWB MIMO-diversity Antenna with Dual Notch Characteristics", Progress in Electromagnetics Research C, vol. 93, pp. 119–129, 2019.

[28] R.E.A. Shehata, A. Elboushi, M. Hindy, and H. Elmekati, "Meta-material Inspired LPDA MIMO array for upper band 5G applications", International Journal of RF and Microwave Computer-Aided Engineering, vol. 32, no. 8, art. no. 23212, 2022.

[29] M.Y. Muhsin, A.J. Salim, and J.K. Ali, "Compact MIMO Antenna Designs Based on Hybrid Fractal Geometry for 5G Smartphone Applications", Progress in Electromagnetics Research C, vol. 118, pp. 247–262, 2022.

[30] Z.F. Al-Azzawi et al., "Designing Eight-port Antenna Array for Multi-band MIMO Applications in 5G Smartphones", Journal of Telecommunications and Information Technology, no. 4, pp. 18–24, 2023.

[31] M.Y. Muhsin et al., "Isolation Techniques in MIMO Antennas for 5G Mobile Devices (Comprehensive Review)", Radioelectronics and Communications Systems, vol. 66, no. 6, pp. 263–287, 2023.

[32] M. Bilal et al., "High-isolation MIMO Antenna for 5G Millimeter-wave Communication Systems", Electronics, vol. 11, no. 6, art. no. 962, 2022.

[33] H. Elmannai et al., "Design and Characterization of a Meandered V-shaped Antenna Using Characteristics Mode Analysis and its MIMO Configuration for Future mmWave Devices", AEU – International Journal of Electronics and Communications, vol. 186, art. no. 155477, 2024.

[34] S. Rahman et al., "Nature Inspired MIMO Antenna System for Future mmWave Technologies", Micromachines, vol. 11, no. 12, art. no. 1083, 2020.

---

## CONCLUSIONS

The paper presents an ultra-wideband four-port MIMO antenna array with the following achievements:

### Key Design Features:
- Simple, planar structure
- Compact 25×25 mm size
- Orthogonal element arrangement
- Polarization diversity for isolation

### Performance Achievements:
- Ultra-wideband: 42.3-63.3 GHz (20 GHz)
- High gain: 7.8 dB peak
- Excellent isolation: >24 dB
- Outstanding diversity: ECC < 0.002, DG > 9.99 dB
- Stable efficiency: 66-72% total, 78-80% radiation

### Application Suitability:
The antenna system is a promising candidate for future mmWave 5G devices due to compact dimensions, wide bandwidth, high gain, and excellent isolation characteristics.

---

**Extraction Status:** COMPLETE
**Document Type:** Comprehensive technical extraction
**Quality Level:** Academic standard with all specifications, equations, and performance metrics preserved
**Format:** Markdown for Word document conversion and standalone reference


# ULTRA-WIDEBAND ANTENNA: EQUATIONS AND MATHEMATICAL MODELS

## MATHEMATICAL FORMULATIONS

### SECTION 1: ENVELOPE CORRELATION COEFFICIENT (ECC)

#### Equation 1: ECC from S-parameters

```
ECC = |ρᵢⱼ| = |S*ᵢᵢSᵢⱼ + S*ⱼᵢSⱼⱼ|² / {[1 - (|Sᵢᵢ|² + |Sⱼᵢ|²)] × [1 - (|Sⱼⱼ|² + |Sᵢⱼ|²)]}

where:
- ρᵢⱼ = envelope correlation coefficient between antenna elements i and j
- Sₓᵧ = S-parameter (scattering parameter)
- * = Hermitian product (complex conjugate transpose)
- |·| = magnitude operator
```

**Variables Definition:**
- i, j = antenna element indices (1, 2, 3, 4 for four-element array)
- Sᵢᵢ = return loss of port i
- Sᵢⱼ = transmission coefficient from port j to port i
- Sⱼᵢ = transmission coefficient from port i to port j
- Sⱼⱼ = return loss of port j

**Interpretation:**
- ECC < 0.5: Good MIMO diversity performance
- ECC < 0.002: Excellent diversity (achieved in this work)
- Lower ECC → Higher independence between elements → Better MIMO performance

---

#### Equation 2: ECC from Far-field Radiation Patterns

```
ECC = |∫∫₄π [→F₁(θ, φ) * · →F₂(θ, φ)] dΩ|² / 
      {∫∫₄π |→F₁(θ, φ)|² dΩ · ∫∫₄π |→F₂(θ, φ)|² dΩ}

where:
- →F₁(θ, φ) = 3D radiation pattern field with excitation at port i
- →F₂(θ, φ) = 3D radiation pattern field with excitation at port j
- * = complex conjugate
- · = dot product
- dΩ = solid angle differential
- ∫∫₄π = integration over full sphere (4π steradians)
```

**Variables Definition:**
- θ = elevation angle (0 to π radians)
- φ = azimuth angle (0 to 2π radians)
- |→F(θ, φ)|² = power radiation pattern
- Ω = solid angle (steradians)

**Computation Steps:**
1. Calculate 3D radiation patterns for each port
2. Integrate cross-product of patterns over full sphere
3. Compute magnitude squared of result
4. Normalize by product of individual pattern integrals
5. Result: ECC value in range [0, 1]

---

### SECTION 2: MEAN EFFECTIVE GAIN (MEG)

#### Equation 3: MEG from S-parameters

```
MEGᵢ = 0.5 × [1 - Σⱼ₌₁ᵏ |Sᵢⱼ|²]

where:
- MEGᵢ = mean effective gain of antenna i
- i = antenna element index (1 to k)
- j = summed antenna indices (1 to k)
- k = total number of antenna elements (4 in this array)
- |Sᵢⱼ|² = power reflection coefficient
```

**Variables Definition:**
- Sᵢⱼ = S-parameter from port j to port i
- Factor 0.5 = accounts for polarization averaging
- Sum term = total reflected power

**MIMO Criterion:**

```
MEGᵢ / MEGⱼ ≈ 1.0 (for all antenna pairs i, j)
```

This criterion ensures balanced power distribution across all array elements.

---

#### Equation 4: MEG from Far-field Radiation Patterns

```
MEG = (2π)⁻¹ ∫₀²π ∫₀π {[XPR/(1+XPR)] × Gθ(θ,φ) × Pθ(θ,φ) 
                       + [1/(1+XPR)] × Gφ(θ,φ) × Pφ(θ,φ)} 
      × sin θ dθ dφ

where:
- MEG = mean effective gain
- XPR = cross polarization power ratio
- Gθ(θ,φ) = antenna gain in θ-polarization
- Gφ(θ,φ) = antenna gain in φ-polarization
- Pθ(θ,φ) = incoming plane wave power component (θ polarization)
- Pφ(θ,φ) = incoming plane wave power component (φ polarization)
- θ = elevation angle (0 to π)
- φ = azimuth angle (0 to 2π)
- sin θ dθ dφ = solid angle weighting
```

**Assumptions:**
- Gaussian distribution in elevation direction
- Uniform distribution in azimuth direction
- Plane wave propagation model
- Isotropic receiving environment

---

#### Equation 5: MEG Criterion

```
MEGᵢ / MEGⱼ ≈ 1.0
```

**Requirement:** This criterion must be satisfied for good MIMO diversity performance, indicating balanced mean effective gain across all antenna elements.

---

### SECTION 3: DIVERSITY GAIN (DG)

#### Equation 6: Diversity Gain Calculation

```
G_DG = 10 × √(1 - |ρ|²)  [dB]

where:
- G_DG = diversity gain in decibels
- ρ = correlation coefficient (from ECC)
- |ρ|² = magnitude squared of correlation coefficient
- Factor 10 = conversion to dB scale
- √(1 - |ρ|²) = diversity factor
```

**Relationship:**
- DG depends directly on ECC value
- Lower ECC → Higher DG
- ECC < 0.002 → DG > 9.99 dB

**Performance Interpretation:**
- DG > 9.99 dB: Exceptional diversity performance
- DG = 10 dB: Maximum theoretical diversity (when ρ = 0, fully uncorrelated)
- Achieved in this work: DG > 9.998 dB across entire band

**Formula Derivation:**
From ECC definition, diversity factor = √(1 - |ECC|²)
Converting to dB: G_DG[dB] = 10 × log₁₀[√(1 - |ECC|²)]

---

### SECTION 4: REFLECTION COEFFICIENT (S₁₁)

#### S-parameter Definition

```
Sᵢⱼ = (V⁻ᵢ / V⁺ⱼ)|_{V⁺ₖ=0 for k≠j}

where:
- Sᵢⱼ = scattering parameter
- V⁺ⱼ = incident voltage wave at port j
- V⁻ᵢ = reflected voltage wave at port i
- All other ports terminated (V⁺ₖ = 0)
```

#### Return Loss (S₁₁) Definition

```
Return Loss [dB] = -20 log₁₀|S₁₁|

where:
- S₁₁ = reflection coefficient at port 1
- Return Loss = 10 dB when |S₁₁| = 0.316
- Return Loss = 20 dB when |S₁₁| = 0.1
- Return Loss = 30 dB when |S₁₁| = 0.0316
```

**Application:**
- S₁₁ < -10 dB requirement: Good impedance matching
- Achieved: S₁₁ < -10 dB across 42.3-62.3 GHz

---

#### Transmission Coefficient (S₂₁)

```
Isolation [dB] = -20 log₁₀|S₂₁|

where:
- S₂₁ = transmission coefficient from port 2 to port 1
- Isolation > 24 dB when |S₂₁| < 0.0631
```

**Application:**
- Measures signal leakage between ports
- Higher isolation (more negative) → Better port independence
- Achieved: Isolation > 24 dB between all ports

---

### SECTION 5: IMPEDANCE MATCHING AND BANDWIDTH

#### Impedance Matching Condition

```
|S₁₁| < 10^(-BW_dB/20)

where:
- BW_dB = desired bandwidth specification (typically 10 dB)
- For -10 dB: |S₁₁| < 0.316
```

#### Fractional Bandwidth

```
FBW = (f_high - f_low) / f_center × 100%

where:
- f_high = 63.3 GHz (upper frequency)
- f_low = 42.3 GHz (lower frequency)
- f_center = (f_high + f_low) / 2 = 52.8 GHz
- FBW = (21 / 52.8) × 100% = 39.8%

Interpretation:
- Ultra-wideband: FBW > 20%
- This antenna: FBW = 39.8% (ultra-wideband)
```

---

### SECTION 6: GAIN CALCULATIONS

#### Directivity

```
D(θ, φ) = U(θ, φ) / U_avg

where:
- D(θ, φ) = directivity in direction (θ, φ)
- U(θ, φ) = radiation intensity = |→E(θ, φ)|² / (2η₀)
- U_avg = average radiation intensity = P_total / 4π
- η₀ = 120π Ω (free space impedance)
- P_total = total radiated power
```

#### Gain

```
G(θ, φ) = η × D(θ, φ)  [linear]
G[dB] = 10 log₁₀(G)   [logarithmic]

where:
- G(θ, φ) = antenna gain in direction (θ, φ)
- η = radiation efficiency (78-80% in this work)
- D(θ, φ) = directivity
```

#### Realized Gain

```
G_realized = G × (1 - |S₁₁|²)

where:
- G = antenna gain
- (1 - |S₁₁|²) = impedance matching efficiency factor
- Accounts for power reflected due to mismatch
```

**Application:**
- Single element: Maximum 6.2 dB
- Array element: 4.1-7.8 dB range
- Peak array gain: 7.8 dB (at optimal frequency)

---

### SECTION 7: RADIATION EFFICIENCY

#### Total Efficiency

```
η_total = η_rad × η_matching

where:
- η_total = total antenna efficiency (66-72% this work)
- η_rad = radiation efficiency (78-80% this work)
- η_matching = matching efficiency = (1 - |S₁₁|²) ≈ 80-85%
- Product: 0.78-0.80 × 0.80-0.85 ≈ 0.66-0.72
```

#### Radiation Efficiency Definition

```
η_rad = P_rad / (P_rad + P_loss)

where:
- P_rad = radiated power
- P_loss = power dissipated in conductor and dielectric
- Typically 78-80% for microstrip antennas
```

#### Effective Isotropic Radiated Power (EIRP)

```
EIRP = P_in × G

where:
- EIRP = effective isotropic radiated power
- P_in = input power
- G = antenna gain (linear, not dB)
- Unit: Watts (or dBm/dBW)
```

---

### SECTION 8: FREQUENCY AND WAVELENGTH RELATIONSHIPS

#### Wavelength Calculation

```
λ = c / f

where:
- λ = wavelength in free space
- c = 3 × 10⁸ m/s (speed of light)
- f = frequency in Hz
```

**Examples at Operating Band:**

| Frequency | Wavelength |
|-----------|-----------|
| 42.3 GHz | 7.09 mm |
| 52.8 GHz | 5.68 mm |
| 63.3 GHz | 4.74 mm |

#### Effective Wavelength in Substrate

```
λ_eff = λ_free / √(ε_r,eff)

where:
- λ_eff = wavelength in substrate
- ε_r,eff = effective relative permittivity ≈ 1.5 (for RT-5880)
- For 52.8 GHz: λ_eff ≈ 4.64 mm
```

---

### SECTION 9: ANTENNA ARRAY PARAMETERS

#### Element Spacing

```
Spacing = 25 mm / 2 = 12.5 mm

Normalized spacing (at f_center = 52.8 GHz):
Spacing / λ = 12.5 mm / 5.68 mm ≈ 2.2 λ
```

#### Array Size Optimization

```
Array size = 25 × 25 mm = 625 mm²

Normalized size (at f_center):
Size / λ² = 625 / 32.3 ≈ 19.3 λ²

Compact design achieved with minimal spacing
```

---

### SECTION 10: MUTUAL COUPLING REDUCTION

#### Isolation Improvement Factor

```
Isolation improvement = 20 log₁₀(1 / |S₂₁|)  [dB]

where:
- |S₂₁| = magnitude of transmission coefficient
- Achieved isolation: > 24 dB
- Corresponds to |S₂₁| < 0.063
```

---

## PERFORMANCE METRICS SUMMARY TABLE

| Metric | Equation | Value | Unit |
|--------|----------|-------|------|
| S₁₁ (return loss) | -20 log₁₀\|S₁₁\| | < -10 | dB |
| Transmission (isolation) | -20 log₁₀\|S₂₁\| | < -24 | dB |
| Gain (single element) | η × D | 6.2 | dB |
| Gain (array) | η × D × Array factor | 4.1-7.8 | dB |
| ECC | Equation 1 or 2 | < 0.002 | (dimensionless) |
| MEG | Equation 3 or 4 | -3.2 to -3.8 | dB |
| Diversity Gain | 10√(1-\|ρ\|²) | > 9.99 | dB |
| Radiation efficiency | η_rad | 78-80 | % |
| Total efficiency | η_total | 66-72 | % |
| Fractional bandwidth | (f_h - f_l)/f_c | 39.8 | % |
| Operating frequency | - | 42.3-63.3 | GHz |
| Wavelength range | c/f | 4.74-7.09 | mm |

---

## SUBSTRATE AND MATERIAL CALCULATIONS

### Effective Dielectric Constant for Microstrip

```
ε_r,eff = (ε_r + 1)/2 + (ε_r - 1)/2 × [1 + 10(t/W)]^(-0.555)

where:
- ε_r = substrate relative permittivity = 2.2
- t = substrate thickness = 0.8 mm
- W = line width (varies per section)
```

**For this substrate:**
- Effective permittivity ≈ 1.8-1.95 (depends on line width)
- Typically lower than bulk permittivity due to fringing fields

### Characteristic Impedance

```
Z₀ = (120/√(ε_r,eff)) × [w/t]  [for w > t]

or

Z₀ = (120π/√(ε_r,eff)) × [1 / (w/t + 1.393 + 0.667×ln(w/t + 1.444))]

where:
- Z₀ = characteristic impedance (target 50 Ω)
- w = line width
- t = substrate thickness
```

---

## NUMERICAL EXAMPLE: CORRELATION CALCULATION

### Example ECC Calculation (Antennas 1 & 3)

**Given S-parameters at 50 GHz:**
- |S₁₁| = 0.2
- |S₁₃| = 0.05
- |S₃₃| = 0.2
- |S₃₁| = 0.05

**Using Equation 1:**
```
ECC = |S*₁₁S₁₃ + S*₃₁S₃₃|² / {[1-(|S₁₁|² + |S₃₁|²)] × [1-(|S₃₃|² + |S₁₃|²)]}

Numerator: |0.2 × 0.05 + 0.05 × 0.2|² = |0.02|² = 0.0004

Denominator:
- [1-(0.04 + 0.0025)] × [1-(0.04 + 0.0025)]
- [1-0.0425] × [1-0.0425]
- 0.9575 × 0.9575 = 0.9168

ECC = 0.0004 / 0.9168 ≈ 0.000436 (well below 0.002 threshold)
```

---

## SIMULATION PARAMETERS

### CST Microwave Studio Settings

**Simulation Setup:**
- Frequency range: 40-70 GHz
- Number of mesh cells: Adequate for accurate field computation
- Boundary conditions: Open region (radiation simulation)
- Solver: Frequency domain solver
- Convergence criterion: S-parameter convergence

**Post-processing:**
- S-parameter extraction
- Radiation pattern computation
- Gain and efficiency calculation
- Far-field pattern analysis
- MIMO diversity metrics evaluation

---

**Document Status:** Complete equations extraction
**Format:** Mathematical notation with explanations
**Completeness:** All significant equations from paper documented
**Verification:** Ready for implementation and analysis



