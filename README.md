# Updated version of **pyILT2**
## Updated by Kan Hatakeyama (2022/9/30)
    - v0.9.8 to v1.0.0
    - Fix bug of property search
    - Update information is available on the bottom of this page

# Update by Pratik Dhakal (10/25/2022)
 - Fixed the pyilt2 report issue "Error : Lower consolute temperature”
 - The error was caused by the addition of new properties such as "Lower consolute temperature" to the NIST IL thermo database
 - The pyilt2 property dictionary had an issue when it encountered the new property name as it had no such property in its own database
 - Simple fix by adding new properties name to the pyilt2 property dictionary

List of properties available in NIST IL thermo can be accessed from here

https://ilthermo.boulder.nist.gov/ILT2/ilprpls


# Added new properties to the pyilt2 property dictionary

 - 'Lower consolute temperature': 'Tlcon'
 - 'Enthalpy of solution': 'Elson'
 - 'Binary diffusion coefficient': 'BDC'
 
 # Modified existing property name to match the NIST IL thermo database
 
 - ~~Self-diffusion coefficient~~   'Self diffusion coefficient' 
 
# Installation

- pip3 install git+https://github.com/pratik994/pyilt2_nist_updated.git


# Usage
## Command line pyilt2 report
 - pyilt2report -c '1-ethyl-3-methylimidazolium thiocyanate' -n 1 -p 'dens' --doi

# Official documentation of NIST IL pyilt2 
- http://wgserve.de/pyilt2/
