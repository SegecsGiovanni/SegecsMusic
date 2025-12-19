# SegecsMusic
# 📋 Projeto SegecsMusic - Spotify Clone

## 📅 Data da Última Atualização
**19 de Dezembro de 2025 - 18:00**

---

## 🎯 Visão Geral do Projeto

**Nome do Projeto:** SegecsMusic  
**Tipo:** Clone do Spotify (Aplicação de Streaming de Música)  
**Arquitetura:** Fullstack (Backend + Frontend)  
**Status:** 🔄 Em desenvolvimento - Fase inicial

---

## 🏗️ Estrutura do Projeto

```
SegecsMusic/
├── backend/
│   ├── package.json (✅ Configurado - Express, módulo ES)
│   ├── src/
│   │   ├── app.js (⏳ Vazio - a ser desenvolvido)
│   │   └── server.js (⏳ Entry point a ser criado)
│   └── node_modules/
├── frontend/
│   ├── package.json (✅ React + Vite + Zustand + Router + Axios)
│   ├── node_modules/
│   └── src/ (⏳ Estrutura Vite a ser criada)
├── .git/ (✅ Repositório inicializado)
├── .gitignore (✅ Configurado)
└── README.md (📝 Documentação)
```

---

## 🔧 Dependências do Backend

### **Dependências de Produção**

| Pacote | Versão | Descrição |
|--------|--------|-----------|
| `express` | ^5.0.1 | Framework web para Node.js - Roteamento e middleware |
| `axios` | ^1.7.9 | Cliente HTTP - Para chamadas de API externas |
| `cors` | ^2.8.5 | Middleware de CORS - Permite requisições cross-origin |
| `helmet` | ^8.0.0 | Segurança HTTP - Define headers de segurança |
| `express-rate-limit` | ^7.5.0 | Middleware de rate limiting - Proteção contra abuso |
| `dotenv` | ^16.4.7 | Carregamento de variáveis de ambiente (.env) |

### **Dependências de Desenvolvimento**

| Pacote | Versão | Descrição |
|--------|--------|-----------|
| `nodemon` | ^3.1.9 | Reinicia servidor automaticamente em mudanças |

---

## 📊 Tecnologias Identificadas

### **Backend**
- **Runtime:** Node.js
- **Framework:** Express.js 5.0.1
- **HTTP Client:** Axios
- **Segurança:** 
  - Helmet (headers de segurança)
  - CORS (controle de origem)
  - Rate Limiting (proteção contra bots)
- **Configuração:** Variáveis de ambiente (dotenv)

### **Frontend**
- ✅ **React** 18.3.1 - Framework UI
- ✅ **React DOM** 18.3.1 - Renderização de componentes
- ✅ **Vite** 6.0.11 - Build tool ultra-rápido
- ✅ **React Router DOM** 7.1.3 - Roteamento
- ✅ **Zustand** 5.0.3 - State Management (leve, sem boilerplate)
- ✅ **Axios** 1.7.9 - Requisições HTTP
- ✅ **TypeScript** types instalados

---

## ✅ O que está Implementado

✅ Configuração inicial do Express.js no backend  
✅ Middleware de segurança e CORS no backend  
✅ Estrutura básica de dependências do backend  
✅ Suporte a variáveis de ambiente (dotenv)  
✅ Inicialização do frontend com React 18.3.1  

---

## ⚠️ O que Falta Implementar

### **Backend (Prioritário)**

- [ ] **Inicializar Express.js em `app.js`**
  - Configurar portas e middleware
  - Testes básicos de conexão

- [ ] **Banco de Dados**
  - MongoDB/PostgreSQL/MySQL para armazenar músicas, usuários, playlists
  - ORM/ODM (Sequelize, Mongoose, Prisma)

- [ ] **Autenticação**
  - JWT (jsonwebtoken)
  - bcryptjs para hashing de senhas
  - Estratégias OAuth (Google, Spotify API)

- [ ] **Funcionalidades Core**
  - Rotas de usuários (registro, login)
  - Rotas de músicas/álbuns
  - Rotas de playlists
  - Rotas de busca
  - Sistema de likes/favoritos

- [ ] **Validação**
  - express-validator ou joi
  - Middleware de validação de entrada

