<p align="center">
  <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSHQkwi1Rv5zgeGm0WK8X-YFslWGTDhrnOzkQ&s" alt="a title">
</p>
# Use Groq API key and Streamlit to make an AI Chatbot interface
Here are some instructions you can  use to make an AI interface using the official Groq API, which you can find here: https://console.groq.com/keys
## Step 1: Get API key
The first step of this project is to get the free API key for Groq. Navigate to this link: https://console.groq.com/keys. Create an account if you need to. Click create API key, make a display name for the key, and copy the API key provided and save it  somewhere, as Groq will not display the API key again.

Make a Groq Account:
![Alt text](https://image-forwarder.notaku.so/aHR0cHM6Ly93d3cubm90aW9uLnNvL2ltYWdlL2h0dHBzJTNBJTJGJTJGcHJvZC1maWxlcy1zZWN1cmUuczMudXMtd2VzdC0yLmFtYXpvbmF3cy5jb20lMkY4N2NmOTdjZS05OTQ2LTRjM2QtYTdlMC1hNzkxZWVhMmE0ZTIlMkYyMzEzOWI5MC04YjJjLTQ4ZmEtYjgxNC0yOGEyZTdhN2RkZTklMkZVbnRpdGxlZC5wbmc_dGFibGU9YmxvY2smc3BhY2VJZD04N2NmOTdjZS05OTQ2LTRjM2QtYTdlMC1hNzkxZWVhMmE0ZTImaWQ9ZDM0MDljNWQtNzg2OC00MGM2LThjY2YtMjA4NTkzODE4MDc4JmNhY2hlPXYyJndpZHRoPTI0MDA= "sign in Groq")

Make an API key here: https://console.groq.com/keys
![Alt text](https://image-forwarder.notaku.so/aHR0cHM6Ly93d3cubm90aW9uLnNvL2ltYWdlL2h0dHBzJTNBJTJGJTJGcHJvZC1maWxlcy1zZWN1cmUuczMudXMtd2VzdC0yLmFtYXpvbmF3cy5jb20lMkY4N2NmOTdjZS05OTQ2LTRjM2QtYTdlMC1hNzkxZWVhMmE0ZTIlMkY3OGNjMjQwZS1hMzAyLTRkN2UtODZiNC0xMWFlMDE0NjdkOWElMkZVbnRpdGxlZC5wbmc_dGFibGU9YmxvY2smc3BhY2VJZD04N2NmOTdjZS05OTQ2LTRjM2QtYTdlMC1hNzkxZWVhMmE0ZTImaWQ9ZWM3OTcxMDUtYWJkZS00NTFlLTkwYzQtOWNjMzk2YjVlMjBiJmNhY2hlPXYyJndpZHRoPTI0MDA= "make API")

Copy API key and save for later


## Step 2: Set up Project
The next step in this project is to create a new Python project, and get Groq and Streamlit. First, initialize a new Python project. Then, in the shell, type the following command.
```bash
git clone https://github.com/opal1056/ai-groq.git
```
This will clone the git repository with the important files. The next thing you want to do is to install Groq and Streamlit libraries using this command.
```bash
pip install streamlit groq
```
This will install Groq and Streamlit, which are needed to run the project.
## Step 3: Run the App
Before running the app, you need to set up a ```secrets.toml``` file. In the directory. It should look something like this:
```toml
[secrets]
GROQ_API_KEY = "your-api-key-here"
```
Replace ```your-api-key-here``` with your actual API. You should also make sure to gitignore this file so Git ignores it when making commits because it contains your API key, which is sensitive information.

The next thing to do is to run the app using the following command:
```bash
streamlit run streamlit_app.py
```
Once you do this, you should receive a local URL to use to access your application locally. Congratulations, you have used Groq and Streamlit to make an AI chat interface. The next thing to do is to deploy it on a public live URL so the world can see it.

## Step 4: Deploying to Streamlit
The next step is to deploy your app on Streamlit. The first thing you need to do is to fork this repository. Now you can deploy to Streamlit. You can do this by making an account on Streamlit here: https://authkit.streamlit.io/sign-up. Now that you have an account, you can deploy your app. Go to https://share.streamlit.io, and click Create App in the top right hand corner. Click the option to deploy from Github, and click on your forked repository and change the domain if you like. Now, click on Advanced Settings and paste this code in the secrets box.
```toml
GROQ_API_KEY = "your-api-key-here"
```
If I were you, I wouldn't make a secrets.toml file in my public Github repository with my API key. You don't want some random person taking your API key and overusing and abusing it. Just paste it here, and replace ```your-api-key-here``` with your actual API key. Now click save.

The final step is to deploy your app using the Deploy button. It will take some time to deploy your app, but you will finally get your deployed. You will receive a live .streamlit.app URL for your app to access from anywhere at anytime. Be careful though, you don't want someone racking up charges on your API using your website.
## Done!
Congratulations! You have built your own AI interface using Groq API and Streamlit!
