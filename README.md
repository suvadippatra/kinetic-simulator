Physics of Kinetic Patterns
Welcome to the laboratory of kinetic optical illusions. This simulation models the interference patterns created by two counter-rotating radial gratings, a phenomenon known as the Moiré Effect.

1. The Moiré Interference Principle
When two repetitive patterns overlap, they create a third, new pattern called a "superposition" or Moiré pattern. In this sculpture, the two wheels are essentially identical but one is mirrored.

As they rotate, the intersection points of the spokes travel along specific loci. Because the wheels rotate in opposite directions (Counter-Rotation), the human eye tracks these intersection points rather than the spokes themselves.

Visual Frequency ≈ | f1 - f2 |
Where f1 and f2 are the spatial frequencies of the two wheels. Small differences in angle create large shifts in the visual pattern, generating the illusion of "swelling" or "breathing."

2. Role of Geometry
The specific "shape" of the illusion depends entirely on the spoke geometry (which you can change in the top menu):

Logarithmic Curves (Dimensions): Create the illusion of 3D depth (a Torus) because the intersection points move radially inward/outward at non-linear speeds.
Sine Waves (Infinity): Create a flowing "waterfall" effect. The intersections move vertically, mimicking fluid dynamics.
Radial Lines (Starburst): Create a "shimmering" or "heat haze" effect. The intersections are purely rotational, causing angular aliasing.
3. Dynamics & Damping
The sliders below control the physical forces acting on the wheels. In the real world, these sculptures are powered by negator springs and slowed by air resistance.

Velocity (Torque): This represents the energy input. Setting opposite signs (e.g., +0.5 and -0.5) maximizes the interference effect.
Damping (Coefficient $\gamma$): This simulates friction.
v_{new} = v_{old} - (v_{old} \times \gamma)
If Damping is 0.0, the wheel spins perpetually (ideal motor). If Damping is high, the wheel acts like it is submerged in water, losing energy rapidly. This allows for "coast" effects where you spin it up and watch it slowly die down.
Experiment: Set Damping to 0.005, fling the velocity slider to max, then release it to 0. Watch the wheel slowly drift to a halt.

Design Spoke Geometry to Mimic Natural Radial Rhythms
You can design spoke geometry and time-modulation to mimic specific biological or physical objects that naturally move in a radial rhythm. Use the Presets panel to try these quickly.

Jellyfish / Squid: Use the "Infinity" style with constrained amplitude and an automated pulse (slight radial scaling) to create a bell-shaped spoke that pulses open/closed like a swimming jellyfish.
Blossoming Flowers: Use a broader logarithmic-curved "Dimensions" spoke and animate a widening phase — interference creates petal-like lobes that appear to open from the center.
Beating Heart: Add a controlled variance in spoke thickness (per spoke), driven by a shared beat-phase. The Moiré envelope then appears to swell and contract like a pulsing muscle.
3D Spheres & Donuts: The "Dimensions" model can produce shading/occlusion cues that look like a torus or sphere — this shows the system can render apparent 3D volumes, not just flat lines.
Eyes / Pupils: A dense radial spoke set with a central dark pupil whose radius is modulated produces the illusion of an iris dilating and contracting.
3. How to achieve "Object" Motion (The Barrier Grid Alternative)
The barrier grid approach (also called 'parallax barrier' or slit-scanning) produces the perception of object motion by sampling a dynamic pattern through a moving slit-mask. Key points:

Render the interference pattern to an offscreen buffer.
Apply a moving mask of opaque and transparent slits across the buffer (the "barrier").
When the slit-mask translates or oscillates at the right speed relative to the pattern, the brain integrates the sampled frames into a coherent object-like motion (apparent translation or depth sweep).
In this demo you can toggle the Barrier Grid option and combine it with the presets to observe how object-like motion emerges without physically moving an object — the slits do the work.

References & Research
David C. Roy Official Site (Primary Artist)
Dimensions Sculpture Manual (PDF)
Research: The perception of dynamic Glass patterns
Paper: Motion integration in Moiré patterns
