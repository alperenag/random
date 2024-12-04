# Status  

`Valid`

# Project Description

This study aims to deliver the center of gravity and moment of inertia matrix for PT1 and establish a straightforward method for calculating the new center of gravity and moment of inertia for the drone when additional mass is added, namely payload. Accurate determination of these parameters is essential for evaluating stability and maneuverability, particularly when modifications like adding payloads or new components are made.

# Methodology 
The process involves five main steps:

1. Determine the New CG:

Calculate the weighted average of the original CG and the position of the added mass.
Adjust the Original Moment of Inertia:

Shift the original moment of inertia matrix to the new CG using the parallel axis theorem.
Add the Effect of the New Mass:

Treat the new mass as a point load to compute its contribution to the moment of inertia relative to the new CG.
Combine this with the adjusted original moment of inertia matrix to get the updated values.
- Ease of manufacturing, specifically through 3D printing
- Durability for repeated use
- Protection of aircraft components by absorbing the energy from landing impacts
- Compatibility with the existing landing legs, avoiding the need to replace them or develop additional systems.

The optimal design for a basic landing gear involves creating it as a single component, where the gear itself functions as the shock absorber. The material must be compatible with most 3D printers on the market and possess a degree of flexibility to ensure it effectively absorbs impact energy. The design should achieve an ideal balance of stiffness to compress under the testbed’s landing loads at maximum takeoff weight (MTOW), while remaining structurally sound when supporting the MTOW on the ground. 

The strength of 3D-printed parts is influenced by various factors, such as the type of printer, slicing software, print settings, and the condition of the filament, which makes FEA unreliable and misleading in this case. In addition, performing a dedicated structural test would require specialized equipment and a complex test setup, making it both expensive and time-consuming. As a result, the model will be tested directly on the aircraft, with iterative adjustments made based on its performance during real-world use.

# Results and Deliverables

TPU (Thermoplastic Polyurethane) was chosen as the primary material due to its excellent elastic properties and durability. Unlike more rigid materials like PLA, TPU provides flexibility that helps absorb impact energy, making it ideal for applications involving shock absorption such as landing gear.

TPU's elasticity ensures that the landing gear can deform under load and then return to its original shape, minimizing the risk of structural damage and enhancing the longevity of the components during repeated use.

The CAD design is created using Fusion 360. It consists of 6 angular tubes that are acting as shock absorbers, a bottom plate to prevent the tubes to be bent more than intended, and a tube on top that will wrap the testbed landing legs. The landing gear is installed on the landing leg using four M5 bolts. Each bolt needs to be longer than 55 mm, with a thread coverage of at least 25 mm. The nuts should be locknuts to ensure they remain secure and do not loosen due to vibration.

![Alt text](aaa.PNG)

The model is printed on a Bambu Lab X1-Carbon Combo 3D printer. One landing gear is used per landing leg, making 4 in total. The design is used for multiple flight tests, and no damage on the landing gear is observed. During the flight tests, the landing gear proved to be successful for absorbing the landing loads.

The landing gear design: https://a360.co/4dwC8Na

# Remarks
- The decision to use TPU for the landing gear was crucial to enhancing its shock absorption and resilience. The material’s flexibility provides a distinct advantage over rigid options like PLA or ABS, especially in applications where energy absorption is key to preventing damage.
- While the single body landing gear system worked effectively in this case, further refinements in the design may help maximize its energy-absorbing potential and strength, such as incorporating different materials for the installation area or thickness variations that enhance deformation in critical areas during impact.
- Initial testing has shown promising results, but additional real-world testing is recommended to assess the long-term performance of TPU under varying environmental conditions and repeated landings.
