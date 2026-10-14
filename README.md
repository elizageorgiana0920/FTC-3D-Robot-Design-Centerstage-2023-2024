# FTC CENTERSTAGE Robot — 3D CAD Design & Mechanical Systems

**A collaborative robotics engineering project focused on designing, integrating, and iterating a competition robot in Onshape.**

![3D CAD model of the FTC robot](assets/robot-overview.png)

[![Onshape](https://img.shields.io/badge/CAD-Onshape-1764a0)](https://www.onshape.com/) ![FIRST Tech Challenge](https://img.shields.io/badge/Competition-FIRST%20Tech%20Challenge-555555) ![Season](https://img.shields.io/badge/Season-CENTERSTAGE%202023--24-8a2636) ![Project](https://img.shields.io/badge/Project-Team%20Engineering-555555)

## Overview

This project documents the **3D design and mechanical development of a robot for the 2023–2024 FIRST Tech Challenge (FTC) CENTERSTAGE season**. We used **Onshape**, a cloud-based parametric CAD platform, to explore mechanisms, assemble subsystems, and identify integration constraints before physical construction.

The central challenge was to fit several competition mechanisms into a single robot while balancing **speed, precision, weight, power consumption, reliability, and limited space**. The project was subsequently documented as a high-school computer science certification project in 2025.

### At a glance

| | |
| --- | --- |
| **Domain** | Robotics · Mechanical design · 3D CAD |
| **Platform** | Onshape |
| **Competition** | FIRST Tech Challenge — CENTERSTAGE (2023–2024) |
| **Robot systems** | Mecanum drivetrain, pixel intake/outtake, paper-airplane launcher, hanging mechanism |
| **Engineering approach** | Parametric modeling, assembly integration, iterative prototyping, design trade-off analysis |
| **Collaboration** | Shared cloud CAD workspace and version history |

## Robot architecture

The robot design brings together four major subsystems:

| Subsystem | Design approach | Engineering considerations |
| --- | --- | --- |
| **Drivetrain** | goBILDA mecanum-wheel chassis with 312 RPM motors | Omnidirectional mobility and maneuverability |
| **Pixel intake/outtake** | Explored brush-wheel collection, articulated arms, and a transfer mechanism | Collection speed vs. placement precision, battery usage, and reach |
| **Paper-airplane launcher** | Servo-released elastic propulsion mechanism | Launcher mass, available mounting space, launch angle, and distance |
| **Hanging mechanism** | Compared a single lift/hook concept against a dual-motor, two-point attachment approach | Completion time, stability, and mechanical reliability |

## Engineering decisions and iterations

### 1. Designing for precision, not just collection speed

Our initial pixel-handling concept used **two brush wheels, articulated arms, and a transfer belt** to move game pieces toward the outtake. While promising for rapid collection, this layout introduced trade-offs in placement accuracy and system complexity.

We explored a more integrated handling mechanism to improve control over both collection and placement. The design process also exposed constraints including **limited vertical reach, slower operation, and battery consumption**. Rather than treating the first design as final, we compared approaches against the actual requirements of the competition.

### 2. Improving the hanging mechanism

The documented first hanging concept used a **117 RPM goBILDA motor and a Viper Slide** to lift a hook. Its reported completion time was **over 30 seconds**, with a reported efficiency of approximately **30%**.

A revised concept used **two 117 RPM motors and two attachment points**, improving stability and bringing the documented completion time to **under 20 seconds** when both hooks were engaged. The trade-off was that its best performance depended on successful two-hook attachment.

> **Design lesson:** A mechanically functional solution is not necessarily a competitive one. We evaluated designs against task completion time and operational constraints, not only whether the mechanism could move.

### 3. Working within packaging constraints

The first launcher concept was too heavy for the available space. We considered mounting it on a hanging arm and using a **servo-actuated elastic release**, taking into account projectile shape, mass, force, angle, and distance.

This reinforced the importance of designing subsystems **as part of a shared assembly**, rather than optimizing each component independently.

## CAD workflow

We used Onshape to support a collaborative, iterative mechanical-design process:

1. **Define competition requirements** and determine which mechanisms need to fit together.
2. **Model individual parts** using sketches and parametric 3D operations.
3. **Assemble components** using mate connectors and assembly tools.
4. **Inspect fit, positioning, and intended movements** to identify integration issues.
5. **Compare design alternatives** based on space, speed, precision, stability, and power considerations.
6. **Track revisions collaboratively** using Onshape's shared workspace and version history.

The accompanying project report also discusses structural simulation techniques in Onshape, including stress and deformation analysis. It does **not** provide reproducible simulation outputs or quantitative structural-test results, so none are claimed here.

## What I learned

This project helped me develop an engineering mindset that also translates to software development:

- **System decomposition:** breaking a complex robot into interacting subsystems.
- **Constraint-driven design:** balancing competing requirements rather than maximizing one metric in isolation.
- **Iteration and debugging:** recognizing the limitations of early prototypes and refining designs accordingly.
- **Integration thinking:** anticipating how a change to one mechanism affects the complete system.
- **Technical collaboration:** working in a shared design environment and documenting decisions.

## Team and credits

**Eliza-Georgiana Boroș** and **Amalia-Elena Tănase**  
High-school computer science certification project (2025)  
Colegiul Național „Dimitrie Cantemir”, Onești

The design work originated in the context of the **FIRST Tech Challenge 2023–2024 CENTERSTAGE** season. Robot CAD visuals are reproduced from the team's project documentation.

---

*Interested in the design process? Start with the [robot architecture](#robot-architecture) and [engineering decisions](#engineering-decisions-and-iterations), or open the [full report](documentation/robot-design-report.pdf).* 
