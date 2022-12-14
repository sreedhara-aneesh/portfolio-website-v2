FROM node:18.12.1
WORKDIR /app

COPY package.json package.json
COPY package-lock.json package-lock.json
RUN npm install

COPY . .

RUN npm run build

ENTRYPOINT npx serve -s build -p 3000