FROM node:10-alpine as build-stage

WORKDIR /app
COPY . .
RUN npm install && \
    npm run build 

FROM node:10-alpine as serve

WORKDIR /app
COPY --from=build-stage /app/dist ./dist
COPY --from=build-stage /app/package* ./
RUN npm install -g serve && \
    adduser -D app && \
    chown -R app /app/

USER app
EXPOSE 5000
ENV API_URL=http://localhost:8000

CMD ["serve","-s","-l","5000","dist"]
