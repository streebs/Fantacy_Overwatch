# Fantacy_Overwatch
A program that gathers player stats and OWL data for analysis

I will be using the overwatch league api to access all the data. i will accomplish this by extracting the data using the requests 
library into .json files. using the json files i can parse through the file as a dictionary.

every weekend a number of matches will be played. i can get access to the match_id by following the /live-match/ path in the api.
i will need to find a way to automatically(manually first) get each match id for the weekend. that way i dont have to parse through the 
master match list. 

form the data of each match i will create player objects. each player will have a portfolio of their stats each week. im thinking of
an excel sheet with the columns being each week(or game posibly), and the rows being the individual stats for those games. 

		// side note. i think the api goes off of one map at a time. so i either need to separate by map or i need to combine the stats 
		// into one game??????

so far, this is a proof of concept to test my own coding and program design skills. also to help me increase proficiency in python. 
once the data is in the corresponding csv(excel sheets) files, Austin will help me desing the algorithms involed in calculating player skill,
ranking and potential. this step is a ways out from development, however it is the ultimate goal of this project. 

Here is a list of things to accomplish:
	- create an object for all players
		* will need player initializatiion routine
		* only needs to happen once then accessed by the app after that
	- successfully parse all the information form the api
		* get match ids
		* get stats
	- player calculations
		* TBA
	- automation
		* i want to eventually make this automatic. meaning let the app run and retrieve stats for us.
	- web implementation
		* one thing at a time


	Player Initialization

	i am not sure how to do this yet. the program needs to have access to all the player classes on run time not create them on runtime
	what im thinking for now is, i create a separate program to load either a master csv or a seperate csv for each player into the directory
	for this program??? could work. it may noe be hte best way.

	Data Retireval

	i will call by match id and map number. from there grab the stats of the players that played in the game and put the stats in
	their corresponding player classes and or csv file. (im thinking of using a PANDAS data frame for this????)
	
	Calculations

	TBA

	Automation

	TBA

	Web implementation

	TBA