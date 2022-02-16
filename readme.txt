Steps:

a. Use provided git repo to get access to the files and once zip file is visible then download it locally and follow the below steps or use readme file:

1. Extract the Zipped file. This will create a directory "FlaskApp".

2.  Extract the "FlaskApp.zip" which contains below files/directories.
	a. __init__.py
	b. logs
	
3. Download and Install Python. Make sure to ADD PATH in system environment.
	can be downloaded through - https://www.python.org/downloads/
	
4. Open the CMD(Command Promt) using Windows+R and type in CMD and Install below Python libraries. 
	1) flask with command:
				pip install flask
4.
	2) Navigate to FlaskApp directory using command: cd FILE_LOCATION (cd followed be filelocation)
	3) Run command: python __init__.py		
	4) This will start the flask server
	5) All the Requests will be visible in CMD(Command Promt).
	
5. Now open the new CMD(Command Promt) and run below URL.
	curl http://127.0.0.1:5000/
	
	if above command returns with "Hello, World" then Flask app is all SET.

6. All the logs will be written in FlaskAPP directory, inside file "Request_Logs.log"

7. Test Cases - 

	1. Go to web browser and use URL: http://127.0.0.1:5000/, it should return "Hello, World".

	2. If Any other URL checked at browser, Example: http://127.0.0.1:5000/XYZ, it should return error as these routes are not defined.

	3. Below curl command should return JSON object.
		curl -H "Accept: application/json" "http://127.0.0.1:5000"
	
	4. Below curl command should return JSON data.
		curl -X POST -H "Accept: application/json" http://127.0.0.1:5000/
	
	5. Below curl command should reutn simple HTML data.
		curl http://127.0.0.1:5000/
	
	6. Below curl command should return simple HTML data.
		curl -X POST http://127.0.0.1:5000/

	7. Test Cases-1, 3, 4, 5, 6 should make entry in Request_logs.log file in "logs" folder.
