# Ponderada Backstage

Para essa atividade, deve-se instalar a aplicação do backstage e rodá-la no Docker. 

## Instalação

### Clone este repositório:
```bash
git clone https://github.com/pingu01/backstage-sem2.git
```

### Instale o Yarn, caso não esteja instalado:
```bash
npm install --global yarn
```



### Navegue até o diretório da aplicação e instale as dependências:
```bash
yarn install --frozen-lockfile
```

### Prepare os types do Backstage:
```bash
yarn tsc
```

### Build a aplicação:
```bash
yarn build:backend
```

## Build no Docker

### Faça o build da imagem Docker:
```bash
docker image build . -f packages/backend/Dockerfile --tag backstage --no-cache    
```

![alt text](image.png)

### Rode o container Docker:
```bash
sudo docker run -it -p 7007:7007 backstage
```

![alt text](image-1.png)


