# con/validation

Platform to discuss/distill coordination for validators output(s).

## Rationale

There is a growing number of standards in neuro*sciences, some of which neuro-specific (e.g. BIDS, NWB), some of wider related community (DICOM, NGFF/OME), and some are generic *file* formats etc (JSON, Zarr, etc).
In addition there is growing use of elements of "linked web" such as ontologies, controlled vocabularies, etc.
One of the main benefits behind standardization and choosing controlled vocabularies is the ability to validate (meta)data.
In addition, some validators might provide recommendations or hints on best practices.
Different validators were created, typically separately for each standard.
Some were "integrated", e.g. BIDS validator uses HED validator.
In `dandi-cli` we also use bidschematools for rudimentary validation of BIDS paths, nwb-inspector for validation of NWB files, and ad-hoc validation for DANDI files layout.

Many if not most validators have means to output results of validation in machine readable form, e.g. JSON.

Ideally we should gain some common format/API/data-structure to define outputs of a validator so we could reuse it.
In `dandi-cli` we already tried to accomplis that in https://github.com/dandi/dandi-cli/blob/master/dandi/validate_types.py .

This repository is attempt to converge across wider range of standards/tools.

**Please add this repo to your repos to watch if interested -- more dialog to be initiated via issues and PRs**

## A list of standards/formats used in neuroscience and needed validation

**TODO**: add references

- BIDS
- HDF5
- HED
- JSON
- NGFF/OME-Zarr
- NWB
- YAML
- Zarr

and could also be seen on "mindmap" for BIDS

![BIDS mindmap](https://bids-website.readthedocs.io/en/latest/assets/img/BIDS-minder.svg)

