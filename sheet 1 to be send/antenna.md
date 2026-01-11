# Antenna Research Directions for 6G - Extracted Content

## Document Information

**Paper Title:** Antenna Research Directions for 6G: A brief overview through sampling literature

**Authors:** Thomas O. Olwal, Peter Nnabugwu Chuku (Tshwane University of Technology, Pretoria, South Africa)
Albert A. Lysko (NextGen Enterprises and Institutions, CSIR, Pretoria, South Africa)

**Conference:** 2021 7th International Conference on Advanced Computing and Communication Systems (ICACCS)

---

## Equations and Mathematical Models

### Link Budget Equation

The fundamental link balance equation is expressed as:

$$P_{RX} = P_{TX} - L_C + G_{TX} - L_P + G_{RX}$$

Where:
- $P_{TX}$ = transmit power (dBm)
- $L_C$ = cable losses (dB)
- $G_{TX}$ = transmit antenna gain (dBi)
- $L_P$ = propagation attenuation/loss (dB)
- $G_{RX}$ = receive antenna gain (dBi)

### Shannon's Theorem and Capacity Equation

$$C = B \log_2(1 + \text{SINR})$$

Where:
- $C$ = capacity (b/s)
- $B$ = channel bandwidth (Hz)
- SINR = signal-to-interference-and-noise ratio

### Thermal Noise Power Calculation

$$N = kTB$$

Where:
- $k$ = Boltzmann's constant ($1.38 \times 10^{-23}$ J/K)
- $T$ = temperature (K)
- $B$ = system bandwidth (Hz)

### Signal-to-Interference-and-Noise Ratio

$$\text{SINR} = \frac{S}{I + N}$$

Where:
- $S$ = signal power
- $I$ = interference power (W)
- $N$ = noise power

### Beamforming Gain Definition

Beamforming is quantified as the ability achieved by Smart Antennas (SAs) to increase the range and capacity of a transmitted signal, resulting in an improved SINR characteristic.

---

## Technical Specifications and Antenna Designs

### 1. Microstrip Linear Antenna Array for 5G

**Design Overview:**
- **Number of Elements:** 16 rectangular patch elements
- **Configuration:** Linear formation
- **Operating Frequency:** 28 GHz
- **Substrate Material:** Low-loss RT/Duroid 5880
- **Dielectric Constant:** 2.2
- **Substrate Thickness:** 0.381 mm
- **Feeding Mechanism:** Gap-coupled feeder (single element)

**Structural Features:**
- Defected Ground Structure (DGS) implemented as rectangular slots to reduce mutual coupling between adjacent elements
- Design optimization for 5G telecommunications

**Performance Metrics:**
- **10-dB Bandwidth:** Exceeds 2 GHz
- **Maximum Gain:** 17.4 dBi at 28.4 GHz
- **Design Compliance:** Fulfills typical 5G system requirements including high radiation efficiency, high gain, and sufficient bandwidth

**Simulation Tool:** CST Microwave Studio

---

### 2. Circularly Polarized Loop-Type Ground Radiation Antenna for IoT Applications

**Design Specifications:**
- **Ground Mode Tuning (GMT) Structure:** Comprises an inductor and a metallic strip installed at the ground plane's edge
- **Operating Frequency Range:** 2.4-2.48 GHz
- **Polarization:** Left-hand circularly polarized (LHCP) waves in one direction; reversely polarized waves in the opposite direction
- **Phase Shift Design:** 90° phase shift between two ground modes

**Performance Metrics:**
- **Bandwidth at -6 dB:** 150 MHz
- **Axial Ratio (AR) Bandwidth at 3 dB:** 130 MHz

**Key Characteristics:** The antenna excites 2 equal magnitude orthogonal modes at the ground plane.

---

### 3. Pattern-Reconfigurable Slot Antenna for IoT (2.4 GHz)

**Design Capabilities:**
- **Radiation Patterns:** Provides 3 evenly-separated directional radiation patterns plus 1 omnidirectional radiation pattern
- **Operating Frequency:** 2.4 GHz
- **Application:** Suitable for integration in IoT base solutions
- **Performance Benefits:** Improves link range and reduces packet collisions

---

