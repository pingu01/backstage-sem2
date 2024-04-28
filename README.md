# Ponderada Backstage

Para essa atividade, deve-se instalar a aplicação do backstage e rodá-la no Docker. 

## Instalação

Para rodar a aplicação, deve-se usar estes comandos:

```bash
    docker image build . -f packages/backend/Dockerfile --tag backstage --no-cache  
    
    docker run -it -p 7007:7007 backstage
```


