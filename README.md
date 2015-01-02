amr_project
===========

numerical methods for PDEs final project, Columbia University, fall 2014


Scripts for running the project are in the myclaw directory.
- run_param_sweep.py and variants to make the runs
- parse_runs.py to read in the data and make plots
Requires clawpack (http://www.clawpack.org/index.html) be installed to run everything.

eluer_base and advection_base directories hold the base forms for the two problems that 
run_param_sweep.py copies from and modifies.

parse_runs.py is set up to store the parsed data using python's pickle module, and thus
can be set to read data from those files rather than reading in directly from the files
output by the runs (which can take some time). Unfortunately the script currently just
saves the plots to the directory it's in, which is somewhat messy, though this wouldn't
be hard to change.

Code in setplot.py in each problem for plotting refinement criteria and refined regions
was provided by Professor Kyle Mandli.
