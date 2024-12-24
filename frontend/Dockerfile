# Imagem base
FROM node:18-alpine

# Define o diretório de trabalho
WORKDIR /app

# Copia o package.json e instala as dependências
COPY package*.json ./
RUN npm install

# Copia o código para o container
COPY . .

# Expõe a porta do servidor de desenvolvimento
EXPOSE 3000

# Comando para iniciar o frontend
CMD ["npm", "start"]
