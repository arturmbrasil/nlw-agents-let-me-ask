# NLW Agents

Projeto desenvolvido durante o evento **NLW (Next Level Week)** da Rocketseat, focado em criar uma aplicação web moderna com React e TypeScript.

## 🚀 Tecnologias Utilizadas

### Core
- **React 19** - Biblioteca para construção de interfaces
- **TypeScript** - Tipagem estática para JavaScript
- **Vite** - Build tool e dev server

### Styling & UI
- **Tailwind CSS 4** - Framework CSS utilitário
- **shadcn/ui** - Componentes UI reutilizáveis
- **Lucide React** - Biblioteca de ícones
- **class-variance-authority** - Utilitário para variantes de componentes
- **clsx & tailwind-merge** - Utilitários para classes CSS

### State Management & Data Fetching
- **TanStack Query (React Query)** - Gerenciamento de estado do servidor

### Routing
- **React Router DOM** - Roteamento da aplicação

### Development Tools
- **Biome** - Linter e formatter (substituindo ESLint + Prettier)
- **Ultracite** - Configuração de linting otimizada

## 📁 Estrutura do Projeto

```
src/
├── components/
│   └── ui/          # Componentes shadcn/ui
├── pages/           # Páginas da aplicação
├── lib/             # Utilitários e configurações
├── app.tsx          # Componente principal
└── main.tsx         # Entry point
```

## 🛠️ Padrões de Projeto

- **Component-Based Architecture** - Componentes reutilizáveis
- **File-Based Routing** - Roteamento baseado em arquivos
- **Atomic Design** - Estrutura de componentes organizada
- **TypeScript First** - Tipagem estática em todo o projeto
- **Modern CSS** - Tailwind CSS com variáveis CSS customizadas

## ⚡ Setup e Configuração

### Pré-requisitos
- Node.js 18+ 
- npm ou yarn

### Instalação

1. Clone o repositório:
```bash
git clone <url-do-repositorio>
cd nlw-agents
```

2. Instale as dependências:
```bash
npm install
```

3. Execute o projeto em modo de desenvolvimento:
```bash
npm run dev
```

4. Acesse `http://localhost:5173` no seu navegador

### Scripts Disponíveis

- `npm run dev` - Inicia o servidor de desenvolvimento
- `npm run build` - Gera build de produção
- `npm run preview` - Preview do build de produção

## 🎯 Funcionalidades

- Criação de salas
- Navegação entre páginas
- Interface responsiva
- Componentes reutilizáveis

---

Desenvolvido com 💜 durante o NLW da Rocketseat 