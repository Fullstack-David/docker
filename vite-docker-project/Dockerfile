FROM node:20-alpine

WORKDIR /app

COPY package.json package-lock.json ./


RUN npm install
RUN npm install -g vite
RUN chown -R node:node /app

USER node 


COPY . .


EXPOSE 5173

# Run the application.
CMD ["npm", "run", "dev"]
