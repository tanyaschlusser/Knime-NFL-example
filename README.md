# Knime NFL example

This repo contains a Knime Analytics workflow that implements a Bayesian
updating scheme to predict game outcomes in the National Football League.

It accompanies a
[blog post](https://tanyaschlusser.github.io/posts/whats-so-great-about-knime/)
describing Knime Analytics (using version 3.6.6).

You may prefer downloading the zipfile containing the Knime workflow
[NFL.knwf](https://tanyaschlusser.github.io/posts/whats-so-great-about-knime/NFL.knwf)
instead.

## Opinion

The value of revision control is lost in this approach, because all
of the Python code is zipped up inside of their respective nodes
and you can't easily diff.

There is actually useful revision control in Knime Server since
[version 3.8 (announcement video)](https://www.youtube.com/watch?v=XewYe39heAE)
(currently 4.7.3) so enterprise users can access this feature without
lame jumping-jacks and should not use a Git repo, in my opinion.
This is just for example in case you really want it.
The useful part, the `.gitignore` file, was first written down
in this
[forum post](https://forum.knime.com/t/using-git-or-another-revision-control-system-for-knime-workflows/7246/5).

## Usage

### Python environment

You will need to install the
following libraries in a `virtualenv` or a `conda` environment to use
the workflow.

- NumPy 1.15.1
- Pandas 0.23.4
- requests 2.19.1
- lxml 4.2.4

Link to the environment you made by navigating to 

<blockquote>
KNIME → Preferences → KNIME → Python
</blockquote>

and browsing to the path for your new environment.
On a Mac depending on how you installed Python and whether you use
Anaconda or virtualenvwrapper, they might be in:

- `~/.virtualenvs`
- `~/miniconda3`
- `~/Anaconda3`

### Knime

You will need [Knime Analytics (download)](https://www.knime.com/downloads).
Open it after cloning this directory. If you wish, move this whole directory
(or the downloaded [NFL.knwf](https://tanyaschlusser.github.io/posts/whats-so-great-about-knime/NFL.knwf))
inside your Knime workspace directory, which in my case is `~/knime-workspace`.

Then go to 

<blockquote>
File → Import Knime Workflow
</blockquote>

and in the window that pops up 

- If you are using this git repo, choose `Select root directory:` then click `Browse` and navigate to where
  you pulled this git repo `Knime-NFL-Example`
- If you are using [NFL.knwf](https://tanyaschlusser.github.io/posts/whats-so-great-about-knime/NFL.knwf),
  choose `Select file:` then click `Browse` and navigate to where you downloaded `NFL.knwf`

Then open the file. Woo!
See [my blog post](https://tanyaschlusser.github.io/posts/whats-so-great-about-knime/)
for more details.
