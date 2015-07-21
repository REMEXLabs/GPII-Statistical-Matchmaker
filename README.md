# GPII Statistical Matchmaker: Runtime Component

## Dependencies

* [GPII's real-time framework ("universal")](https://github.com/GPII/universal).

## Installation instructions

First, get the code by running the following command in a terminal window:

    git clone https://github.com/REMEXLabs/GPII-Statistical-Matchmaker.git

Then change to the newly created directory (`cd GPII-Statistical-Matchmaker`) and run the following command:

    npm install
	
Depending on your system, you might have to remove `node_modules\universal\node_modules\kettle\node_modules\infusion`.
	
Depending on your system, you might have to move `node_modules\universal\node_modules\infusion` to `node_modules\infusion`.

The matchmaker uses the file `StatisticalMatchMakerData.js` in the directory `lib` as input. This file is generated by the [Analysis Module](https://github.com/REMEXLabs/GPII-Statistical-Matchmaker-Analysis). Instructions for generating this file based on the training data are available in the README.md file in the GPII-Statistical-Matchmaker-Analysis
 repository.

## Running the Statistical Matchmaker

    node bin/smm.js
	
Per default, using the Debug environment, the matchmaker will listen on port 8077. You can change that in `configs/development.json`.

## Testing the Statistical Matchmaker
	
Usage example using [curl](http://curl.haxx.se/):

	curl -H "Content-Type: application/json" --data @sample_in.json http://127.0.0.1:8077/match


## Funding Acknowledgement

The research leading to these results has received funding from the European
Union's Seventh Framework Programme (FP7/2007-2013) under grant agreement No.289016
([Cloud4all](http://www.cloud4all.info/)).
