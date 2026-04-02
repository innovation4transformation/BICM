# BICM
BICM – Bi-focal Innovation Contagion Model
This model has been developed by David Alkaher as part of the resreach: Winning the Tug of War in Hierarchical Military Organizations: Achieving Anti-Fragility through the Institutionalization of Effective Innovation Management Systems

**Overview**
The Bi-focal Innovation Contagion Model (BICM) simulates the diffusion of innovation and resistance within a hierarchical public sector organization (PSO).
Agents represent individuals whose energy of change evolves over time through local interactions. Exposure to innovation-supporting agents increases this energy, while exposure to resistance-supporting agents decreases it. The model captures how micro-level interactions, constrained by organizational hierarchy, give rise to emergent system-level patterns such as innovation diffusion, stagnation, or collapse.

**Core Mechanism**
The model is governed by a simple dynamic:
Innovation (contagion) → increases energy
Resistance (bleeding) → decreases energy
Hierarchy constraint → influence flows:
downward (from higher ranks)
laterally (same rank)
not upward

Each agent’s trajectory depends on the balance between these opposing forces.

**Agent Types**
Agents are represented by colors corresponding to behavioral states:
🔴 Red (Resister)
Reduces the energy of others (energy bleeding)
⚪ Gray (Neutral / Susceptible)
Does not actively influence others
🟢 Green (Innovator)
Increases others’ energy (innovation contagion)
🔵 Blue (Fully Adapted)
Strong innovation carriers; reinforce diffusion
⚙️ White (CINO – Chief Innovation Officer)
High-impact innovation agents with extended influence radius

**Key Variables**
Agent Attributes
energy-of-change
Continuous value representing readiness for innovation
hierarchy-level
Integer (1–9), where higher values indicate seniority
innovation-contamination-factor
Strength of positive influence (green / blue / white agents)
energy-bleeding-factor
Strength of negative influence (red agents)
radius-of-impact
Spatial interaction range (larger for CINOs)

**State Thresholds**
Energy determines behavioral state:
Energy Range	State
0–25	Red
26–49	Gray
50–79	Green
80–100	Blue
150	White (CINO)

**Interaction Logic**
At each time step:
Agents interact with nearby agents
Energy is updated:
Increased by innovation-supporting neighbors
Decreased by resistance-supporting neighbors
Influence depends on:
agent type
hierarchy relation
spatial proximity
Agents update their state based on energy thresholds

**Key Assumptions**
No upward influence (lower ranks do not affect higher ranks)
Interactions are local (proximity-based)
Movement is stochastic (random walk)
The model is heuristic, not predictive
Innovation and resistance operate as competing forces

**Running the Model**
Open the model in NetLogo
Click setup
Click go
Adjust parameters via sliders:
number of agents
contamination factors
bleeding factor
distribution of CINOs
leadership type

**Parameters**
Key tunable parameters include:
innovation-contamination-factor-var
Blue-contamination-factor-var
CINO-contamination-factor-var
energy-bleeding-factor-var
number of agents at each hierarchy level
CINO distribution (centralized vs decentralized)
leadership type (top-level agent state)