### 4. Compact Double Folded Loop (DFL) Antenna for Metal-Proximity IoT Applications

**Design Specifications:**
- **Antenna Type:** Double Folded Loop (DFL) antenna
- **Operating Frequency Band:** 2.4 GHz
- **Connection Terminal Location:** λ/4 wavelength from the feeding point
- **Terminal Connection:** Between the inner and outer loop of the antenna
- **Substrate Integration:** Dielectric substrate with through-holes for antenna bending to create compact design
- **Operational Capability:** Can operate effectively even when metal is in close proximity, regardless of position

**Performance Advantages:**
- **Radiation Efficiency Gain:** Exceeds 6 dB in signal strength when compared to λ/2-wavelength dipole close to metal

---

### 5. Single-Substrate Planar Multi-Band 5-Element MIMO Antenna for IoT

**Design Structure:**
- **Number of Elements:** 5-element MIMO configuration on single substrate
- **Compact Design Component:** 2-element folded meandered MIMO antenna
- **Additional Components:** 2-element MIMO antennas at specified frequency bands

**Multi-Band Operating Frequencies:**
- **LTE Sub-GHz Band:** 754-971 MHz
- **RFID/LTE Band 1:** 1.65-1.83 GHz
- **RFID/LTE Band 2:** 2.4-3.66 GHz
- **WLAN/LTE Band:** 5.1-5.6 GHz

**Spectrum Sensing Capabilities:**
- **Wideband Antenna Coverage:** 0.668-1.94 GHz and 3-4.6 GHz frequency ranges
- **Ground Plane Integration:** Sensing antenna functions as ground plane for MIMO elements

---

## Design Techniques, Configurations, and Methodologies

### 1. Beamforming Techniques

#### Analog vs. Digital vs. Hybrid Beamforming

**Digital Beamforming:**
- **Configuration:** N RF chains + N antenna elements + Digital Signal Processing (DSP)-based beamformer
- **Advantages:** High flexibility and full control
- **Disadvantages:** Higher power consumption; limited dynamic range

**Analog Beamforming:**
- **Configuration:** 1 RF chain + N antenna elements + Analog beamformer modules (each with phase shifter and attenuator)
- **Function:** Phase shifters and attenuators control phase and amplitude of signals transmitted from each antenna element
- **Advantages:** Cheaper than digital beamforming; higher dynamic range handling; energy-effective due to low power consumption of phase shifters/attenuators
- **Limitations:** Only one beam can be transmitted/received at a time (due to single RF chain)

**Hybrid Beamforming:**
- **Configuration:** Combines digital and analog beamforming approaches
- **Components:** Constant modulus analog beamformer (RF part) + baseband digital beamformer
- **Benefits:** Combines advantages of both digital and analog methods
- **Research Focus:** Low-resolution ADCs (Analog-to-Digital Converters) integrated with hybrid beamforming for reduced power consumption in 5G systems
- **Finding:** Low-resolution ADC beamforming systems may achieve higher energy-efficiency than traditional hybrid beamforming systems

---

### 2. MIMO and Spatial Filtering Techniques

**Multiple-Input Multiple-Output (MIMO) Integration:**
- Utilize spatial diversity to increase throughput proportionally to the number of antennas
- Require digital signal processing and additional channel information transmission
- Enable tracking of users with narrow beams

**Spatial and Frequency Filtering:**
- Antennas used as both spatial and frequency filters
- Frequency selectivity support in cognitive radio systems
- Operation capability across very wide frequency ranges (e.g., Television White Spaces - TVWS)

---

### 3. Millimeter-Wave (mm-Wave) Antenna Systems

**Operating Frequency Range:** 30 GHz to 300 GHz

**Key Implementation Aspects:**
- Latest generations (5G cellular and Wi-Fi) use multiple antennas at mm-wave frequencies
- Large-scale antenna systems with hybrid beamforming structures investigated for mm-wave band
- Optimal designs analyze hybrid beamforming structures based on:
  - Number of transceivers
  - Number of active antennas per transceiver
  - Spectrum and energy efficiency relationships
  - Energy efficiency point determination on the efficiency curve

**Advanced Applications:**
- Full-duplex techniques in millimeter-wave communications
- Reference signal design for improved channel estimation compared to purely analog beamformer approaches
- Delay-aware schemes for high energy efficiency in energy conservation and resource management

