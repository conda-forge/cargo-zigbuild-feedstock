About cargo-zigbuild-feedstock
==============================

Feedstock license: [BSD-3-Clause](https://github.com/conda-forge/cargo-zigbuild-feedstock/blob/main/LICENSE.txt)

Home: https://github.com/rust-cross/cargo-zigbuild

Package license: MIT

Summary: Compile Cargo project with zig as linker

Development: https://github.com/rust-cross/cargo-zigbuild

Compile Cargo project with zig as linker for easier cross compiling.

Current build status
====================


<table>
    
  <tr>
    <td>Azure</td>
    <td>
      <details>
        <summary>
          <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=26230&branchName=main">
            <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/cargo-zigbuild-feedstock?branchName=main">
          </a>
        </summary>
        <table>
          <thead><tr><th>Variant</th><th>Status</th></tr></thead>
          <tbody><tr>
              <td>linux_64</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=26230&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/cargo-zigbuild-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_64_" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_aarch64</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=26230&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/cargo-zigbuild-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_aarch64_" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>osx_64</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=26230&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/cargo-zigbuild-feedstock?branchName=main&jobName=osx&configuration=osx%20osx_64_" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>osx_arm64</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=26230&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/cargo-zigbuild-feedstock?branchName=main&jobName=osx&configuration=osx%20osx_arm64_" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=26230&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/cargo-zigbuild-feedstock?branchName=main&jobName=win&configuration=win%20win_64_" alt="variant">
                </a>
              </td>
            </tr>
          </tbody>
        </table>
      </details>
    </td>
  </tr>
</table>

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-cargo--zigbuild-green.svg)](https://anaconda.org/conda-forge/cargo-zigbuild) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/cargo-zigbuild.svg)](https://anaconda.org/conda-forge/cargo-zigbuild) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/cargo-zigbuild.svg)](https://anaconda.org/conda-forge/cargo-zigbuild) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/cargo-zigbuild.svg)](https://anaconda.org/conda-forge/cargo-zigbuild) |

Installing cargo-zigbuild
=========================

Installing `cargo-zigbuild` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:

```
conda config --add channels conda-forge
conda config --set channel_priority strict
```

Once the `conda-forge` channel has been enabled, `cargo-zigbuild` can be installed with `conda`:

```
conda install cargo-zigbuild
```

or with `mamba`:

```
mamba install cargo-zigbuild
```

It is possible to list all of the versions of `cargo-zigbuild` available on your platform with `conda`:

```
conda search cargo-zigbuild --channel conda-forge
```

or with `mamba`:

```
mamba search cargo-zigbuild --channel conda-forge
```

Alternatively, `mamba repoquery` may provide more information:

```
# Search all versions available on your platform:
mamba repoquery search cargo-zigbuild --channel conda-forge

# List packages depending on `cargo-zigbuild`:
mamba repoquery whoneeds cargo-zigbuild --channel conda-forge

# List dependencies of `cargo-zigbuild`:
mamba repoquery depends cargo-zigbuild --channel conda-forge
```


About conda-forge
=================

[![Powered by
NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org)

conda-forge is a community-led conda channel of installable packages.
In order to provide high-quality builds, the process has been automated into the
conda-forge GitHub organization. The conda-forge organization contains one repository
for each of the installable packages. Such a repository is known as a *feedstock*.

A feedstock is made up of a conda recipe (the instructions on what and how to build
the package) and the necessary configurations for automatic building using freely
available continuous integration services. Thanks to the awesome service provided by
[Azure](https://azure.microsoft.com/en-us/services/devops/), [GitHub](https://github.com/),
[CircleCI](https://circleci.com/), [AppVeyor](https://www.appveyor.com/),
[Drone](https://cloud.drone.io/welcome), and [TravisCI](https://travis-ci.com/)
it is possible to build and upload installable packages to the
[conda-forge](https://anaconda.org/conda-forge) [anaconda.org](https://anaconda.org/)
channel for Linux, Windows and OSX respectively.

To manage the continuous integration and simplify feedstock maintenance
[conda-smithy](https://github.com/conda-forge/conda-smithy) has been developed.
Using the ``conda-forge.yml`` within this repository, it is possible to re-render all of
this feedstock's supporting files (e.g. the CI configuration files) with ``conda smithy rerender``.

For more information please check the [conda-forge documentation](https://conda-forge.org/docs/).

Terminology
===========

**feedstock** - the conda recipe (raw material), supporting scripts and CI configuration.

**conda-smithy** - the tool which helps orchestrate the feedstock.
                   Its primary use is in the construction of the CI ``.yml`` files
                   and simplify the management of *many* feedstocks.

**conda-forge** - the place where the feedstock and smithy live and work to
                  produce the finished article (built conda distributions)


Updating cargo-zigbuild-feedstock
=================================

If you would like to improve the cargo-zigbuild recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`conda-forge` channel, whereupon the built conda packages will be available for
everybody to install and use from the `conda-forge` channel.
Note that all branches in the conda-forge/cargo-zigbuild-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@messense](https://github.com/messense/)
* [@ruben-arts](https://github.com/ruben-arts/)

