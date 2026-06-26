FROM node:20-alpine
WORKDIR /app
COPY app/package*.json ./
RUN npm oi --omit=dev
COPY app/ ./ /app/
ENV NODE_ENV=production
ENV PORT=3000
EXPOSE 3000
USER node 
CMD {"npm","start"}