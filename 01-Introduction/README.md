# Chapter 1: Introduction

## Overview

This chapter introduces the VS-50 suborbital launch vehicle project and establishes the research context for robust attitude and guidance control system development. It presents the motivation, objectives, and scope of the thesis work.

## Figures in This Chapter

### Figure 1.1: VS-50 Launch Vehicle
**File:** `VS-50.png`

**Description:** Complete overview of the VS-50 suborbital launch vehicle showing the overall configuration, dimensions, and key components.

**Key Features:**
- **Vehicle Type:** Single-stage suborbital launch vehicle
- **Configuration:** Rocket-powered with thrust vector control
- **Primary Mission:** Technology demonstration for micro-satellite launch capabilities
- **Cooperation:** Brazilian-German joint development (IAE-DLR)

### Figure 1.2: VS-50 Motor Thrust Profile
**File:** `Motor Thrust Profile.png`

**Description:** Comprehensive thrust profile and performance characteristics of the VS-50 motor during powered flight, including both actual thrust (with atmospheric pressure effects) and vacuum thrust, along with the thrust-to-weight ratio evolution.

**Statistics:** Max Thrust: 533.0 kN | Avg Thrust: 445.2 kN | Total Impulse: 36733 kN⋅s

**Key Performance Parameters:**
- **Burn Duration:** 82.5 seconds total powered flight
- **Peak Thrust:** 533.0 kN (vacuum conditions)
- **Thrust Profile:** Variable thrust with characteristic mid-flight dip and peak performance around 40-50 seconds
- **Maximum T/W Ratio:** ~7.4 (well above minimum T/W = 1 for vertical ascent)
- **Thrust Variation:** Shows realistic atmospheric pressure effects on actual thrust performance

**Engineering Significance:**
- **Control Design Impact:** Variable thrust profile affects vehicle dynamics and control requirements
- **Mission Analysis:** T/W ratio evolution critical for trajectory planning and control system design
- **Performance Validation:** Actual vs. vacuum thrust comparison validates propulsion model accuracy

### Figure 1.3: Vehicle Mass and Moment of Inertia Variation
**File:** `Vehicle Moments of Inertia.png`

**Description:** Comprehensive time evolution of vehicle mass and three-axis moments of inertia during powered flight, illustrating the dramatic parameter variations that constitute the primary challenge for robust control system design.

**Critical Parameter Changes:**
- **Mass Variation:** 15,644 kg → 3,603 kg (77% reduction, 12,041 kg propellant consumed)
- **Roll Moment (Ixx):** ~77,000 → ~47,000 kg⋅m² (39% reduction)
- **Pitch Moment (Iyy):** ~77,000 → ~47,000 kg⋅m² (39% reduction)
- **Yaw Moment (Izz):** ~4,500 → ~1,500 kg⋅m² (67% reduction)

**Control Design Implications:**
- **Parameter Uncertainty:** Massive variations require robust control approaches
- **Gain Scheduling:** Traditional fixed-gain controllers inadequate for this envelope
- **LMI Synthesis Justification:** Wide parameter variations motivate robust control framework
- **Performance Challenges:** Maintaining stability and tracking across dramatic operating point changes

**Physical Interpretation:**
- **Mass Loss Rate:** Approximately 146 kg/s average propellant consumption
- **Inertia Coupling:** Different reduction rates between axes create control coupling challenges
- **Dynamic Response:** Varying inertia directly affects attitude control bandwidth and response
- **Robustness Requirements:** Controllers must handle 2.5x-4x parameter variations

### Figure 1.4: Center of Gravity and Center of Pressure Variation
**File:** `CoG and CoP.png`

**Description:** Comprehensive analysis of aerodynamic stability through center of gravity (CoG) and center of pressure (CoP) evolution during powered flight, including critical static margin analysis that determines vehicle stability characteristics.

**Aerodynamic Stability Parameters:**
- **CoG Evolution:** -8.0m → -7.0m (1.0m forward shift due to propellant consumption)
- **CoP Variation:** -8.3m → -4.8m (3.5m total displacement from aerodynamic/geometric changes)
- **Static Margin Range:** -1.0m to +2.2m (critical stability parameter)

