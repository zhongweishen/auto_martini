# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).


## [0.0.1]
### Added
- New CLI for reading input and writing output
- New modular design consisting of "test" and "engine" submodules
- CLI arg --top to the parser so that the output topology would be written to a file (no longer printed to stdout)
- Support for python 3
- New "optimization.pyx" module for faster implementation (in C) of find_bead_pos()

### Changed
- Fixed genMoleculeSDF() which did not use "sdf" input argument
- Fixed function printBonds() which used undefined "atomPartitioning" object
- Function Substructure() no longer creates then reads "tmp-auto-martini.smi" file
- Function check_additivity() no longer creates then reads "tmp-auto-martini.smi" file

### Removed
- Undefined objects "hbondA" and "hbondD" in function printAtoms()
- Variable "mad" in function checkAdditivity() was already defined as a function

## [0.0.2]
### Added
- Testing scripts that work with pytest

### Changed
- Fxed bug with ...

### Removed
- test submodule (replaced with pytest scripts)