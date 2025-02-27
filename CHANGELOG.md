# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.1.4] - 2022-01-25

### Modified

- Fix the file in the transposonmapper module inside the exporting submodule: save_as_wig.py
- The change is related to save the wig file as the standard convention which requires a lower case letter instead of a capital one that was the case of previous versions. Specifically, the change of the `VariableStep` line to `variableStep`. 
- This change is not affecting the functionality of the code.
- Fix the 10% first truncation of the gene calculation. Basically redefine`N10percent` to `int(len(N_reads) * 0.1)`

## [1.1.3] - 2021-11-23

### Added
- Fix a bug on the pysam module import when using the default version of transposonmapper, that should not require this installation from the user. This is an issue for Windows and Mac users, where pysam can not be used.
- Add an integration test for the pysam module import.

## [1.1.2] - 2021-11-01
### Added 
- FIX to the volcano plot function from the statistics module of transposonmapper (https://github.com/SATAY-LL/Transposonmapper/issues/62)


## [1.1.1] - 2021-09-22
### Added
- Test framework with continuos integration through Github actions that generates a coverage report from SoundCloud after every push and pull requests. 
- Pip installable package 
- Contributing guidelines 
- Containerization through Docker 
- Package documentation through Jupyter Book integrated in the main repository.
- Adding a citation file  
- Adding notebooks that describe the whole pipeline package.

### Changed
- The code was refactored as much as possible into functions in order to design unit tests on them. 
- The GUI have now a Getting started help document to know how to use it. 
- Readme improved. 
- The code structure was changed to modules inside the package. 

### Removed


## [1.0.0] - 2021-03-25

This is the initial version of Transposonmapper from https://github.com/SATAY-LL/LaanLab-SATAY-DataAnalysis/releases