---

### 4. Reconfigurable Antenna Systems

**Core Capabilities:**
- Ability to change direction of operation
- Frequency band reconfigurability
- Integration with filtering functions
- Software-defined metasurface implementation for index modulation techniques

**Index Modulation (IM) Techniques:**
- Promise for improving energy and spectral efficiencies in high data-rate 5G wireless communications
- Implementation of spatial and subcarrier index modulations
- Beam steering and phase modulation capabilities
- Metasurface aperture modulation and multiplexing over spectral, spatial, and temporal domains using space-time coding

---

### 5. Non-Orthogonal Multiple Access (NOMA) Integration

**NOMA Capabilities and Benefits:**
- Permits more than one user to share wireless resources within a network
- Scaling improvements:
  - Scale up number of users
  - Improve user fairness
  - Enhance spectral efficiency in wireless networks
- Performance Improvements: 5-9 times improvements for number of users; up to 100% more efficiency

**NOMA Compatible Technologies:**
- Cognitive and cooperative communications
- Multiple-Input Multiple-Output (MIMO)
- Massive MIMO systems
- Physical layer security
- Future communications networks

**Hybrid Beamforming with NOMA for mm-Wave:**
- **Sub-Connected Structure (SCS) HBF-NOMA:** Energy-efficient low-complexity design
- **Fully-Connected Structure (FCS) HBF-NOMA:** Full connectivity design
- **Operating Environments:** Line-of-sight (LOS) and non-line-of-sight (NLOS) conditions at millimeter waves

**Advanced Techniques:**
- Successive Interference Cancellation-Zero Forcing (SIC-ZF) approach
- Phased Zero-Forcing (P-ZF) approach
- 3-bit quantization for sum-rate optimization in finite resolution systems
- User clustering optimization for maximum performance

---

### 6. Physical Layer Security (PHY Security)

**Traditional Approaches:**
- Artificial noise-based methods
- Transmit beamforming methods
- Limitation: May fail to provide required secure performance when legitimate user (LU) and eavesdropper (Eve) channels are highly correlated

**Frequency Diverse Array (FDA) Beamforming Approach:**
- Innovation: Deliberately introduces frequency offsets over array antennas
- Function: Decouples LU and Eve's channels
- Security Enhancement: Degrades Eve's ability to listen to correct information; enhances physical layer security
- Optimization: Maximizes secrecy through optimization of both frequency offsets and transmit beamformer

**Physical Layer Security Protocols:**
- Derivation from intrinsic channel properties of transmission environment
- Applied to:
  - Key generation
  - Randomness extraction
  - Sharing
- Performance Characteristics: Low computational complexity; good energy efficiency; sustained unconditionally secure communications

**Advanced Quantization Scheme:**
- Comprehensive quantization scheme for physical layer security
- Focus: Intrinsic channel characteristics and crucial performance metrics

---

### 7. Dielectric Antenna Technology for Size Reduction

**Objective:** Reduce antenna size while maintaining performance

**Key Research Direction:** Explore potential in dielectric antennas to enable:
- Size reduction
- Modified cellular system operation through overlapping antenna beam advantages

**Design Approach for Omnidirectional Enhanced-Gain Antennas:**
- Transmit equal beamforming signals in all directions
- Omnidirectional pattern with enhanced gain
- Accurate beamforming capability

**Enhancement Method:**
- Introduce constant to the adaptive RLS (Recursive Least Squares) algorithm
- Enhance antenna gain while providing strong beamforming signal to desired users
- Reduce interference effects on signal

---

### 8. Adaptive Beamforming in Cellular Systems

**Significance:** Industrial significance in modern wireless communication systems

**Applications:**
- Emerging technologies like Long-Range Evolution (LTE)
- 5G technology implementation
- Accommodation of increasing network services:
  - Internet of Things (IoT)
  - Mobile broadband

**Massive and Adaptive Beamforming:** Critical component of 5G capability to accommodate ever-increasing network services

---

### 9. Non-Coherent SIMO (Single-Input Multiple-Output) Systems

**Framework Characteristics:**
- Non-coherent, non-orthogonal massive SIMO implementation
- Large antenna deployment creating high spatial diversity
- Ultra-reliable communications enablement

