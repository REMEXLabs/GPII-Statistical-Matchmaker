### Dependencies

[universal](https://github.com/GPII/universal)

Installation instructions

    npm install
	
    Depending on your system, you might have to remove node_modules\universal\node_modules\kettle\node_modules\infusion
	
    Depending on your system, you might have to move node_modules\universal\node_modules\infusion to node_modules\infusion
	
### Running the Statistical Matchmaker

    node bin/smm.js
	
Per default, using the Debug environment, the matchmaker will listen on port 8077. You can change that in configs/development.json

### Testing the Statistical Matchmaker
	
Usage example using [curl](http://curl.haxx.se/):

	curl -H "Content-Type: application/json" --data @sample_in.json http://127.0.0.1:8077/match
