# Scope of Work (SOW): AI-Driven Automation of Puppetry 
**(With Emphasis on Precedent Research & Existing Systems)**

---

## 1. Project Overview
This project seeks to create a **Minimum Viable Product (MVP)** for an AI-driven mechanical puppetry system, initially focusing on a **simple puppet** (e.g., a wagging tail, swaying branch, or minimalist Javanese-style figure). The overarching vision is to scale up to complex Javanese shadow puppetry, enabling **AI-controlled performances** that blend tradition with cutting-edge robotics and artificial intelligence.

A critical component is **researching existing animatronic and robotic systems**—both commercial and academic—to understand industry best practices, potential pitfalls, and design inspirations. This will ensure the MVP is informed by established solutions and well-positioned for expansion.

---

## 2. Objectives
1. **Precedent & Market Research**  
   - Identify, evaluate, and document existing solutions (e.g., Disney animatronics, Jim Henson Creature Shop, RoboThespian, academic robotics labs).  
   - Synthesize lessons learned to guide our mechanical design and AI integration.

2. **MVP Mechanical Puppet**  
   - Develop a small-scale puppet with **1–2 degrees of freedom** as a proof of concept.  
   - Include basic actuation (servo, stepper, or similar) and potential sensors for interactive or responsive motion.

3. **AI/ML Motion Generation**  
   - Gather movement data (video recordings, sensor streams) and train a **lightweight AI model** (could be an LLM or a specialized ML approach).  
   - Enable real-time or near-real-time motion control, allowing the puppet to mimic or improvise movements.

4. **Integration & Demonstration**  
   - Build a **hardware-software control loop** (microcontroller + AI + mechanical rig).  
   - Showcase at least one dynamic behavior (e.g., responding to a “wind” sensor or user command) with a smooth, stable motion.

5. **Scalability & Future-Proofing**  
   - Design modularly, so the system can expand to multi-axis Javanese shadow puppets.  
   - Incorporate best practices from the research phase to allow more complex gestures and potential multi-puppet coordination.

---

## 3. Precedent Research & Existing Systems
1. **Disney Animatronics**  
   - Known for realistic character motions in theme parks (e.g., Pirates of the Caribbean, Star Wars figures).  
   - Use advanced servo systems, hydraulic/pneumatic actuators, and sophisticated control software.  
   - Patented technology around smooth motion curves and real-time control.

2. **Jim Henson Creature Shop**  
   - Pioneers in puppetry for film/TV, combining mechanical rigs with remote puppeteering.  
   - Focus on expressive, lifelike movements using cable, rod, and servo-driven systems.

3. **RoboThespian & Similar Platforms**  
   - Commercially available humanoid robots designed for entertainment and education.  
   - Incorporate motion capture and scripting for real-time or pre-programmed performances.

4. **Academic & Research Projects**  
   - University labs exploring robotic arms and custom animatronics (e.g., MIT Media Lab, Carnegie Mellon Robotics Institute).  
   - Open-source robotics frameworks (ROS, etc.) that could be adapted for puppetry control.

5. **Gaps & Opportunities**  
   - **Real-time, AI-driven** motion generation specifically for cultural or artistic performances.  
   - **Lightweight** solutions for smaller puppets or simpler mechanical rigs.  
   - **Interactive** systems that react dynamically to human performers or environmental inputs.

**Outcome of Research:**  
This investigation will guide hardware selection (servo type, control boards, mechanical linkages) and inform the design of an **AI-driven control** methodology tailored to puppetry’s unique needs (smooth, expressive, often delicate movements).

---

## 4. Requirements

### 4.1 Mechanical & Hardware
- **Simple Puppet Rig**  
  - 1–2 degrees of freedom (e.g., rotating joint, bending hinge) for demonstration.  
  - 3D-printed or laser-cut parts for rapid prototyping and iteration.
- **Actuators & Controllers**  
  - Servos or stepper motors (low-cost, standard torque) plus drivers.  
  - Optional sensor (e.g., IMU or “wind” sensor) if interactive demonstration is desired.
- **Structural Framework**  
  - Lightweight materials (acrylic, plywood, or aluminum extrusions).  
  - Secure mounting points for motors, ensuring minimal backlash or wobble.

### 4.2 Software & AI
- **Data Capture & Pre-processing**  
  - Video or sensor-based recordings of basic puppet motions.  
  - Labeling and segmentation for training a model (e.g., “wag left,” “wag right,” “idle”).