**Latency Reduction:**
- Non-coherent and non-orthogonal multiple access techniques reduce latency effects at:
  - Physical layer
  - Data link layer

**Practical Implementation:**
- Two-user Industrial IoT (IIoT) system example:
  - 2 controlled nodes (CNs) transmit signals to managing node (MN)
  - Transmission uses shared time-frequency resource block (RB)
  - MN employs noncoherent maximum likelihood detector
  - Recovery of transmitted symbols from received sum signal

**Performance Result:** Smaller error probability compared to other designs

---

### 10. Energy-Based Modulation for Non-Coherent Detection in Industrial IoT

**Design Framework:**
- Energy-based modulation constellation design for noncoherent detection
- Massive SIMO systems for ultra-reliable, low-latency wireless communication
- Industrial IoT communications focus

**System Configuration:**
- Single antenna transmitter linked to receiver with large antenna array
- Signal transmission through Rayleigh fading channel
- Data decoding after each symbol termination

**Advanced Decoding Algorithm:**
- Fast noncoherent decoding algorithm development
- Closed-form expression of symbol error probability (SEP) for non-negative PAM modulation SIMO systems

**System Optimization:**
- Energy efficiency enhancement through optimal PAM constellation selection
- Minimization of exact SEP
- Derived upper and lower bounds for optimal SEP
- Unique expression for coding gain optimization in massive SIMO systems

---

## Simulation Results and Performance Metrics

### Microstrip Linear Antenna Array (5G - 28 GHz)

| Metric | Value | Unit |
|--------|-------|------|
| Number of Elements | 16 | patches |
| Operating Frequency | 28 GHz | - |
| Maximum Gain | 17.4 | dBi |
| Peak Gain Frequency | 28.4 | GHz |
| 10-dB Bandwidth | >2 | GHz |
| Substrate Material | RT/Duroid 5880 | - |
| Dielectric Constant | 2.2 | - |
| Substrate Thickness | 0.381 | mm |
| Radiation Efficiency | High | - |
| Design Validation | CST Microwave Studio | simulation |

---

### Circularly Polarized Loop-Type Ground Radiation Antenna

| Metric | Value | Unit |
|--------|-------|------|
| Operating Frequency Range | 2.4-2.48 | GHz |
| Bandwidth at -6 dB | 150 | MHz |
| Axial Ratio (AR) Bandwidth at 3 dB | 130 | MHz |
| Polarization Type | Circular (LHCP/Reverse) | - |
| Phase Shift Between Modes | 90 | degrees |

---

### Compact Double Folded Loop (DFL) Antenna for Metal-Proximity Applications

| Metric | Value | Unit |
|--------|-------|------|
| Operating Frequency Band | 2.4 | GHz |
| Connection Terminal Location | λ/4 | wavelength |
| Radiation Efficiency Gain vs. λ/2 Dipole | >6 | dB |
| Metal Proximity Operation | Yes | - |
| Form Factor | Compact | - |

---

### Multi-Band 5-Element MIMO Antenna System

**Operating Frequency Bands:**

| Frequency Range | Application | Bandwidth |
|-----------------|-------------|-----------|
| 754-971 MHz | LTE Sub-GHz | ~217 MHz |
| 1.65-1.83 GHz | LTE Band 1 | 0.18 GHz |
| 2.4-3.66 GHz | RFID/LTE Band 2 | 1.26 GHz |
| 5.1-5.6 GHz | WLAN/LTE Band | 0.5 GHz |
| 0.668-1.94 GHz | Spectrum Sensing | 1.272 GHz |
| 3-4.6 GHz | Spectrum Sensing | 1.6 GHz |

---

### Non-Coherent SIMO System Performance

**Key Finding:** The non-coherent massive SIMO framework demonstrates smaller error probability when compared to other designs, confirming ultra-reliable communication capability for Industrial IoT applications.

---

## References

[1] P. Sotenga, P. Chuku, and T. Olwal, "Analysis of IEEE 802.11n Network Access Categories in EDCA non-saturated Networks," IEEE Intl Conf. on Computing, Comm. and Security (ICCCS), January 2016.

