FROM node:latest

WORKDIR /mydir
COPY . .
RUN npm install
EXPOSE 5000
ENV API_URL=http://localhost:5000
CMD ["npm", "start"]

