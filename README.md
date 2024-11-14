# RoninFlow - Projeto em desenvolvimento

## Requisitos

- **Docker**: Para criar um ambiente de desenvolvimento isolado
- **Docker Compose**: Para gerenciar os contêineres necessários
- **Node.js e NPM**: Para construir e gerenciar os arquivos estáticos

## Configuração do Ambiente de Desenvolvimento

### Passo a Passo

1. **Clone o repositório:**
``` bash
git clone https://github.com/seu_usuario/roninflow.git
cd roninflow
```

2. Crie o arquivo .env: 
``` bash
cp .env.example .env
```

3. Suba os contêineres com Docker Compose:
``` bash
docker-compose up -d
```

4. Acesse o container app
``` bash
docker-compose exec app bash
```

5. Instale as dependências do projeto
``` bash
composer install
```

6. Gere a key do projeto Laravel
``` bash
php artisan key:generate
```

7. Rodar as migrations
``` bash
php artisan migrate
```

8. Na pasta raiz do projeto, execute:
``` bash
npm install
npm run build
```

### Acesse o projeto http://localhost:8000