[2] A. A. Lysko, C. R. Burger, and E. Hagopian, "Comparison of the Modelled Maximum Wireless Link Distance for TVWS and Wi-Fi within South African Regulatory Constraints: Which Technology Wins and in Which Scenarios?" 2019 IEEE WAC, Pretoria, Aug 2019.

[3] I. A. Rumyancev and A. S. Korotkov, "Survey on Beamforming Techniques and Integrated Circuits for 5G Systems," 2019 IEEE Intl Conf. on Electr. Eng. and Photonics (EExPolytech), Oct 2019.

[4] K. Roth et al., "A Comparison of Hybrid Beamforming and Digital Beamforming with Low-Resolution ADCs for Multiple Users and Imperfect CSI," IEEE J. of Selected Topics in Signal Processing, Vol. 12, No. 3, June 2018.

[5] M. M. Molu et al., "Low-Complexity and Robust Hybrid Beamforming Design for Multi-Antenna Communication Systems," IEEE Trans. on Wireless Comm., Vol. 17, No. 3, March 2018.

[6] S. Rajoria, A. Trivedi, and W. W. Godfrey, "A comprehensive survey: Small cell meets massive MIMO," Phys. Comm., Vol. 26, February 2018.

[7] I. Ahmed et al., "A Survey on Hybrid Beamforming Techniques in 5G Architecture and System Model Perspectives," IEEE Comm. Surveys Tutorials, Vol. 20, No. 4, 2018.

[8] I. Ahmed et al., "A Survey on Hybrid Beamforming Techniques in 5G Architecture and System Model Perspectives," IEEE Comm. Surveys Tutorials, Vol. 20, No. 4, 2018.

[9] P. Karami and S. Mojtaba Atarodi, "Beamforming, null-steering, and simultaneous spatial and frequency domain filtering in integrated phased array systems," AEU - International Journal of Electronics and Communications, Vol. 110, October 2019.

[10] A. A. Lysko, F. V. Nelwamondo, and L. P. Mfupe, "Television Whitespace Sharing: CSIR's experimental research experiences on a new way to connect people and business," SAIEE WattNow, July 2020.

[11] Tian Lin et al., "Hybrid Beamforming for Millimeter-Wave Systems Using the MMSE Criterion," IEEE Trans. on Comm., Vol. 67, May 2019.

[12] K. Satyanarayana et al., "Hybrid Beamforming Design for Full-Duplex Millimeter Wave Communication," IEEE Trans. on Vehicular Technology, Vol. 68, No. 2, Feb. 2019.

[13] Mojtaba Vaezi et al., "Interplay Between NOMA and Other Emerging Technologies: A Survey," IEEE Transactions on Cognitive Communications and Networking, Vol. 5, No. 4, Dec. 2019.

[14] A. A. Badrudeen, "Performance Analysis of Hybrid Beamforming Precoders for Multiuser Millimeter Wave NOMA Systems," IEEE Trans. on Vehicular Technology, Vol. 69, No. 8, Aug. 2020.

[15] M. A. Almasi et al., "Impact of Beam Misalignment on Hybrid Beamforming NOMA for mmWave Communications," IEEE Trans. on Communications, Vol. 67, No. 6, June 2019.

[16] Z. Zahid, L. Qu, K. H-Hoon, and H. Kim, "Circularly Polarized Loop-Type Ground Radiation Antenna for IoT Applications," J. of Electromagn. Eng. and Sci., Vol. 19, No. 3, 2019.

[17] L. H. Trinh, T. N. Le, R. Staraj, F. Ferrero, and L. Lizzi, "A Pattern-Reconfigurable Slot Antenna for IoT Network Concentrators," Electronics, Article 6, 105, 2018.

[18] L. Jingran et al., "Physical-Layer Security for Proximal Legitimate User and Eavesdropper: A Frequency Diverse Array Beamforming Approach," IEEE Trans. on Inform. Forens. and Secur., Vol. 13, No. 3, March 2018.

[19] M. Bottarelli et al., "Physical characteristics of wireless communication channels for secret key establishment: A survey of the research," Computers Security, Vol. 78, September 2018, pp. 454-476.

