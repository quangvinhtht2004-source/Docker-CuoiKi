# Sử dụng node image nhẹ (alpine)
FROM node:18-alpine

# Thiết lập thư mục làm việc
WORKDIR /app

# Copy file package.json trước để tận dụng cache layer của Docker
COPY package*.json ./

# Cài đặt dependencies
RUN npm install

# Copy toàn bộ source code
COPY . .

# Mở port 3000
EXPOSE 3000

# Lệnh chạy ứng dụng
CMD ["npm", "start"]