- **Model Training**  
  - A **lightweight AI/ML model** (could be a small neural net or LLM-based sequence generator).  
  - Ability to generate joint angle commands at regular intervals (e.g., 10–30 fps).
- **Control Interface**  
  - Microcontroller (Arduino, Raspberry Pi) or PC-based environment interfaced with motor drivers.  
  - Real-time feedback loop to handle sensor input or user commands.
- **User Interface (UI)**  
  - Simple application (desktop, web, or microcontroller-based) to start/stop puppet motion, switch between modes, or override AI.

### 4.3 Performance & Scalability
- **Latency**  
  - Aim for sub-200ms from AI output to puppet movement.  
  - Minimizing lag ensures natural or “lifelike” motion.
- **Reliability**  
  - Must handle repeated cycles without motor burnout or mechanical failures.  
  - Sufficient torque margin for all tested movements.
- **Modularity**  
  - Design everything with an eye toward adding more degrees of freedom or more puppets.  
  - Code structured to accept additional servo channels or advanced AI modules.

---

## 5. Scope of Work

### 5.1 Phase 1: Precedent & Market Research
1. **Comprehensive Literature & Product Review**  
   - Delve deeper into Disney animatronics, Jim Henson techniques, and academic projects.  
   - Document mechanical designs, actuator types, control software approaches, and relevant patents.  
2. **Research Synthesis & Feasibility**  
   - Identify which design elements or control methodologies could apply to an MVP puppet.  
   - Outline the unique features we can improve upon or adapt for a smaller-scale puppet.

**Deliverables:**  
- **Annotated Research Summary**: including mechanical and AI insights from existing systems.  
- **Feature Comparison Matrix**: cost, complexity, potential adaptation to our MVP.

---

### 5.2 Phase 2: Concept Development & System Architecture
1. **Mechanical Concept Design**  
   - Sketch a simple puppet with one pivot (e.g., a tail or branch) or a small set of linkages.  
   - Decide on materials and actuation approach (servo vs. stepper).
2. **AI & Control Flow Design**  
   - Draft a **block diagram** for data flow: sensors → AI model → motor controllers.  
   - Define performance metrics (speed, torque, reaction time).

**Deliverables:**  
- **Concept Sketches**: initial mechanical drawings.  
- **Architecture Diagram**: showing how AI, sensors, and actuators will interact.

---

### 5.3 Phase 3: CAD & Mechanical Prototyping
1. **Detailed CAD Modeling**  
   - Create 2D and 3D CAD designs (Autodesk Inventor or similar).  
   - Ensure bracket and linkage designs align with chosen actuators.
2. **Simulation & Validation**  
   - Perform basic kinematic checks (range of motion, servo torque).  
   - Identify potential points of mechanical stress or collision.

**Deliverables:**  
- **Parametric CAD Files**: covering puppet structure, brackets, and linkages.  
- **Simulation Reports**: verifying motion feasibility (range, torque requirements).

---

### 5.4 Phase 4: Data Capture & AI Model Training
1. **Motion Data Collection**  
   - Record short puppet movements (manual manipulation or reference videos).  
   - Label frames/sequences to train a motion-generation model (e.g., “wag,” “idle,” “random wiggle”).
2. **Training a Lightweight Model**  
   - Use a simple neural network or a small LLM for sequence generation.  
   - Validate output on test sets to ensure fluid, stable motion commands.

**Deliverables:**  
- **Labeled Motion Dataset**: raw videos and processed sensor data.  
- **Trained Model Files**: plus documentation (hyperparameters, training logs).

---

### 5.5 Phase 5: Integration & Assembly
1. **Hardware Build**  
   - Fabricate or 3D-print mechanical parts from CAD designs.  
   - Assemble puppet rig with servo(s) and sensor(s).
2. **Software Integration**  
   - Implement real-time control software on a microcontroller or PC.  
   - Connect the AI model to the servo controller, ensuring smooth signal flow.
3. **Initial Testing & Debugging**  
   - Verify basic functionality (does the puppet move as commanded?).  
   - Calibrate angles, check for mechanical interference, fine-tune servo speed/torque settings.

**Deliverables:**  
- **Assembled MVP Puppet**: physically complete and powered.  
- **Functional Control Software**: bridging AI output and servo input.  
- **Initial Test Footage**: short video showcasing basic movements.

---

### 5.6 Phase 6: System Testing, Iteration & Demonstration
1. **Extended Performance Testing**  
   - Run repeated cycles to confirm reliability.  
   - Evaluate movement fluidity, responsiveness, and any mechanical wear.
