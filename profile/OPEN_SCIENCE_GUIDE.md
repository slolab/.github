# How open source software works in academia (and how it doesn't)

At the basis of this guide is the recurrent observation of a mismatch between
the incentives that drive open source software development and the incentives
that drive academic work, as well as a desire to align the two to yield better
outcomes for individual researchers and the scientific community as a whole.

> [!NOTE]
> This guide is not complete, and contributions and discussion are very welcome.
> Go to the [Discussion](https://github.com/orgs/slolab/discussions/2) to chime
> in!

## Open source software in academia

Open source software is a cornerstone of modern scientific work. It allows
researchers to access and build upon each other's work, to automate repetitive
tasks, and to create tools that are not only useful but also accessible to
everyone. However, from the perspective of an individual researcher, the
academic credit they receive for their work is their main metric of success. In
consequence, many contributions to open source software do not happen, for
instance, because the researcher needs to focus on publishing their own work.
This very often results in the
[reinvention of the wheel](https://en.wikipedia.org/wiki/Reinventing_the_wheel#In_software_development).

## How we work

While there is no simple, clear-cut solution to this problem, there is no
alternative to approaching it with a desire to remove redundancies. To tackle
the issue systemically, the academic credit system needs to be changed to
account for the value of open source software contributions, particularly those
that are a large collaborative effort. This naturally is a slow process, which
requires practical solutions to be implemented in the meantime.

Here are some of the solutions we have found to be effective (but subtle and
sometimes tricky to implement):

### Increase reliance on existing software

This requires good knowledge of the existing software landscape, which takes
time to develop.

It also requires decisions: when is the existing software appropriate to use in
my case? Does it offer all the features I need? Is it maintained? Would I be
able to contribute to it if I am missing a feature? How will I receive credit
for my work in the academic system?

There are only few software projects that are so widely used that they fulfill
these criteria (for instance, [scikit-learn](https://scikit-learn.org/stable/)).
Still, these projects can also be superceded by more specialized or
methodologically different software (for instance, sklearn is not the best tool
for deep learning, which led to the development of
[PyTorch](https://pytorch.org/), [TensorFlow](https://www.tensorflow.org/), and
[JAX](https://jax.readthedocs.io/en/latest/)).

### Contributing smaller packages to an existing ecosystem

Contributing smaller packages to an existing ecosystem, which amortises
developments costs through providing a framework for development, is another
solution. They often provide guidelines, templates, and pre-made components for
development and testing. Scientific examples include
[PyOpenSci](https://pyopensci.org/),
[Bioconductor](https://www.bioconductor.org/), and
[scverse](https://scverse.org/).

### Using templates to get a head start

If you have a good idea for a software project, you are aware of the software
landscape, and you are sure that your idea is not already implemented, you can
use templates to get a prototype or proof of concept fast. Softwares like
[cookiecutter](https://cookiecutter.readthedocs.io/en/latest/) and
[copier](https://copier.readthedocs.io/en/stable/) are great tools to do this;
templates are provided by the community, for instance,
[PyOpenSci](https://github.com/pyOpenSci/pyos-package-template) and
[scverse](https://cookiecutter-scverse-instance.readthedocs.io/en/latest/template_usage.html).

### Sprints and hackathons

Sprints and hackathons are great ways to get started with open source software.
They provide a structured way to work on a project, with a clear goal and
deliverables. They also provide a way to network with other developers and
researchers, and to get feedback on your work. They do not require a large
investment of time, and they yield valuable insight even when they fail their
main goal.

In extension, sprints-like events can be used to test the feasibility of ideas
with little risk, evolve existing projects, drive very specific features, and
increase community engagement and visibility. The main requisite for applying
this process is a shift in mentality, from the traditional scientific project
(that is a long, involved, and often slow process) to a more agile and iterative
approach. Think of it as an analog of short-lived feature branches in software
development: the results of the sprint are merged back into the main research
project, which facilitates development and does not change the ultimate goal.
