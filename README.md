# docker-puppeteer

Base docker image with puppeteer support

## Usage

```
FROM uninode/puppeteer
WORKDIR /usr/src/app
COPY package*.json ./
RUN npm install --production
COPY . .
EXPOSE 3000
CMD [ "npm", "start" ]
```
