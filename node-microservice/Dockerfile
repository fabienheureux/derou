FROM node
ENV SCRIPT start
WORKDIR /app
COPY ./package*.json ./
RUN npm ci
COPY . .
RUN npm run build
EXPOSE 3000
CMD ["sh", "-c", "npm run $SCRIPT"]
