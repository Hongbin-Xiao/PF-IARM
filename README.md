# PF-AIRM: Problem-Oriented Requirements Modeling for Intelligent Agents

[![License](https://img.shields.io/badge/license-Academic-blue.svg)]()
[![Paper](https://img.shields.io/badge/paper-Published-green.svg)]()
[![Framework](https://img.shields.io/badge/framework-PF--AIRM-orange.svg)]()

## 📋 Overview

**PF-AIRM** (Problem Frames based Agent Intelligent Requirements Modeling) is a systematic requirements engineering methodology specifically designed for intelligent agent systems in industrial applications. This method innovatively integrates Jackson's Problem Frames theory with the intelligent agent paradigm to address the limitations of traditional requirements engineering approaches in capturing agent characteristics such as autonomy, adaptability, and uncertainty.

## 🎯 Key Features

- **Extended Meta-Model**: Incorporates intelligent agent domain, environment domain, knowledge domain, and goal domain
- **Four Core Problem Patterns**:
  - Perception-Decision-Execution (PDE) Pattern
 ![四种模式_01](https://github.com/user-attachments/assets/0be80675-f831-467a-babd-f0fbe15440d2)


  - Knowledge Acquisition and Learning Pattern
    ![四种模式_01(1)](https://github.com/user-attachments/assets/651aa824-caf5-47c5-94eb-5806a4a148e2)

  - Goal-Oriented Behavior Pattern
 
    ![四种模式_01(2)](https://github.com/user-attachments/assets/ec7e5fe3-7ac8-4541-84ad-9cea515185b3)

  - Multi-Agent Collaboration Pattern
 
  ![四种模式_01(3)](https://github.com/user-attachments/assets/2339303d-213e-4a11-809b-1a00b68cf9e9)


- **Graphical Modeling Platform**: Visual requirements modeling tool with standardized notation system
- **Industrial Pattern Library**: Reusable problem patterns for common industrial scenarios

## 🏗️ Architecture
![面向问题的智能Agent需求建模方法-图(1)_01(1)](https://github.com/user-attachments/assets/d6c6fdfc-9f15-41b7-80d8-96fba1677bd1)


## 🔬 Methodology

### 1. Requirements Elicitation and Analysis
- Stakeholder interviews
- Scenario analysis
- Goal decomposition
- Constraint identification

### 2. Problem Decomposition and Framework Selection
- Functional/goal-based decomposition
- Pattern matching from library
- Framework composition strategy

### 3. Problem Context Modeling
- Domain identification and description
- Phenomenon and interface definition
- Requirements specification

### 4. Requirements Specification Generation
- Formal specification extraction
- Completeness and consistency validation
- Stakeholder confirmation
- Iterative refinement

## 📊 Formal Definitions

### Intelligent Agent Domain
\[A = (C, K, G, L, F)\]
- \(C\): Capability set
- \(K\): Knowledge base
- \(G\): Goal set
- \(L\): Learning mechanism
- \(F\): Function set

### Environment Domain
\[E = (S, O, D)\]
- \(S\): State space
- \(O: S \rightarrow P\): Observability function
- \(D: S \times A \rightarrow S\): Dynamics function

### Knowledge Domain
\[K = (T, R, U, V)\]
- \(T\): Knowledge type
- \(R\): Relations
- \(U: K \rightarrow [0,1]\): Uncertainty measure
- \(V: K \rightarrow \{true, false, unknown\}\): Verification mechanism

### Goal Domain
\[G = (P, C, E)\]
- \(P: G \rightarrow \mathbb{R}\): Priority function
- \(C\): Constraint set
- \(E: S \rightarrow [0,1]\): Evaluation function

## 🎨 Graphical Notation

| Element | Type | Representation |
|---------|------|----------------|
| Intelligent Agent | Domain T3 | Orange rectangle with agent icon |
| Environment | Domain T3 | Blue rectangle |
| Knowledge | Domain T3 | Green rectangle |
| Goal | Domain T3 | Purple rectangle |
| Machine | Domain T1 | White rectangle |
| Interface | Relationship | Solid line connection |
| Phenomenon | Relationship | Labeled connection (Domain!{Phenomenon}) |

## 💡 Case Study: Intelligent Customer Service Agent

The methodology was validated through a comprehensive case study of an e-commerce intelligent customer service system, demonstrating:

- **Query Understanding & Response**: PDE pattern for natural language processing
- **Knowledge Learning & Update**: Dynamic knowledge base management
- **Transaction Processing**: Goal-oriented automated operations
- **Human Handoff Decision**: Multi-agent collaboration for complex queries
- **Service Quality Optimization**: Continuous improvement through feedback

## 📈 Evaluation Results

### Comparison with Existing Methods

| Method | Agent Domain | Environment | Knowledge | Goal | Uncertainty | Temporal |
|--------|--------------|-------------|-----------|------|-------------|----------|
| PF-CPS | ❌ | ✅ | ❌ | ❌ | ❌ | ❌ |
| PF-HCPS | ❌ | ✅ | ❌ | ❌ | ❌ | ❌ |
| PF-STPA | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |
| **PF-AIRM** | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |

### Key Improvements
- ✅ Enhanced expressiveness for agent characteristics
- ✅ Systematic requirements analysis process
- ✅ Reduced transformation cycle from requirements to design
- ✅ Improved requirement completeness and accuracy

![00e98020cf3ddfd1e4dca83be3f218cc](https://github.com/user-attachments/assets/6eb7b3a8-c3dd-4c1f-95e3-3f4e68badcad)


## 🛠️ Installation & Usage

```bash
# Clone the repository
git clone https://github.com/yourusername/PF-AIRM.git

# Install dependencies
cd PF-AIRM
npm install

# Launch the modeling platform
npm start
@article{xiao2025pfairm,
  title={Problem-Oriented Requirements Modeling Methodology for Intelligent Agents},
  author={Xiao, Hongbin and Liu, Wanglong and Tan, Shuru and Wang, Wenhao and Li, Zhi and Tang, Fei},
  journal={Journal of Wuhan University (Natural Science Edition)},
  year={2025}
}
