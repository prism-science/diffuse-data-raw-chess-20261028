# Raw data: CHESS beamtime 20261028

**Logbook entry: <https://diffuse.science/logbook/beamtime/20261028-chess/>**

This repository catalogs the raw data from one beamtime of [The Diffuse Project](https://prismscience.org/science/accelerating-dynamic-data-collection#diffuse-scattering) at beamline ID7B2 of the Cornell High Energy Synchrotron Source (CHESS). The logbook entry above describes the samples, the experiments, and the data processing results. Entries for all beamtimes are in the [logbook](https://diffuse.science/logbook/beamtime).

It is a [DataLad](https://www.datalad.org) dataset. Git holds the directory tree and file checksums. The file contents are tracked with [git-annex](https://git-annex.branchable.com) and hosted on the [Open Storage Network](https://www.openstoragenetwork.org) (OSN), at `https://nyu1.osn.mghpcc.org/diffuse-chess-public/20261028/`. Anyone can download the files without an account, and every download is checked against its recorded checksum. Data on OSN are not modified after they are written.

## Usage

Install DataLad, which requires git-annex (for example, `mamba install -c conda-forge datalad`). Cloning downloads only file names and metadata. File contents are fetched on request.

```bash
datalad clone https://github.com/prism-science/diffuse-data-raw-chess-20261028.git
cd diffuse-data-raw-chess-20261028

# fetch one file or directory
datalad get <path>

# fetch everything, four files at a time (diffraction images can be large)
datalad get -J4 .

# free up disk space when finished
datalad drop <path>
```

Plain git and git-annex also work:

```bash
git clone https://github.com/prism-science/diffuse-data-raw-chess-20261028.git
cd diffuse-data-raw-chess-20261028
git annex init
git annex get <path>
```

To download single files without git, use `https://nyu1.osn.mghpcc.org/diffuse-chess-public/20261028/<path>`.

## Acknowledgments

This work was supported by Radial, a division of Astera Institute.

Beamline ID7B2 at CHESS is part of the Center for High-Energy X-ray Sciences (CHEXS), which is supported by the National Science Foundation (BIO, ENG and MPS Directorates) under award DMR-2342336, and the Macromolecular Diffraction at CHESS (MacCHESS) facility, which is supported by award P30GM124166 from the National Institute of General Medical Sciences and the National Institutes of Health. Beamtime for this project was supported by funds from Cornell University.

Raw data are shared publicly on the Open Storage Network (OSN) via project allocation BIO250275 from [ACCESS](https://access-ci.org), supported by U.S. National Science Foundation (NSF) grants #2138259, #2138286, #2138307, #2137603, and #2138296.
