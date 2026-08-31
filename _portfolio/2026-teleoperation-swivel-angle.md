---
title: "7-DOF Teleoperation with Swivel-Angle Constraints"
excerpt: "Constraining a redundant arm by the operator's elbow angle for better posture alignment, with a Pareto analysis against multi-node IK."
collection: portfolio
---

A 7-DOF arm is kinematically redundant: many joint configurations reach the same end-effector pose. In teleoperation this shows up as an arm that gets to the right place in the wrong posture.

I constrained the redundancy using the operator's own **elbow angle** (the swivel angle about the shoulder–wrist axis), rather than tracking the elbow *position* as an extra IK node. A simulated **Pareto analysis** across posture-alignment and end-effector-accuracy objectives showed the swivel-angle formulation gives superior end-effector accuracy over the elbow-position multi-node formulation.

**Pipeline**
* Operator pose estimated from a **RealSense D435i** with GPU-accelerated **VINS-Fusion**
* A joint-calibration workflow that brought reconstruction error down to **11%**, making the swivel angle usable in real time
* Extracted swivel angle fed as a constraint to a **PyBullet** IK solver driving the **OpenArm**

*Dimeidos, Kaohsiung — 2026*
