# Virtual Shopping Assistant

## Index
- **[About](#about)**
- **[Features](#features)**
- **[Instructions for running locally](#Instructions-for-running-locally)**
   - **[Initial steps](#initial-steps)**
   - **[Steps to Run](#steps-to-run)**
- **[Demo video](#demo-video)**
- **[Screenshots](#screenshots)**
- **[Tech Stack](#tech-stack)**   
- **[File Structure](#file-structure)**
## About
Virtual Shopping Assistant is a chatbot, which can assist consumers in deciding the right product and bridge the gap between online and offline shopping. 

## Features
- Suggests products to the consumer depending upon his needs, just like a salesperson.
- Helps the consumer to virtually experience fashion products. E.g. If a consumer needs to try a T-shirt or a spectacle our virtual shopping assistant gives him real time experience of how that product would look on him/her.
- Provides a summary of all the reviews about a product, which prevents users from doing the tedious job of going through hundreds of reviews of that product.

# Instructions for running locally

## Initial steps

1. Clone the repository by using the below command:

```
git clone https://github.com/cjchirag7/shopping-assistant
```

2. Download the 4 model files from [here](https://drive.google.com/drive/folders/1nu6HFg_POr-wF24rAJEH-ZRCn7wtIpIo?usp=sharing) and copy them all to the directory `shopping-assistant/services/api/`. Please note that if you download the `model_files` folder in .zip format, then you need to extract all the files out of it and then copy them to the above directory. 

## Steps to run
### Pre-requisites

1. Install `Docker` by looking up the
   [docs](https://docs.docker.com/get-docker/)
2. Install `Docker Compose` by looking up the
   [docs](https://docs.docker.com/compose/install/)
```
Note: If you are using Windows, make sure Docker Desktop is running.
```

### Steps

1. Make sure you are in the root of the project (i.e., `./shopping-assistant/`
   folder).
2. Run `docker-compose up` to spin up the containers. If you are using Linux or Mac, you may need to use `sudo` for this command to work. 
3. `web-app` would then be available locally at http://localhost:3000 , `server`
   at http://localhost:8000 and the `API documentation` would be available at http://localhost:8000/redoc

## Demo video

- Available at [https://youtu.be/IEIY7cP5M2U?si=TjLXJs0Np7mq4zNa]

## Screenshots

![Home Page](./screenshots/ss-1.png)
![Asking for printed shirts](./screenshots/ss-2.gif)
![Asking for printed shirts in other words](./screenshots/ss-3.gif)
![Asking for virtual trial](./screenshots/ss-4.png)
![Virtual trial step 1](./screenshots/ss-5.png)
![Virtual trial step 2](./screenshots/ss-6.png)
![Selecting a dress](./screenshots/ss-7.png)
![Virtual trial step 3](./screenshots/ss-8.png)
![Another example of virtual trial](./screenshots/ss-9.png)
![Asking for a mobile phone with specific properties](./screenshots/ss-10.gif)
![Virtual trial of sunglasses](./screenshots/ss-11.png)
![Summary of reviews](./screenshots/ss-12.png)
## Tech Stack

### Server

- [FastAPI](https://fastapi.tiangolo.com/#example)
- [Pytorch](https://pytorch.org/)
- [NLTK](https://www.nltk.org/)
### Web App

- [React.js](https://reactjs.org/docs/getting-started.html)
- [Jeeliz](https://github.com/jeeliz/jeelizGlassesVTOWidget)
### Others

- [Docker](https://www.docker.com/)

## File structure

- Screenshots have been attached in `screenshots/`
- Training files have been attached as `training-files/`
- Server code has been attached in `services/api/`
- Frontend code has been attached in `services/web-app/`
