# foot: An R package for processing building footprints
WorldPop Research Group, University of Southampton

### Quick Start  

1. Clone the repository to your computer (easiest with GitHub Desktop)
2. Install the *foot* package using the code in `./pkg_build.R`
3. Run the example script in `./wd/code/example_script.R`.
4. Check out the example function in `./R/footFun.R`.

### Inputs
Building footprints:  

//worldpop.files.soton.ac.uk/worldpop/Projects/WP517763_GRID3/DataIn/raw/DigitizeAfrica_building_footprints/

### Outputs
Rasters:  

1. Settlement (binary)
2. Building count
3. Total building area
5. Building density
4. Average building area
5. Standard deviation of building area
6. Coefficient of variation of building area
7. Average building perimeter length
8. Standard deviation of building perimeter length
9. Coefficient of variation of building perimeter length

### Repository Structure
The repository is structured as an R package with an additional folder "wd" that is a working directory for storing scripts, input data, and output data.

**./pkg_build.R**  
A script to build the R package and install it on your machine.

**./R/**  
A folder containing functions for the R package. Each file contains a function with Roxygen documentation for the function at the top of the script. See the example function `./R/footFun.R` for a template.

**./wd/code/**  
A folder containing scripts. See the example script `./wd/code/example_script.R` for a template.

**./wd/in/**  
A folder containing input data. This folder is included in the .gitignore for the repository, so files you save here will not be uploaded to github or shared with collaborators on the repository.

**./wd/out/**  
A folder containing outputs from the scripts. This folder is included in the .gitignore for the repository, so files you save here will not be uploaded to github or shared with collaborators on the repository.

**./man/**  
A folder containing function documentation created by Roxygen. **Do not edit these files.** Instead, use Roxygen to document each function (see `./R/footFun.R` for example) and build the documentation using `devtools::document()` (see `./pkg_build.R` for example).