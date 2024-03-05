# JHU Computing Club: Parallelism and GPUs

This repository includes material for the 2024/03/05 talk at the JHU Computing Club. In particular, it
includes the material on parallelism using R or [SLURM](https://slurm.schedmd.com/) at [JHPCE](https://jhpce.jhu.edu/). See the [Google Slides](https://docs.google.com/presentation/d/1gJzrL1E3EJRQEzbvg8t1rGNM6GsrKU42QoPo-ykKhH0/edit?usp=sharing) for the remaining material on using and understanding GPU resources at JHPCE.

## All Talk Materials

- [Slides on GPUs](https://docs.google.com/presentation/d/1gJzrL1E3EJRQEzbvg8t1rGNM6GsrKU42QoPo-ykKhH0/edit?usp=sharing)
- [Parallelism Vignette](https://nick-eagles.github.io/JHU_parallelism_and_gpus/)
- [JHPCE GPU Documentation](https://jhpce.jhu.edu/knowledge-base/gpus-on-the-jhpce-cluster/)


## Parallelism in R

First, I cover the `BiocParallel` R package for making use of multiple CPUs cores on Linux-like
machines, including those at JHPCE. The [raw R markdown file](index.Rmd) is available, but I encourage you to follow along with the [rendered HMTL](https://nick-eagles.github.io/JHU_parallelism_and_gpus/). I also conceptually introduce array jobs.

## Parallelism by Array Job

Next, the `nnSVG` array job [shell script](nnSVG_array.sh) and [R script](nnSVG_array.R) show
a practical case where parallelism can be achieved by dividing the data into units and assigning
each unit an array task with one CPU. I'll interactively walk through these scripts.
