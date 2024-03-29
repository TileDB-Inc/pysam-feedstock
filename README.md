About pysam-feedstock
=====================

Feedstock license: [BSD-3-Clause](https://github.com/TileDB-Inc/pysam-feedstock/blob/main/LICENSE.txt)

Home: https://github.com/pysam-developers/pysam

Package license: MIT

Summary: Pysam is a Python module for reading and manipulating SAM/BAM/VCF/BCF files. It's a lightweight wrapper of the htslib C-API, the same one that powers samtools, bcftools, and tabix.

Current build status
====================


<table>
    
  <tr>
    <td>Azure</td>
    <td>
      <details>
        <summary>
          <a href="https://dev.azure.com/TileDB-Inc/CI/_build/latest?definitionId=45&branchName=main">
            <img src="https://dev.azure.com/TileDB-Inc/CI/_apis/build/status/pysam-feedstock?branchName=main">
          </a>
        </summary>
        <table>
          <thead><tr><th>Variant</th><th>Status</th></tr></thead>
          <tbody><tr>
              <td>linux_64_libdeflate1.17</td>
              <td>
                <a href="https://dev.azure.com/TileDB-Inc/CI/_build/latest?definitionId=45&branchName=main">
                  <img src="https://dev.azure.com/TileDB-Inc/CI/_apis/build/status/pysam-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_64_libdeflate1.17" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_64_libdeflate1.18</td>
              <td>
                <a href="https://dev.azure.com/TileDB-Inc/CI/_build/latest?definitionId=45&branchName=main">
                  <img src="https://dev.azure.com/TileDB-Inc/CI/_apis/build/status/pysam-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_64_libdeflate1.18" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_64_libdeflate1.19</td>
              <td>
                <a href="https://dev.azure.com/TileDB-Inc/CI/_build/latest?definitionId=45&branchName=main">
                  <img src="https://dev.azure.com/TileDB-Inc/CI/_apis/build/status/pysam-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_64_libdeflate1.19" alt="variant">
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
| [![Conda Recipe](https://img.shields.io/badge/recipe-pysam-green.svg)](https://anaconda.org/tiledb/pysam) | [![Conda Downloads](https://img.shields.io/conda/dn/tiledb/pysam.svg)](https://anaconda.org/tiledb/pysam) | [![Conda Version](https://img.shields.io/conda/vn/tiledb/pysam.svg)](https://anaconda.org/tiledb/pysam) | [![Conda Platforms](https://img.shields.io/conda/pn/tiledb/pysam.svg)](https://anaconda.org/tiledb/pysam) |

Installing pysam
================

Installing `pysam` from the `tiledb` channel can be achieved by adding `tiledb` to your channels with:

```
conda config --add channels tiledb
conda config --set channel_priority strict
```

Once the `tiledb` channel has been enabled, `pysam` can be installed with `conda`:

```
conda install pysam
```

or with `mamba`:

```
mamba install pysam
```

It is possible to list all of the versions of `pysam` available on your platform with `conda`:

```
conda search pysam --channel tiledb
```

or with `mamba`:

```
mamba search pysam --channel tiledb
```

Alternatively, `mamba repoquery` may provide more information:

```
# Search all versions available on your platform:
mamba repoquery search pysam --channel tiledb

# List packages depending on `pysam`:
mamba repoquery whoneeds pysam --channel tiledb

# List dependencies of `pysam`:
mamba repoquery depends pysam --channel tiledb
```




Updating pysam-feedstock
========================

If you would like to improve the pysam recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`tiledb` channel, whereupon the built conda packages will be available for
everybody to install and use from the `tiledb` channel.
Note that all branches in the TileDB-Inc/pysam-feedstock are
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

* [@jdblischak](https://github.com/jdblischak/)
* [@shelnutt2](https://github.com/shelnutt2/)

