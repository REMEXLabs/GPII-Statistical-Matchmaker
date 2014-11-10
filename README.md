### Dependencies

[universal](https://github.com/GPII/universal)

Installation instructions

Firstly, install node and npm.

    npm install
	
### Running the Statistical Matchmaker

    node bin/smm.js
	
Per default, using the Debug environment, the matchmaker will listen on port 80. You can change that in configs/development.json

### Testing the Statistical Matchmaker
	
Usage example using [curl](http://curl.haxx.se/):

	curl -X POST -H "Content-Type: application/json" localhost:80/match -d @[some preference set]
