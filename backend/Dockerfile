FROM node

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 80

# Pass user_name and password by running docker run --e command
ENV MONGODB_USERNAME=user_name
ENV MONGODB_PASSWORD=user_password

CMD ["npm", "start"]
