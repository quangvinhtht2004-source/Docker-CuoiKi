FROM node:18-alpine
WORKDIR /app

# COPY package*.json ./      <-- Thêm dấu # ở đầu dòng này
# RUN npm install            <-- Thêm dấu # ở đầu dòng này

COPY . .
EXPOSE 3000
CMD ["npm", "start"]