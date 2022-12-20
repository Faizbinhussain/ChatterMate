# ChatterMate
ChatterMate is a free to use AI chatbot made with Flask and Dialogflow.  
## PREREQUISITE
Make sure you have installed the following tools.
- Download and install [**Python**](https://www.python.org/) from here as per your supported OS (Any versions >= 3.6).
- IDE (Integrated Development Environment) [**Visual Studio Code**](https://code.visualstudio.com/download). ***`optional`***
## REQUIRED LIBRARIES
- [**Flask**](https://pypi.org/project/Flask)
```
pip install Flask
```
- [**Dialogflow**](https://pypi.org/project/dialogflow)
```
pip install dialogflow=1.1.1
```
### Service Account Setup
1. In [**Dialogflow's console**](https://dialogflow.cloud.google.com), go to settings ⚙ and under the general tab, you'll see the project ID section with a Google Cloud link to open the Google Cloud console. Open Google Cloud.
2. In the Cloud console, go to the menu icon **☰ > APIs & Services > Credentials**
3. Under the menu icon **☰ > APIs & Services > Credentials > Create Credentials > Service Account Key**.
4. Under Create service account key, select New Service Account from the dropdown and enter. If you already have a service account key, select that. 
5. Give any name for the name and click Create. Give **Dialogflow API Admin** role.
6. Create a new key with format of JSON.
7. JSON file will be downloaded to your computer that you will need in the setup sections below.

### Set up Dialogflow DetectIntent endpoint to be called from the App
1. Inside root folder, replace the key.json in the credentials folder with your own credentials json file. 
2. In app.py, Change the GOOGLE_PROJECT_ID = **"<YOUR_PROJECT_ID>"** to your project ID.

### Using the chatbot
1. Run app.py after following all given above instructions.
2. Open [**http://127.0.0.1:5000**](http://127.0.0.1:5000) in your browser.
3. Enjoy chatting. :)
