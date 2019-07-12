# SciPy Day 3
12 July 2019

Is it the year of stream-of-concious keynotes?

## Jupyter: ALways Open for Learning and Discovery
Carol Willing
	
	- "WebAssembly is up and coming" - what is WebAssembly?

### Resources

	- Ten Simply Rules for Reproducable Research in Jupyter Notebooks

## Raiders of the Pottery GAN: Using 3D Denerative Adversarial Networks for Data Augmentation in Archeological Studies
Celia Cintas

## Cupy: A NumPy-Compatible Library for High Performance Computing with GPU
Masayuki Takagi

	- Can directly replace `numpy` operations with `cupy`, making code run on GPUs up to 10x faster
	- If don't have access to GPUs, can try out on Google Colaboratory

### Resources
	- `pomegrenate` is a probabilistic and graphical modeling package that uses cupy

## How to Accelerate an Existing Codebase with Numba
Stanly Seibert

One of best talks so far

	- jit: Just In Time compiler
		- Used by Numba on individual function with decorator `@jit(nopython=True)
	- Numba good for bit manipulation
	- Comparing Cupy-Numba-Cython:
		- Cython translates to C++, where you can inpect it
		- Numba goes directly to the machine level, with no in-between C
		- Cupy is for when you have GPUs
	- Unit tests: did I break it?
	- Performance tests: did I make it faster?
	- Use object mode for i/o and callbacks (progress bars)
	- Numpy arrays best for Numba
	- Loops perform just as fast as array functions

### Resources
	- `cprofile` and `line_profile` + `SnakeVIZ`
		- Find time spent in each function graphically
