######### Important Note #########
Here is how to get the file working, as it uses a few packages.
	1. Navigate to your directory of the ising model.
	2. Open your terminal.
	3. in your terminal, run '$pip install -r requirements.txt'
	4. in your terminal, run the file by using '$python3 main.py'
	5. to close the script, simply close the window.
	6. Enjoy! ( :

######## Description #########
Here we present an ising model created using a network abstraction of the lattice. That means, we can compute everything using matrix multiplication, which, for sparse graphs, is both parallelizable and computationally efficient. 

For the moment, it has only been parallelized on the CPU, however, in the future I will parallelize the functions to be computed on the GPU, given that the latency is not too significant. 

As of now, the computational bottleneck is plotting using matplotlib: consequentially, if anyone has a faster way to plot in Python, please do let me know so we can get massive ising models! Moreover, networkX drawing is computationally inefficient, so, if anyone has a better implementation, I want to do some visualization for complex networks also! 

As of right now, on my PC with 16 cores I can easily handle 1000x1000 lattice (1 million nodes, being plotted every 5 time steps).

######### CHANGEABLE VARIABLES ##########
In the main.py file, there are a few variables that are modulateable:
	1. The temperature (normalized)
	2. The lattice size.
	3. The number of time steps between each matlotlib display.

More to come soon!

- By: Marcus Engsig