[20] N. Yang and K. W. Leung, "Size Reduction of Omnidirectional Cylindrical Dielectric Resonator Antenna Using a Magnetic Aperture Source," IEEE Trans. on Ant. and Propag., Vol. 68, No. 4, April 2020.

[21] M. Abedian et al., "Wideband rectangular dielectric resonator antenna for low-profile applications," IET Microw., Ant. Prop., Vol. 12, Aug 2017.

[22] P. Chuku, T. Olwal, and K. Djouani, "Enhanced RLS in Smart Antennas for Long-Range Communication Networks," The 9th Intl Conf. on Ambient Systems, Netw. and Technologies (ANT 2018).

[23] J. A. Hodge, K. V. Mishra, and A. I. Zaghlooul, "Reconfigurable Metasurfaces for Index Modulation in 5G Wireless Communications," 2019 Intl Applied Comput. Electromagn. Soc. Symp. (ACES).

[24] D. Johnson, "The 5G Dilemma: More Base Stations, More Antennas-Less Energy," IEEE Spectrum Newsletter, 03 October 2018.

[25] M. A. Saada, T. Skait, and R. Alhalabi, "Design of Efficient Microstrip Linear Antenna Array for 5G Communications Systems," ICPET 2017.

[26] S. Han, I. Chih-Lin, Z. Xu, and C. Rowell, "Large-Scale Antenna Systems with Hybrid Analog and Digital Beamforming for Millimeter Wave 5G," Millimeter-Wave Communications for 5G, IEEE Comm. Mag. 2015.

[27] C. X. Mavromoustakis, A. Bourdena, G. Mastrakis, E. Pallis, and G. Kormentzas, "An Energy-Aware Scheme for Efficient Spectrum Utilization in a 5G Mobile Cognitive Network Architecture," Telecommunications Systems Conference 2015.

[28] C. Shanzhi, S. Shaohui, G. Oiubin, and S. Xin, "Adaptive Beamforming in TDD-Based Mobile Communication Systems: State of The Art and 5G Research Directions," IEEE Wireless Communications, 2016.

[29] H. Chen, Z. Dong, and B. Vucetic, "Noncoherent and non-orthogonal Massive SIMO for Critical Industrial IoT Communications," IEEE Intl Conf. on Industr. Cyber Physical Systems (ICPS) 2019.

[30] X. Gao et al., "Energy-Efficient and Low-Latency Massive SIMO Using Noncoherent ML Detection for Industrial IoT Communications," IEEE Internet of Things J., Vol. 6, No. 4, 2019.

[31] K. R. Jha, B. Bukhari, C. Singh, G. Mishra, and S. K. Sharma, "Compact Planar Multistandard MIMO Antenna for IoT Applications," IEEE Trans. on Antennas and Propagation, Vol. 66, No. 7, 2018.

[32] Z. Zahid, L. Qu, K. H-Hoon, and H. Kim, "Circularly Polarized Loop-Type Ground Radiation Antenna for IoT Applications," J. of Electromagnetic Eng. and Sci., Vol. 19, No. 3, 2019.

[33] Y. Koga and M. Kai, "A Compact Antenna for IoT Applications Operable even in Close Proximity to a Metal," IEEE Intl Symp. on Ant. and Propag. (USNCURSI Nat. Radio) 2018.

[34] M. Aldababsa et al., "A Tutorial on Nonorthogonal Multiple Access for 5G and Beyond," Wireless Comm. and Mobile Computing, 2018.

---

## Document Notes

**Important Note Regarding Diagrams and Figures:**

The original research paper is a literature survey and overview document. While it references numerous diagrams, figures, and illustrations from its 35+ cited publications, these visual elements are contained within the referenced papers rather than being presented in the original document itself. The paper serves as a comprehensive overview of antenna research directions for 6G rather than presenting novel antenna designs with accompanying original visual specifications.

**Sections Successfully Extracted:**

- All mathematical equations and theoretical models
- Five distinct antenna designs with complete technical specifications
- Ten design techniques, configurations, and methodologies
- Simulation results and performance metrics with tabular data
- Complete reference list with 34 cited publications
- All parametric specifications and performance characteristics

**Content Organization:**

This extraction maintains the original context and relationships between technical concepts while presenting them in a clean, organized format suitable for professional reference and documentation purposes.


