# Knime NFL example

This repo contains a Knime Analytics workflow that implements a Bayesian
updating scheme to predict game outcomes in the National Football League.

It accompanies a
[blog post](https://tanyaschlusser.github.io/posts/whats-so-great-about-knime/)
describing Knime Analytics (using version 3.6.6).

You may prefer downloading the zipfile containing the Knime workflow
[NFL.knwf](https://tanyaschlusser.github.io/posts/whats-so-great-about-knime/NFL.knwf)
instead.


## Usage

### Python environment

You will need to install the
following libraries in a `virtualenv` or a `conda` environment to use
the workflow.

- NumPy 1.15.1
- Pandas 0.23.4
- requests 2.19.1

Link to the environment you made by navigating to 

<blockquote>
KNIME → Preferences → KNIME → Python
</blockquote>

and browsing to the path for your new environment.
On a mac depending on how you installed Python and whether you use
Anaconda or virtualenvwrapper, they might be in:

- `~/.virtualenvs`
- `~/miniconda3`
- `~/Anaconda3`

### Knime

You will need [Knime Analytics (download)](https://www.knime.com/downloads).
Open it after cloning this directory, and move

## Opinion

The value of revision control is lost in this method, because all
of the Python code is zipped up inside of their respective nodes.

There is actually useful revision control in Knime Server since
[version 3.8 (announcement video)](https://www.youtube.com/watch?v=XewYe39heAE)
(currently 4.7.3) so enterprise users can access this feature without
lame jumping-jacks and should not use a Git repo, in my opinion.
This is just for exmaple.