- [ ] **Testing**
  - Jest ou Mocha
  - Supertest para testes de API

- [ ] **Logging**
  - Morgan ou winston
  - Monitoramento de erros

### **Frontend (Inicializado - Próximos Passos)**

- [ ] Instalar dependências adicionais
  - React Router v6+
  - Axios para requisições
  - State Management (Redux ou Context API)
  - UI Library (Material-UI, Tailwind CSS)

- [ ] Scaffolding do projeto
  - Estrutura de pastas (src/components, src/pages, src/services)
  - Arquivo index.js e App.js

- [ ] Componentes UI principais
  - Navigation/Header
  - Sidebar
  - Player de música
  - Search bar

- [ ] Integração com API backend
- [ ] Sistema de autenticação
- [ ] Player de música funcional
- [ ] Gerenciamento de estado

### **DevOps & Deployment**

- [ ] Docker/Dockerfiles
- [ ] CI/CD (GitHub Actions)
- [ ] Deploy em produção
- [ ] Configuração de variáveis de ambiente (.env)

---

## 🚀 Próximas Etapas Recomendadas

### **Fase 1 - Backend Foundation (URGENTE - 1-2 horas)**
1. ✅ Backend package.json configurado com Express 5.0.1
2. ⏳ **Criar `backend/src/server.js`** como entry point
3. ⏳ **Implementar `backend/src/app.js`** com Express + middlewares
4. ⏳ Criar `backend/.env` com PORT=3001
5. ⏳ Testar: `npm run dev` → curl http://localhost:3001/api/health
6. Configurar banco de dados (MongoDB recomendado para MVP)
7. Implementar autenticação com JWT
8. Criar modelos de dados (User, Music, Playlist)
9. Desenvolver rotas básicas CRUD

### **Fase 2 - Frontend Setup (EM PROGRESSO - 1-2 horas)**
1. ✅ React 18.3.1 + Vite 6.0.11 + Zustand 5.0.3 instalados
2. ⏳ **Criar estrutura Vite:**
   - `frontend/index.html` (template HTML)
   - `frontend/src/main.jsx` (entry point)
   - `frontend/src/App.jsx` (componente raiz)
   - `frontend/vite.config.js` (configuração)
3. ⏳ Criar pastas: `src/components/`, `src/pages/`, `src/services/`, `src/store/`
4. ⏳ Testar: `npm run dev` → http://localhost:5173
5. Instalar Tailwind CSS ou Material-UI
6. Configurar roteamento com React Router
7. Criar componentes principais (Header, Sidebar, Player)

### **Fase 3 - Integração (1-2 dias)**
1. Configurar axios com baseURL para backend
2. Conectar frontend com API backend
3. Implementar autenticação no frontend
4. Criar player de música funcional
5. Sistema de busca de músicas

### **Fase 4 - Polish & Deploy (1-2 dias)**
1. Testes automatizados (Jest + Supertest backend, Vitest frontend)
2. Otimização de performance
3. Docker & Docker Compose
4. CI/CD com GitHub Actions
5. Deploy em produção

---

## 📦 Dependências Atuais do Projeto

### **Backend** (package.json)
**Produção:**
- express ^5.0.1
- axios ^1.7.9
- cors ^2.8.5
- helmet ^8.0.0
- express-rate-limit ^7.5.0
- dotenv ^16.4.7

**Desenvolvimento:**
- nodemon ^3.1.9

**Engines:** Node.js >=22.12.0, npm >=10.0.0

### **Frontend** (package.json)
**Produção:**
- react ^18.3.1
- react-dom ^18.3.1
- axios ^1.7.9
- react-router-dom ^7.1.3
- zustand ^5.0.3

**Desenvolvimento:**
- vite ^6.0.11
- @vitejs/plugin-react ^4.3.4
- @types/react ^18.3.18
- @types/react-dom ^18.3.5

**Engines:** Node.js >=22.12.0, npm >=10.0.0

---

## 📦 Recomendações de Novas Dependências

### **Para Produção**
```json
{
  "mongoose": "^7.x.x",          // MongoDB ODM
  "jsonwebtoken": "^9.x.x",      // JWT
  "bcryptjs": "^2.x.x",           // Hashing de senhas
  "express-validator": "^7.x.x",  // Validação
  "multer": "^1.x.x",             // Upload de arquivos
  "stripe": "^14.x.x"             // Pagamentos (opcional)
}
```

