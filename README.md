# Dry-Etching-Profile-Simulation 
Objective
 Theobjective of this project is to simulate the evolution of etch profiles in microfabrication
 using dry etching techniques. Specifically, the simulation compares:
 • Anisotropic dry etching, where material is etched primarily in the vertical di
rection.
 • Isotropic dry etching, where material is removed equally in all directions.
 The project involves implementing both processes in MATLAB, generating visual profiles
 over multiple etch steps, and creating animations to visualize trench evolution. The goal
 is to understand the differences in etch behavior and resulting geometry under each
 condition.
 Background Theory
 In semiconductor fabrication, etching is a process used to selectively remove material
 from the wafer surface to form devices and circuits. There are two broad classes:
 • Wet etching (using liquid chemicals)
 • Dry etching (using plasma or gas-phase reactions)
 This project focuses on dry etching, which uses plasma to remove material more pre
cisely. Depending on the directionality of etching, dry etching can be:
 • Anisotropic: Directional etching, primarily vertical, due to ion bombardment.
 • Isotropic: Uniform etching in all directions, due to chemical diffusion.
 Etch profile geometry plays a critical role in determining device dimensions, functionality,
 and yield.
 Simulation Methodology
 A2Dsimulation is performed on a square grid representing a material block with a mask
 layer on top.
 • The grid values represent:– 0: Etched (air/vacuum)– 1: Material (e.g., silicon)– 2: Mask (photoresist/hardmask)
 • Amask opening is created in the center of the top row.
 • For each time step:– In anisotropic etching, material is removed only if the pixel above is air.– In isotropic etching, material is removed if any of the 4 neighbors is air.
 1
• Each step is saved as an image. After 90 steps, these frames are compiled into mp4
 movies.
 Results and Discussion
 The following visualizations and movies show the trench profiles after 90 steps of etching.
 Anisotropic Etching Profile
 Figure 1: Final etch profile after 89 steps — Anisotropic
 • The trench profile is narrow with vertical sidewalls.
 • Etching occurs only in the vertical direction under the mask opening.
 • No lateral undercut is observed.
 Isotropic Etching Profile
 • The profile expands sideways with rounded sidewalls.
 • Etching spreads laterally beneath the mask visible undercutting.
 • Matches real-world isotropic behavior caused by chemical species.
 Simulation
 Both etching processes were simulated over 90 steps and exported as animation videos:
 • anisotropic
 • isotropic
 etching.mp4
 etching.mp4
 2
Figure 2: Final etch profile after 89 steps — Isotropic
 To watch the anisotropic etching simulation, please click here.
 To watch the isotropic etching simulation, please click here.
 Conclusion
 This project successfully simulates the evolution of etch profiles in dry etching for both
 anisotropic and isotropic cases using MATLAB. The results match expected physical
 behavior:
 • Anisotropic etching results in straight, vertical trenches.
 • Isotropic etching results in rounded and undercut profiles.
 This simulation highlights the importance of etching directionality in semiconductor man
ufacturing and helps visualize microscopic process effects at a macro level
