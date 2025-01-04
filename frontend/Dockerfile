# Usando a imagem oficial do Node.js com Alpine para um ambiente leve
FROM node:18-alpine

# Definir o diretório de trabalho dentro do contêiner
WORKDIR /app

# Copiar os arquivos de dependência (package.json e package-lock.json) para o contêiner
COPY package.json package-lock.json ./

# Instalar dependências
RUN npm install

# Copiar o restante do código da aplicação
COPY . .

# Rodar o build da aplicação React
RUN npm run build

# Expor a porta que o React usa
EXPOSE 3000

# Comando para iniciar a aplicação React
CMD ["npm", "start"]
