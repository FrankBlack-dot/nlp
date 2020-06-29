# Requirements for the NLP project on Azure

## Tasks list for first NLP prototype :

1) Environment\
a) set up workspace\
b) save in config files

2) Data -  Request
Download data from NewsApi. There can be different input combinations. Run the download for each input kombination

a) Define the inputs for the download <br>
	I) concept - corona, corona virus etc <br>
	II) keywords - Procter and Gamble, P&G etc <br>
	III) language - en etc <br>
	IV) number of articles - 100 <br>
--> set of input <br>
b) Run the download on azure with python script <br>

3) Data - Storage <br>
Implement a python script which is doing <br>
a) one json is available for each set of inputs <br>
b) store  and register the json file on az - which is the best storage object/service on az for this <br>
c) transform the json to a dataframe <br>
d) store and register the dataframe on az - which is the best storage object/service on az for this <br>
e) make an az ML experiment out of it with the goal to re-run it and to schedule it on a regular basis <br>

4) Data - Analyse <br>
a) load the data from 3c) <br>
b) draw matplot lib charts <br>
	I) sentiment <br>
	II) #of news <br>
c) create an experiment and add plot to the experiment <br>

5) Modelling <br>
Provide a python to run on az <br>
a) define stop words <br>
b) perfome topic modelling <br>
c) create visulisation <br>
	I) topic <br>
	II) word clould <br>
d) create az experiment for modelling <br>
e) run the model training on az <br>
f) register the modell on azure <br>
e) save plot on az as experiment <br>


6) Provide a python script which make step 1-5 availabe as pipeline on az <br>


7) Deploy the results from az <br>
a) Model output as webservice -> tbd <br>
b) download result into BASF on premise -> tbd <br>

# Open question regarding azue

- How to access az with juoyter within BASF network
-Machine Learning Images, see jupyter notebook what is going on there<br>
-Review traing, building and do the training<br>
-Best practise development - local and deploy azure?<br>
-How to get files from one resource<br>
-When deploy a trainning script (or other) which is run on azure, where is it physically available<br>
-quota request - how do I get more, what do we have availabe<br>
-information about compute instances<br>, what can we get and how?
-compute instance vs. compute cluster<br>