### **Para Frontend**
```json
{
  "react-router-dom": "^6.x.x",  // Roteamento
  "axios": "^1.x.x",              // Requisições HTTP
  "redux": "^4.x.x",              // State management
  "react-redux": "^8.x.x",        // Integração Redux
  "@mui/material": "^5.x.x",      // Material-UI ou use Tailwind
  "tailwindcss": "^3.x.x"         // Alternativa para CSS utility
}
```

---

## 🔐 Segurança - Checklist

- [ ] Variáveis sensíveis em `.env` (já configurado com dotenv)
- [ ] Helmet para headers de segurança (já instalado)
- [ ] CORS configurado corretamente
- [ ] Rate limiting ativo
- [ ] Validação de entrada em todas as rotas
- [ ] Hashing de senhas (bcryptjs)
- [ ] JWT com tempo de expiração
- [ ] HTTPS em produção
- [ ] SQL injection/NoSQL injection prevenção

---

## 📝 Status por Arquivo

### Backend
- **package.json** ✅ Completo - Express + middlewares + scripts
- **src/app.js** ⏳ Vazio - PRÓXIMO: Criar middleware do Express
- **src/server.js** ⏳ Não existe - PRÓXIMO: Criar como entry point
- **node_modules/** ✅ Dependências instaladas
- **.env** ⏳ Não existe - PRÓXIMO: Criar com PORT=3001, etc.

### Frontend
- **package.json** ✅ Completo - React + Vite + Zustand + Router + Axios
- **node_modules/** ✅ Dependências instaladas
- **src/** ⏳ Não existe - PRÓXIMO: Criar estrutura Vite
- **public/** ⏳ Não existe - PRÓXIMO: Assets públicos
- **index.html** ⏳ Não existe - PRÓXIMO: Template HTML
- **vite.config.js** ⏳ Não existe - PRÓXIMO: Configuração Vite

---

## 📝 Observações Importantes

1. **Backend `app.js` vazio:** 🔴 URGENTE - Implementar Express com middlewares
2. **Backend `src/server.js` não existe:** 🔴 URGENTE - Criar como entry point
3. **Frontend estrutura Vite não criada:** 🟡 Vite instalado, mas sem arquivos base (main.jsx, App.jsx, index.html)
4. **Database não configurado:** Escolher MongoDB ou PostgreSQL + ORM
5. **Autenticação não implementada:** JWT e bcryptjs ainda não instalados
6. **Vite escolhido em vez de Create React App:** Muito mais rápido e moderno ✅
7. **Zustand escolhido em vez de Redux:** Mais simples e leve para este projeto ✅
8. **Sem testes:** Jest + Supertest (backend), Vitest + React Testing Library (frontend)
9. **Sem logging estruturado:** Morgan ou Winston para logs HTTP

---

## 🎵 Funcionalidades do Spotify Clone Esperadas

- Busca de músicas/artistas
- Criar/editar playlists
- Like/Favoritar músicas
- Reprodutor de música
- Histórico de reprodução
- Recomendações personalizadas
- Modo offline (opcional)
- Compartilhamento de playlists

---

## 📞 Próxima Ação Imediata

### 🚨 **PRIORITY 1 - HOJE (Backend - 30 min)**
1. Criar `backend/src/server.js`
2. Implementar `backend/src/app.js` com Express + middlewares
3. Criar `backend/.env` com PORT=3001
4. Testar: `npm run dev` → GET http://localhost:3001/api/health

### 🟡 **PRIORITY 2 - HOJE (Frontend - 30 min)**
1. Criar `frontend/index.html`
2. Criar `frontend/src/main.jsx`
3. Criar `frontend/src/App.jsx`
4. Criar `frontend/vite.config.js`
5. Testar: `npm run dev` → http://localhost:5173

### 🟢 **PRIORITY 3 - AMANHÃ (Database & Auth)**
1. Escolher MongoDB ou PostgreSQL
2. Instalar Mongoose ou Prisma
3. Implementar autenticação JWT
4. Criar modelos de dados

**Estimativa:** Backend + Frontend base em 1-2 horas ✅
