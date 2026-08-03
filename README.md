## About me
Hi, I am Physics graduate currently looking for PhDs in astrophysics with an emphasis in numerical modelling. I graduated from the University of Exeter in 2024 with a 1st class MPhys degree in Physics with Astrophysics. I have a broad range of interests including mathematics such as abstract algebra, topology, and order theory and physics such as mechanics and fluid dynamics. I code predominately code in Python although I have been known to dabble in C and HTML.

University Projects:
1. (MPhys Final Project) Forming Diverse Planets by Pebble Accretion:
	*Context* Planets are formed from material leftover from star formation, but the processes through which a 'planetary embryo' grows into a fully fledged planet are still uncertain. One process capable of forming planetary cores is pebble accretion, the aeryodynamically assisted accumulation of pebble-sized solids by a planetary embryo.
	*Aims* In this project, we seek to model the growth of proto-planets through pebble accretion in order to suggest some of the conditions an early solar system would require to be able to develop giant planets.
	*Methods* We combine pebble accretion with two other processes: planetary migration and gas accretion to build a versatile model of planetary growth. In Python, we use the foward Euler method with an adaptive timestep to integrate both the position and mass of the planet with respect to time. 
	*Results* Growth is highly dependent on the orbital radius of the embryo, and the largest planets develop outside the inner solar system before migrating inwards. Our model was able to form giant planets in early solar systems with moderate amounts of dust - more than estimated in real exoplanet systems, but less than needed to form giant planets in other models.
2. (Computational Physics Module Final Project) Trajectory of a Particle in The Vicinity of a Black Hole
	*Context* The spacetime surrounding a black hole is warped, and this distortion increases approaching the event horizon. In the case that the black hole is non-rotating, the Schwarzschild metric describes the curvature of the spacetime, and in combination with a set of equations called the geodesic equations, it can be used to forecast the trajectory of a particle through spacetime. 
	*Aims* In this project, we seek to model a particle of negligable mass in the vicinity of a black hole. We then compare the behaviour of our model to the analytical solution in different limiting scenarios. 
	*Methods* We limit the degrees of freedom of the particle without loss of generality and use a SciPy adaptive solver to compute its trajectory over a specified time interval. 
	*Results* The simulation showed expected behaviour: Precessing elliptical orbits, Keplerian circular orbits in the far-field limit, and the radial infall of initially stationary particles. The simulation performed best when using a fifth order implicit Runge Kutta method of the Radau-family, the SciPy Radau method, as opposed to explicit methods, implying this is a stiff set of equations.

Recently, I've been experimenting in Python modelling 2D anisotropic Harmonic Oscillators. These are systems which obey an equation of motion of the form: 

$$m\ddot{x}(t) + B\dot{x}(t)+K[x(t) - x_\text{eq}] = \vec{F}(t)$$

where $x(t)$, $\dot{x}(t)$, and $\ddot{x}(t)$ are respectively the position, velocity, and acceleration of the oscillator, $m$ is its scalar mass, $B$ and $K$ are positive semi-definite linear operators which are the damping and restoring coefficients respectively, and $\vec{F}(t)$ is the external force on the oscillator at time $t$. 

An example trajectory: 

<img width="640" height="480" alt="DampedAnisotropicOscillator" src="https://github.com/user-attachments/assets/85f57ad4-02d8-4165-b0a2-2c34b9282330" />
