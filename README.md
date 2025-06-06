# VS-50 Supplementary Material Repository

## Robust Attitude and Guidance Control for a Launch Vehicle System: A Lyapunov-LMI Framework with HIL Validation

This repository contains supplementary material for the Master's thesis:

**"Robust Attitude and Guidance Control for the VS-50 Launch Vehicle Via LMI Synthesis"**

**Author:** Roberto Brusnicki  
**Institution:** Instituto Tecnológico de Aeronáutica (ITA)  
**Program:** Master of Science in Electronic and Computer Engineering  
**Year:** 2025  

## 📋 Repository Overview

This repository provides high-resolution figures, detailed analysis results, and supplementary documentation that complement the published thesis. All materials are organized according to the thesis PDF chapter structure for easy reference.

### 🚀 Project Background

The VS-50 is a suborbital launch vehicle developed through Brazilian-German cooperation between IAE (Instituto de Aeronáutica e Espaço) and DLR (Deutsches Zentrum für Luft- und Raumfahrt). This thesis presents robust control strategies using Linear Matrix Inequality (LMI) synthesis for attitude and guidance control systems.

## 📁 Repository Structure

```
VS50-Supplementary-Material/
├── Chapter-01-Introduction/          (1 figure)
├── Chapter-02-Literature-Review/     (7 figures)  
├── Chapter-03-Mathematical-Modeling/ (28 figures)
├── Chapter-04-Results-and-Analysis/  (27 figures)
├── Annex-A-Bode-Plots/              (15 figures)
├── Annex-B-Worst-Case-Scenarios/    (10 figures)
├── README.md                         (this file)
├── PDF-to-LaTeX-Figure-Mapping.md    (technical mapping)
└── REORGANIZATION-STEPS.md           (organization guide)
```

**Total: 88 High-Resolution Figures**

## 📖 Chapter Contents

### [Chapter 1: Introduction](Chapter-01-Introduction/)
- **1 Figure**: VS-50 launch vehicle overview
- **Content**: Project background, vehicle specifications, research objectives

### [Chapter 2: Literature Review](Chapter-02-Literature-Review/) 
- **7 Figures**: Navigation systems, coordinate frames, mathematical foundations
- **Content**: State-of-the-art review in launch vehicle control, reference coordinate systems, fundamental concepts

### [Chapter 3: Mathematical Modeling and Control](Chapter-03-Mathematical-Modeling/)
- **28 Figures**: System modeling, control architectures, design methodologies
- **Content**: Complete mathematical model, control system design, LMI synthesis, HIL setup

### [Chapter 4: Results and Analysis](Chapter-04-Results-and-Analysis/)
- **27 Figures**: Frequency and time domain analysis, performance comparisons
- **Content**: Comprehensive results comparing current vs. proposed controllers, robustness analysis

### [Annex A: Additional Bode Plots](Annex-A-Bode-Plots/)
- **15 Figures**: Detailed frequency response analysis
- **Content**: Closed-loop Bode plots, controller comparisons across flight phases

### [Annex B: Worst Case Scenarios](Annex-B-Worst-Case-Scenarios/)
- **10 Figures**: Mission performance under extreme conditions
- **Content**: Worst-case disturbance analysis, controller performance comparison

## 🛠️ Technical Highlights

### Control Methodologies
- **LMI-based Robust Control**: Lyapunov stability guarantees
- **Gain Scheduling**: Adaptation to varying flight conditions  
- **H∞ Control**: Disturbance rejection and robustness
- **PID Control**: Baseline comparison and implementation

### Validation Approach
- **Hardware-in-the-Loop (HIL)**: Real-time validation using actual flight hardware
- **Monte Carlo Simulations**: Statistical performance assessment
- **Worst-Case Analysis**: Robustness verification under extreme conditions

### Key Technologies
- **DMARS Navigation System**: High-precision inertial navigation
- **TVA (Thrust Vector Actuator)**: Primary attitude control actuator
- **Real-Time Implementation**: LabVIEW-based control system

## 📊 Key Results

### Performance Improvements
- **Enhanced Robustness**: Superior performance under parameter uncertainties
- **Improved Tracking**: Better attitude and guidance response
- **Extended Stability Margins**: Increased phase and gain margins
- **Validated Performance**: Confirmed through HIL testing

### Innovation Contributions
1. **LMI Synthesis Framework**: Systematic robust controller design
2. **Integrated HIL Validation**: Real hardware testing methodology  
3. **Comprehensive Analysis**: Complete frequency and time domain evaluation
4. **Practical Implementation**: Ready-to-deploy control algorithms

## 🔗 Related Publications

### Submitted Journal Paper
**Title:** "Robust Attitude and Guidance Control for a Launch Vehicle System: A Lyapunov-LMI Framework with HIL Validation"

**Authors:** 
- Roberto Brusnicki (TUM)
- Cesar Batagini (IAE) 
- Josef Ettl (DLR)
- Renan Lima Pereira (ITA)

**Journal:** Aerospace Science and Technology (Under Review)

## 📚 How to Use This Repository

### For Researchers
1. **Reference Figures**: All figures are numbered according to the thesis PDF
2. **High-Resolution Access**: Download original image files for presentations/papers
3. **Detailed Analysis**: Explore comprehensive results in each chapter directory
4. **Methodology Understanding**: Review mathematical models and control architectures

### For Students
1. **Learning Resource**: Study control system design methodologies
2. **Implementation Guide**: Reference HIL setup and validation procedures  
3. **Mathematical Foundation**: Access detailed modeling equations and derivations
4. **Performance Analysis**: Understand robustness evaluation techniques

### For Industry
1. **Control Algorithms**: Reference robust control design procedures
2. **Validation Methods**: HIL testing protocols and procedures
3. **Performance Metrics**: Evaluation criteria and benchmarking approaches
4. **Implementation Guidelines**: Practical deployment considerations

## 🏛️ Institutional Acknowledgments

### Academic Institutions
- **ITA (Instituto Tecnológico de Aeronáutica)** - Brazil
- **TUM (Technical University of Munich)** - Germany  
- **IAE (Instituto de Aeronáutica e Espaço)** - Brazil
- **DLR (Deutsches Zentrum für Luft- und Raumfahrt)** - Germany

### Project Collaboration
This work was conducted under the Brazilian-German cooperation in space technology, specifically within the VS-50 suborbital launch vehicle development program.

## 📄 Citation

If you use this material in your research, please cite:

```bibtex
@mastersthesis{brusnicki2025robust,
  title={Robust Attitude and Guidance Control for the VS-50 Launch Vehicle Via LMI Synthesis},
  author={Brusnicki, Roberto},
  year={2025},
  school={Instituto Tecnológico de Aeronáutica},
  type={Master's thesis},
  address={São José dos Campos, Brazil}
}
```

## 📞 Contact

**Roberto Brusnicki**  
- 📧 Email: [roberto.brusnicki@tum.de]
- 🔗 LinkedIn: [linkedin.com/in/roberto-brusnicki]
- 🎓 Institution: Technical University of Munich (TUM)

## 📝 License

This repository is provided for academic and research purposes. Please refer to the individual figure sources and respect copyright restrictions when using materials for publications.

---

**Last Updated:** June 2025  
**Repository Version:** 1.0  
**Total Figures:** 88  
**Thesis Status:** Completed 