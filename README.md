# ✨ Streamlit based Automatic YouTube subtitle generation 🔊 [![Project Status: Active](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active) [![](https://img.shields.io/badge/Prateek-Ralhan-brightgreen.svg?colorB=ff0000)](https://prateekralhan.github.io/)
A streamlit based webapp to generate subtitles for YouTube Videos. This work is just a streamlit implementation of the wonderful work done by **[m1guelpf](https://github.com/m1guelpf/yt-whisper#automatic-youtube-subtitle-generation)**.

![demo](https://user-images.githubusercontent.com/29462447/201472171-0c20444c-82a4-444e-85eb-a1898c9ae896.gif)

## Installation:
* Simply run the command ***pip install -r requirements.txt*** to install the necessary dependencies.

## Usage:
1. Head over to [this link](https://github.com/openai/whisper) and follow the steps to get a comprehensive overview of the architecture of OpenAI's whisper models. 
2. Simply run the command: 
```
streamlit run app.py
```
3. Navigate to http://localhost:8501 in your web-browser.

![1](https://user-images.githubusercontent.com/29462447/201472184-e0d865dc-cbfc-4f92-bc16-7231916fa888.png)



### Running the Dockerized App
1. Ensure you have Docker Installed and Setup in your OS (Windows/Mac/Linux). For detailed Instructions, please refer [this.](https://docs.docker.com/engine/install/)
2. Navigate to the folder where you have cloned this repository ( where the ***Dockerfile*** is present ).
3. Build the Docker Image (don't forget the dot!! :smile: ): 
```
docker build -f Dockerfile -t app:latest .
```
4. Run the docker:
```
docker run -p 8501:8501 app:latest
```

This will launch the dockerized app. Navigate to ***http://localhost:8501/*** in your browser to have a look at your application. You can check the status of your all available running dockers by:
```
docker ps
```