2. **Model & Design Optimization**  
   - Adjust AI model parameters to refine motion transitions and variety.  
   - Reinforce or reprint any weak mechanical parts discovered during testing.
3. **Final MVP Demonstration**  
   - Present the system to stakeholders, highlighting how AI-generated motions adapt to triggers (e.g., user commands, sensor input).  
   - Document potential next steps for scaling up to multi-axis puppets.

**Deliverables:**  
- **Performance Logs**: reliability, servo temperature checks, motion smoothness metrics.  
- **Refined Model & Mechanical Design**: if iterative improvements were made.  
- **Demonstration Video & Presentation**: final showcase of the MVP system.

---

## 6. Timeline

| Phase                            | Duration (Weeks) | Key Milestones                                           |
|----------------------------------|------------------|----------------------------------------------------------|
| **1. Precedent & Market Research** | 1–2              | Research summary & recommendations                       |
| **2. Concept Development**       | 1–2              | Mechanical & AI architecture finalized                   |
| **3. CAD & Prototyping**         | 2–3              | CAD files + simulation analysis                          |
| **4. Data & Model Training**     | 2–4              | Labeled dataset + trained motion-generation model        |
| **5. Integration & Assembly**    | 3–4              | Puppet assembled + baseline software integration         |
| **6. Testing & Demonstration**   | 2–3              | Optimized system + final MVP showcase                    |

*(Timelines may shift depending on complexity, availability of materials, and research findings.)*

---

## 7. Deliverables
1. **Precedent Research Documentation**  
   - Annotated summary of existing animatronics and relevant AI/ML approaches.
2. **MVP Puppet CAD & Mechanical Assembly**  
   - 2D drawings, 3D models, BOM (Bill of Materials).
3. **Data & AI Model**  
   - Recorded motion dataset, trained model files, and training scripts.
4. **Hardware-Software Control System**  
   - Source code for microcontroller/PC, wiring diagrams, servo/actuator controllers.
5. **Testing & Validation Reports**  
   - Mechanical stress checks, AI motion accuracy, overall reliability.
6. **Final Demonstration**  
   - Video or live demonstration of AI-driven puppet responding to user inputs or simulated conditions.

---

## 8. Acceptance Criteria
1. **Comprehensive Research**  
   - Clear documentation on how existing systems influenced design decisions.
2. **Functional MVP**  
   - Puppet exhibits at least one or two distinct AI-generated motions with smooth, stable actuation.
3. **Real-Time or Near Real-Time Control**  
   - Low-latency response (sub-200ms) for interactive or sensor-driven motions.
4. **Modular & Scalable Design**  
   - Mechanical rig and codebase are extensible to more axes or additional puppets.
5. **Demonstrated Reliability**  
   - Sustains repeated cycles without servo burnouts or mechanical failure.

---

## 9. Roles & Responsibilities
- **Research Lead**:  
  - Conducts the precedent and market research, produces summary documents.
- **Mechanical Engineer / Designer**:  
  - Oversees CAD design, mechanical fabrication, and system assembly.
- **AI/ML Engineer**:  
  - Handles data collection, model training, real-time inference integration.
- **Software Developer / Control Engineer**:  
  - Implements firmware, user interface, and orchestrates data flow between AI and hardware.
- **Project Manager**:  
  - Coordinates schedules, manages resources, ensures deliverables align with milestones.

---

## 10. Budget & Resources
- **Hardware Costs**  
  - Servo motors (1–2), microcontroller, 3D printing materials, sensors.  
  - Optional expansions for advanced features (e.g., multi-axis linkages, extra sensors).
- **Software & Tools**  
  - Autodesk Inventor (or similar CAD), open-source AI libraries (PyTorch, TensorFlow).  
  - License fees if specialized software for advanced simulation is needed.
- **Labor / Consulting**  
  - Time for research, mechanical design, AI development, and project management.
- **Contingency**  
  - Spare funds for unforeseen hardware replacements or additional prototypes.

---

## 11. Conclusion
By integrating **in-depth research on existing animatronic and robotics systems** with a **targeted MVP** approach, this project will deliver a foundational AI-driven puppet. The combination of mechanical prototyping, lightweight AI motion generation, and real-time control aims to demonstrate **proof of concept** while remaining flexible for future scaling. This approach preserves traditional puppetry’s artistic essence while introducing innovative, interactive capabilities—paving the way for **AI-enhanced performances** of increasingly complex and culturally significant puppets (e.g., Javanese shadow puppets).

**End of Scope of Work**
