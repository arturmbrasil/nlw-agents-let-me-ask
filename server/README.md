# NLW Agents

Projeto desenvolvido durante o evento **NLW (Next Level Week)** da Rocketseat, focado em criar uma API para gerenciamento de agentes/chatbots.

## 🚀 Tecnologias Utilizadas

### Backend
- **Node.js** - Runtime JavaScript
- **TypeScript** - Linguagem de programação tipada
- **Fastify** - Framework web rápido e eficiente
- **Drizzle ORM** - ORM moderno para TypeScript
- **PostgreSQL** - Banco de dados relacional
- **Zod** - Validação de schemas e tipos
- **Docker** - Containerização da aplicação

### Ferramentas de Desenvolvimento
- **Biome** - Linter e formatter
- **Drizzle Kit** - CLI para migrações e seeds
- **Ultracite** - Ferramenta de desenvolvimento

## 📁 Estrutura do Projeto

```
src/
├── db/
│   ├── connection.ts    # Conexão com banco de dados
│   ├── schema/          # Schemas do Drizzle ORM
│   └── seed.ts          # Dados iniciais
├── http/
│   └── routes/          # Rotas da API
├── env.ts               # Configuração de variáveis de ambiente
└── server.ts            # Servidor principal
```

## 🛠️ Padrões de Projeto

- **Arquitetura em Camadas** - Separação clara entre rotas, banco de dados e lógica de negócio
- **Type Safety** - Uso extensivo de TypeScript com validação via Zod
- **Database First** - Schemas definidos com Drizzle ORM
- **Environment Validation** - Validação de variáveis de ambiente com Zod
- **CORS Configurado** - API preparada para integração com frontend

## ⚙️ Setup e Configuração

### Pré-requisitos
- Node.js 18+
- Docker e Docker Compose
- PostgreSQL (via Docker)

### Instalação

1. **Clone o repositório**
```bash
git clone <url-do-repositorio>
cd server
```

2. **Instale as dependências**
```bash
npm install
```

3. **Configure as variáveis de ambiente**
Crie um arquivo `.env` na raiz do projeto:
```env
PORT=3333
DATABASE_URL=postgresql://docker:docker@localhost:5432/agents
```

4. **Inicie o banco de dados**
```bash
docker-compose up -d
```

5. **Execute as migrations e seeds**
```bash
npx drizzle-kit migrate

npm run db:seed
```

6. **Inicie o servidor**
```bash
# Desenvolvimento
npm run dev

# Produção
npm start
```

## 📡 Endpoints da API

- `GET /health` - Health check da aplicação
- `GET /rooms` - Lista todas as salas/agentes

## 🐳 Docker

O projeto inclui configuração Docker para PostgreSQL com pgvector:

```bash
# Iniciar banco de dados
docker-compose up -d

# Parar banco de dados
docker-compose down
```

## 📝 Scripts Disponíveis

- `npm run dev` - Inicia o servidor em modo desenvolvimento com hot reload
- `npm start` - Inicia o servidor em modo produção
- `npm run db:seed` - Executa o seed do banco de dados

---

Desenvolvido com 💜 durante o NLW da Rocketseat 