
# FROM node as development

# WORKDIR /usr/app

# COPY package.json ./

# RUN npm install

# COPY . .

# EXPOSE 3000

# RUN npm run build

# FROM node as production

# WORKDIR /usr/app

# COPY package.json ./

# RUN npm install --only=production

# COPY . .

# EXPOSE 3000

# COPY --from=development /usr/app/dist ./dist

# CMD ["node", "dist/main.js"]

FROM node as development

WORKDIR /usr/app

COPY package.json ./

RUN npm install

COPY . .

EXPOSE 3000

CMD ["npm", "run", "start:dev"]