# Sử dụng môi trường Node.js
FROM node:18-alpine

# Thiết lập thư mục làm việc
WORKDIR /app

# Copy file package.json trước (để tận dụng cache)
COPY package*.json ./

# Lệnh cài đặt thư viện (chỉ chạy khi build)
RUN npm install

# Copy toàn bộ code vào
COPY . .

# Mở cổng 3000
EXPOSE 3000

# Lệnh chạy ứng dụng
CMD ["npm", "start"]