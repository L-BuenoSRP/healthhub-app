# Health Hub

Aplicação full-stack para gerenciamento de saúde, com dashboard interativo e integração com serviços de IA.

## Tecnologias

### Frontend
- React 18 com Vite
- Tailwind CSS para estilização
- React Router para navegação
- Recharts para visualização de dados
- Lucide React para ícones

### Backend
- Node.js
- Serverless Framework
- AWS Lambda
- DynamoDB
- OpenAI API

## Estrutura do Projeto

```
.
health-hub-backend/     # Backend Serverless
    src/               # Código fonte
    package.json       # Dependências do backend
    serverless-compose.yml  # Configuração Serverless
health-hub-frontend/   # Frontend React
    src/               # Código fonte
    public/            # Arquivos estáticos
    package.json       # Dependências do frontend
```

## Pré-requisitos

- Node.js 18+
- npm ou yarn
- Conta na AWS (para deploy)
- Credenciais AWS configuradas

## Como executar localmente

### Backend

1. Acesse a pasta do backend:
   ```bash
   cd health-hub-backend
   ```

2. Instale as dependências:
   ```bash
   npm install
   ```

3. Configure as variáveis de ambiente:
   Crie um arquivo `.env` na raiz do backend com as configurações necessárias.

4. Inicie o servidor local:
   ```bash
   npm run dev
   ```

### Frontend

1. Acesse a pasta do frontend:
   ```bash
   cd health-hub-frontend
   ```

2. Instale as dependências:
   ```bash
   npm install
   ```

3. Inicie o servidor de desenvolvimento:
   ```bash
   npm run dev
   ```
   O aplicativo estará disponível em `http://localhost:5173`

## Variáveis de Ambiente

### Backend
Crie um arquivo `.env` na pasta `health-hub-backend` com as seguintes variáveis:

```
AWS_ACCESS_KEY_ID=seu_access_key_id
AWS_SECRET_ACCESS_KEY=sua_secret_access_key
AWS_REGION=us-east-1
OPENAI_API_KEY=sua_openai_api_key
```

## Deploy

### Backend
```bash
cd health-hub-backend
npm run deploy
```

### Frontend
```bash
cd health-hub-frontend
npm run build
# Siga as instruções do seu provedor de hospedagem para fazer o deploy dos arquivos em /dist
```

## Licença

Este projeto está sob a licença MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.

## Contribuição

1. Faça um Fork do projeto
2. Crie uma Branch para sua Feature (`git checkout -b feature/FeatureIncrivel`)
3. Adicione suas mudanças (`git add .`)
4. Comite suas mudanças (`git commit -m 'Adicionando uma Feature incrível!'`)
5. Faça o Push da Branch (`git push origin feature/FeatureIncrivel`)
6. Abra um Pull Request