**Flight Phase Analysis:**
- **Phase 1 (0-10s):** Marginally stable with small negative static margin (~-0.3m)
- **Phase 2 (10-30s):** **Critical unstable region** with negative static margin (-1.0m minimum)
- **Phase 3 (30-82s):** Stable flight with increasing positive static margin (up to +2.2m)

**Control System Requirements:**
- **Active Stabilization:** Essential during 10-30s unstable period for flight safety
- **Precision Control:** Required during stable phase for trajectory accuracy
- **Transition Management:** Smooth control authority transition between stability regimes
- **Robustness Design:** Must handle aerodynamic uncertainty across all flight phases

**Physical Interpretation:**
- **CoG Forward Movement:** Propellant consumption shifts mass distribution forward
- **CoP Complex Evolution:** Combined effects of changing mass distribution, vehicle geometry, and aerodynamic flow patterns
- **Static Margin Physics:** Positive margin = natural stability, negative margin = inherent instability requiring active control
- **Control Authority:** Aerodynamic control effectiveness varies with dynamic pressure and static margin

**Design Significance:**
- **Traditional Control Limitation:** Fixed-gain controllers cannot handle stability regime transitions
- **Robust Control Justification:** Wide stability margin variations require adaptive/robust approaches
- **Safety Critical:** Control system failure during unstable phase results in mission loss
- **Performance Optimization:** Optimal control strategies differ between stable and unstable flight phases

## Chapter Content Summary

### Research Context
- **Problem Statement:** Need for robust control systems in launch vehicles
- **Technical Challenge:** Handling parametric uncertainties and disturbances
- **Solution Approach:** LMI-based robust control synthesis

### Project Background
- **VS-50 Program:** Brazilian-German cooperative suborbital vehicle
- **Technical Goals:** Demonstrate advanced control technologies
- **Research Objectives:** Develop and validate robust control algorithms

### Thesis Scope
- **Mathematical Modeling:** Complete vehicle dynamics and control systems
- **Controller Design:** LMI synthesis for attitude and guidance control
- **Validation:** Hardware-in-the-Loop (HIL) experimental verification
- **Performance Analysis:** Comprehensive evaluation and comparison

### Key Contributions
1. **Robust Control Framework:** Systematic LMI-based design methodology
2. **Integrated Validation:** HIL testing with actual flight hardware
3. **Performance Enhancement:** Improved robustness and tracking performance
4. **Practical Implementation:** Ready-to-deploy control algorithms

## Technical Specifications

### Vehicle Parameters
- **Length:** [Specific dimensions from thesis]
- **Diameter:** [Specific dimensions from thesis]  
- **Mass:** [Vehicle mass parameters]
- **Thrust:** [Engine specifications]

### Control System Components
- **Navigation:** DMARS high-precision inertial navigation system
- **Actuation:** Thrust Vector Actuator (TVA) for attitude control
- **Computing:** Real-time control implementation platform
- **Sensors:** Inertial measurement unit and additional sensors

### Mission Profile
- **Flight Duration:** Suborbital trajectory
- **Altitude:** [Maximum altitude achieved]
- **Control Phases:** Launch, powered flight, coast, re-entry
- **Landing:** Parachute recovery system

## Research Methodology

### Control Design Approach
1. **Mathematical Modeling:** Comprehensive vehicle dynamics
2. **Uncertainty Characterization:** Parameter variations and disturbances
3. **Robust Synthesis:** LMI-based controller design
4. **Performance Analysis:** Frequency and time domain evaluation
5. **Experimental Validation:** HIL testing and verification

### Innovation Aspects
- **LMI Framework:** Systematic robust control design
- **HIL Integration:** Real hardware validation methodology
- **Comprehensive Analysis:** Complete performance characterization
- **Practical Focus:** Industry-ready implementation

## Chapter References

This chapter references key literature in:
- Launch vehicle control systems
- Robust control theory
- LMI synthesis methods
- Hardware-in-the-loop validation
- Aerospace control applications

## Related Material

- **Chapter 2:** Detailed literature review and theoretical foundations
- **Chapter 3:** Complete mathematical modeling and control design
- **Chapter 4:** Comprehensive results and performance analysis
- **Annexes:** Additional technical details and validation results

---

**Figure Count:** 4  
**Content Type:** Project introduction and background  
**Technical Level:** Overview and motivation 