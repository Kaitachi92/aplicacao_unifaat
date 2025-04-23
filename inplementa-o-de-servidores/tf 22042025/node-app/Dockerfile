# Use a imagem oficial do Node.js (especifique a versão para evitar problemas futuros)
FROM node:16

# Define o diretório de trabalho dentro do contêiner
WORKDIR /app

# Copia os arquivos de dependências para o contêiner
COPY package*.json ./

# Instala as dependências do projeto
RUN npm install

# Copia todos os arquivos do projeto para o contêiner
COPY . .

# Expõe a porta que o aplicativo usará
EXPOSE 3001

# Comando para iniciar o aplicativo
CMD ["npm", "start"]