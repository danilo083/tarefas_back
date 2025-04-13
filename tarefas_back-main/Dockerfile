# Usa a imagem oficial do Node.js como base (versão 18)
FROM node:18

# Define o diretório de trabalho dentro do container
# Tudo que for copiado ou executado a partir daqui será dentro de /app
WORKDIR /app

# Copia todos os arquivos do projeto para dentro do container
COPY . .

# Instala todas as dependências listadas
RUN npm install

# Define a variável de ambiente PORT com valor padrão 3000
# Pode ser sobrescrita por variáveis externas
ENV PORT=3000

# Expõe a porta 3000 para permitir acesso externo ao container
EXPOSE 3000

# Define o comando que será executado quando o container for iniciado
CMD ["npm", "start"]
