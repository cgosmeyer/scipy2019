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

## Invisible Work, Incentives, and Burnout in Open Communities
Dorothy Howard

## Work Open, Lead Open ($WOLO)
Abigail Mayes

	- Interesting open-the-mountain illustration of how to bring in and keep people in your community and bring them into leadership roles.
	- To keep people, show them how their work contributed to the community's goal. 
	- Align their interests/skills with tasks. 
	- Have a clear end-time for leadership roles. It should be something that gets "renewed" rather than something they step down from.

## Astropy Beyond Astronomy: Infrastrcutre of an Open Source Ecosystem
Brigitta Sipocz

	- Always the documentation self-back pats. 
	- What IS the problem with Astropy?  I think it is that most of the developers aren't the users who rely on it every day.

## Lightning Talks

	- Cat's Eyes are a way to express error bars
	- Should try plotting in Seaborn
	- `DataClass` is new in Python 3.7.  I might have used this instead of making data containers for my verification!
		- Requires optional typing.
	- signac - help with maintaining file-based workflows esp with HPC systems
		- maintained by computaional material scientists (github @bdice)
		- https://github.com/glotzerlab/signac
	- Pypy is fast Python, Python with a jit.

