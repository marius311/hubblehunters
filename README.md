# The Hubble Hunters Guide

This repo contains the code to make the two plots from [The Hubble Hunter's Guide](link-TBD). 

### Requirements

* Julia 1.1+
* Python 3.6+
* gfortran

*Note:* [Cosmology.jl](https://github.com/marius311/Cosmology.jl) (which is a dependency that is automatically installed if you follow the instructions below) needs to compile a [single Fortran file](https://github.com/marius311/Cosmology.jl/blob/ac971e7b3e6e87a538934020f9c880bea3ce53ad/deps/build.jl#L11); this has only been tested on Linux. 

### Instructions

```bash
git clone https://github.com/marius311/hubblehunters
cd hubblehunters
```
Then install Julia dependencies via:
```bash
julia --project=@. -e "using Pkg; Pkg.instantiate()"
```
and Python dependencies via:
```bash
pip install -r requirements.txt
```

Then run JupyterLab or Jupyter Notebook and open and run the two notebooks included. 

*Note:* The Julia dependencies are installed in the environment in the `hubblehunters` folder. If for whatever reason this environment is not activated, make sure to do `Pkg.activate("/path/to/hubblehunters")`.
