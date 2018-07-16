# LK-Tap-News-System

Pre-requirement:

1.redis

2.mongodb

Install:

pip3 install -r requirements.txt

cd ./tap-news-webserver/web
npm install

cd ./tap-news-webserver/server
npm install


Run:

./news_launcher.sh(scrape, dedupe news)

./launcher.sh

web: localhost:3000

This is a real-time news scraping rendering and recommendation system. A news pipeline was built to scrape latest news from various of sources such as CNN, BBC. A single-page web application using React was buit to render scraped news to users. In addition, in order to customize news for users, I designed and built a training pipeline for news topic modeling using Tensorflow.

● Implemented a news pipeline which monitors, scrapes and dedupes latest news (MongoDB, Redis, RabbitMQ, TF-IDF);

● Built a single-page web application for users to browse news (React, Node.js, RPC, SOA, JWT);

● Implemented a click event log processor which collects users’ click logs, then updates a news preference model for each user (NLP);

● Designed and built an offline training pipeline for news topic modeling (Tensorflow, DNN, NLP);

● Deployed an online classifying service for news topic modeling using the trained model.

# Architecture
![architecture](https://user-images.githubusercontent.com/29580346/42471918-59705270-8374-11e8-9e42-4bbff803ba9b.png)

# Life Cycle
![image](https://github.com/wxm146case/Tap-News-System/blob/master/life%20cycle.PNG)

# ScreenShot
![login](https://user-images.githubusercontent.com/29580346/42471970-8a0e2326-8374-11e8-91f6-ea4c69ae105d.png)
![web](https://user-images.githubusercontent.com/29580346/42471971-8c174e36-8374-11e8-85e0-f9633e536bad.png)
