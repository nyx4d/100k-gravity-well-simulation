100k-gravity-well-simulation

**ES5 Particle System: A Simulation of Cosmic Dynamics**

This project is a simulation of cosmic dynamics interactive particle system inspired by real-world wave-particle dynamics and gravitational fields. Using Three.js in ES5, the simulation renders 100,000 particles moving in a 3D space, where their behavior mimics the interaction of particles with a localized gravitational source (gravity well). This project explores the beauty of emergent behavior in simple systems and the analogies between programming and natural phenomena.
Inspiration

The particle system draws inspiration from:

    Electromagnetic Wave Behavior: Particles move fluidly, creating patterns reminiscent of charged particles interacting with oscillating fields.
    Gravitational Wells: The central concept mirrors how massive celestial objects like stars or black holes create gravitational forces that influence surrounding matter.
    Cosmic Plasma Dynamics: The simulation echoes the chaotic yet harmonic behavior of particles in plasma fields, where they are both attracted and repelled by forces.

Real-World Analogy

Think of the particle system as:

    Auroras: Particles’ vibrant, shifting colors and movements resemble the auroras created when solar wind interacts with Earth's magnetic field.
    Gravity-Induced Particle Flows: Similar to how debris or gases swirl and accelerate when approaching a celestial object like a planet or black hole.

Mathematical Foundation
The Gravity Well Formula

The gravity well effect is driven by a simplified inverse-square law formula:

F=1d2F=d21​

Where:

    FF: Force applied to a particle.
    dd: Distance between the particle and the center of the gravity well.

Breakdown:

    Direction Vector: For each particle, the vector from its current position to the gravity well center is calculated:
    dx=xgravity−xparticle
    dx=xgravity​−xparticle​
    dy=ygravity−yparticle
    dy=ygravity​−yparticle​
    dz=zgravity−zparticle
    dz=zgravity​−zparticle​

    Distance Calculation: The Euclidean distance between the particle and the gravity well is derived as:
    d=dx2+dy2+dz2
    d=dx2+dy2+dz2

    ​

    Force Calculation: A force proportional to 1d2d21​ is applied, simulating gravitational pull:
    F=kd2
    F=d2k​

    Here, kk is a scaling factor.

    Velocity Update: The particle’s velocity is adjusted based on this force:
    vx+=dx⋅F
    vx​+=dx⋅F
    vy+=dy⋅F
    vy​+=dy⋅F
    vz+=dz⋅F
    vz​+=dz⋅F

Particle Behavior

Each particle has:

    Randomized Initial Velocity: Creates diverse trajectories.
    Randomized Initial Position: Ensures the particles are distributed evenly in a cube-like region.
    Dynamic Motion: Velocities are continuously updated, resulting in fluid, wave-like movement.

When a gravity well is active:

    Particles accelerate toward it, creating swirls and patterns that emulate a real gravitational pull.
    Close particles exhibit rapid, chaotic motion, while distant particles gently drift inward.

Features

    Massive Particle Count: Efficiently renders 100,000 particles using Three.js BufferGeometry.
    Dynamic Forces: Real-time gravity well simulation influenced by user input.
    Realistic Motion: Particles behave like small celestial objects influenced by gravity.
    Vibrant Visualization: Randomized colors bring the simulation to life.

Real-World Comparisons

This simulation aligns conceptually with:

    Gravity Well Dynamics: Similar to how planets orbit stars, the particles’ trajectories reflect gravitational pull in a localized field.
    Electromagnetic Waves: The system creates wave-like ripples as particles realign themselves dynamically.
    Plasma and Charged Particles: The chaotic, swirling motion resembles plasma fields in space or laboratory experiments.

How to Run

    Clone the repository:

    git clone https://github.com/nyx4d/100k-gravity-well-simulation.git
    cd 100k-gravity-well-simulation

    Open index.html in your browser or use a local server for WebGL compatibility.

    Move your mouse to create a gravity well and observe the particles’ reactions in real time.

Customization
Key Variables

    particleCount: Increase or decrease the number of particles to control the density of the system.
    velocityMultiplier: Adjust the speed of particles.
    gravityStrength: Change the intensity of the gravity well effect.

Ideas for Extensions

    Particle Trails: Leave a fading trail behind each particle to visualize motion history.
    3D Camera Controls: Add orbit or pan controls for a more interactive experience.
    Dynamic Gravity Wells: Allow multiple gravity wells to exist simultaneously.

Acknowledgments

This project was inspired by:

    Physics Simulations: Simplified gravitational models and charged particle dynamics.
    Three.js Documentation: A fantastic resource for building interactive 3D experiences.
    chatGPT-4o and openai for assisting in my educational journy and bringing my my visusals to life. my curiosities and hel

Special thanks to everyone exploring the intersection of physics and programming.
About the Author

👩‍💻 Rachel Nyx
GitHub: @nyx4d
Contact: nyx4d@proton.me

Rachel is passionate about visualizing complex systems and bringing cosmic-inspired designs to life through programming. This project is part of her journey to merge creativity with computational exploration.
