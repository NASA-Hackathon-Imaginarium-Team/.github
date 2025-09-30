# NASA Hackathon

Hi Team. Ive made some notes ahead of the Friday meeting as to what I think our project could look like, and what I believe the roles should look like. Considering the size of our team, it will be important to be organised. Each person should have a clear role and understand their part in the wider task. 
Below, I have listed 3 ideas for what the project could be. These are not set in stone, and can be changed during the Friday meeting. Consider these ideas as a starting point. 
Below that, you will find a number of job roles and thier desciption. Please have a read through and see what you find interesting. You may end up having 2 roles on the 2 days. For example:
- Shaheer, you may want to do data processing on day 1 and create a data pipeline, then switch to creating the webapp for day 2.
- Senan, you may wish to work on training the AI model day 1, but choose to work on the webapp day 2.
This is up to you! 

## Project Ideas

### Exoplanet Classification Webapp
An interactive visualisation of the predictions from the datasets. Potentially a dashboard or some analytics page that shows the number of exoplanets identified etc.

### Exoplanet Browser
A webapp allowing people to filter the database for exoplanets with specific characteristics

### Citizen Science Logger
Citizen Science is a form of public participation in research studies. The idea is to use citizens as your researchers to get more eyes and ears in the field. In Ornithology, citizen science is used for members of the public to log sighting of bird species to track thier movements and population.
A webapp could be created using these citizen science principles allowing astronomers to submit data that could be an exoplanet. Could include a leaderboard for people who upload datasets that lead to "discoveries"

## Job roles:
- Data Processing
	- Getting data from various datasets
	- Ensuring data from datasets are consistent in layout
	- Cleaning data for null values etc
	- Splitting dataset into test and train bins. I am proposing a 70/20/10 split. 70% of the dataset used for training, 20% used to test the model, 10% unseen by the model used to test the finished webapp
- AI Trainer
	- Testing multiple models and selecting the best suited model. Start with XGBoost and EfficientNet
	- Testing hyperparameters
	- Creating classifcation matrixes and reports to ensure models are not overfitting
	- Export trained models as .pkl files to be used by the server and webapp frontend
- Web Developer
	- Create a server to serve the webapp and host API endpoints for getting predictions from the trained AI model
	- Design a frontend to display useful data. Work with the physicist to understand what information is deemed "useful". Treat the physicists as the end-user/product owner.
	- Create frontend using any web technology to be served from the server
- Physics Consultant
	- Help the team understand the data were looking at
	- Work with the web developers to design a tool that is useful in physics research. Consider what data you would like to have readily available from this dataset. What data would be interesting to display.
	- Work with the AI trainig and data processing team to determine which fields from the dataset should be used to train the models, and which fields dont add value
	- Work with the data processing team to help them understand how the data should be formatted, and what the data means.
	- Treat the computer scientists as if all the information is written in a different language, and you are the only interpreter available. Because thats essentially how it is!
