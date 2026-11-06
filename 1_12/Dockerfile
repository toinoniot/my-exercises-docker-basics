FROM ubuntu

WORKDIR /usr/src/app

EXPOSE 5001

COPY . ./

RUN apt-get update && apt-get install -y curl

RUN curl -sL https://deb.nodesource.com/setup_16.x | bash && apt-get install -y nodejs

RUN npm install

RUN npm install -g serve

RUN npm run build

CMD ["serve", "-s", "-l", "5001", "build"]

