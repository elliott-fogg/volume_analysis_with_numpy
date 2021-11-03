# volume_analysis_with_numpy
A small experiment I did for a colleague to workout a faster way of iterating through a slightly more complex NumPy array using NumPy functions to speed up analysis.

The input format is a NumPy array with 2 sub-arrays. The first sub-array is the time steps of an experiment. The second sub-array is an array of groups of coordinates for 
particles in the experiment. For each time step, there is a corresponding group that is an array of 3-dimensional coordinates.

The required analysis is calculating how many particles are within a given volume at each timestep, and then returning only those timesteps and particle-counts where the particle-count is nonzero.

In this notebook I show a way of processing the data using NumPy functions which is orders of magnitude faster for very large datasets.
