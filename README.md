# solar-model

A Solar system planetary motion simulation project in Java.

#### Prerequisites:
 - Java - to run the code;
 - VMD - to visualise the solar system. You can download VMD from [here](http://www.ks.uiuc.edu/Research/vmd/). 

#### Running the code:

 - Compile ParticleManyBody, Particle3D and Vector3D
 - Run "java ParticleManyBody particle.input param.input traj.xyz"

#### Config files:

 - particle.input contains positions and velocities of Solar system objects, taken from [NASA/JPL HORIZONS system](http://ssd.jpl.nasa.gov/horizons.cgi). 2016-03-05 snapshot of the Solar system was used to make this file.
 - param.input contains the number of iterations, timestep length in Earth days and the gravitational constant in units of AU^2^ E~mass~^-1^ E~day~^-2^ units. The file contains "365, 1, 8.89e-10" by default.

#### Visualising the system:
If you have VMD installed, you can run "vmd traj.xyz" to visualise and animate the solar system. Be sure to change the drawing method to "Points" by clicking Graphics -> Representations... -> Draw Style -> Drawing Method and increase the size until you can see the points. The simulation can be played by clicking the ▶ button on the VMD Main window.

You can also see the orbits of planets by typing in a range (e.g. 0:365) at Graphics -> Representations... -> Trajectory -> Draw Multiple Frames and pressing enter.
