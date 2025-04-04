FROM node:18

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

# Expose the port (common port for React apps, adjust if needed)
EXPOSE 3000

# Update the command to bind to all interfaces
ENV HOST=0.0.0.0

# Run the development server
CMD [ "npm" , "run", "dev", "--", "--host", "0.0.0.0" ]