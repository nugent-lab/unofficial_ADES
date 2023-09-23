# Unofficial Python script to create ADES output


The Astrometry Data Exchange Standard (ADES) is a way of encoding observations of minor planets, such as asteroids and comets, with important information such as errors on measurements. Observations encoded following the ADES standard are accepted by the Minor Planet Center (MPC).

There is only one IAU-sanctioned ADES code repository, and this is not it. Here is the official [ADES repository is on GitHub.](https://github.com/IAU-ADES/ADES-Master)

The MPC [also has a page](https://minorplanetcenter.net/iau/info/ADES.html) describing the ADES standard.

## Then what is this?
This is a totally unsanctioned, unofficial, easy to use Python script that will take your observations and observation metadata (in dictionary format) and produce nicely formatted ADES 2017 output.

The authors make no claim or guarantee to the accuracy of this script. Use at your own risk. Again, [here is the official ADES repository.](https://github.com/IAU-ADES/ADES-Master)


## Usage

1. You will need Python3. This uses the `xml` package, which is probably already part of your install.

2. Clone or download this repository to your local machine.

3. Open the script `ades.py` in a code editor.

4. Modify the `ades_dict` and `ades_obs_dict` dictionaries in the script to provide your observatory's specific header information and observation data. As a default, you can  produce a 2-observation ADES xml output by running: 
 ```bash
python3 ades.py
```
4. However, most people will probably want to take the functions and calls and integrate them into your own software.

5. The MPC has a [very useful ADES validator](https://minorplanetcenter.net/submit_xml_test?method=post). Use it to check your output before submission.

## Authorship and Attribution
This code was written by T. Linder and refactored by C. Nugent, as part of the NEAT reprocessing project.

If you use this code in your work, please cite 
Nugent et al., "Reprocessing the NEAT dataset," in prep. 
