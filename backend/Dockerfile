FROM node:20
EXPOSE 80/tcp
ENV DB_HOST=mysql
RUN adduser expense
RUN mkdir /app
RUN chown expense:expense -R /app
WORKDIR /app
COPY package.json .
COPY *.js .
RUN npm install
CMD ["node", "index.js"]



