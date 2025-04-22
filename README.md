# 💾Preservação Digital de Documentos
[![React](https://img.shields.io/badge/React-17.0-blue)](https://reactjs.org/) [![NestJS](https://img.shields.io/badge/NestJS-8.0-red)](https://nestjs.com/)
[![Prisma](https://img.shields.io/badge/Prisma-2.23-green)](https://www.prisma.io/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-13-orange)](https://www.postgresql.org/)
[![Docker](https://img.shields.io/badge/Docker-20-blue)](https://www.docker.com/)

Projeto realizado para trazer uma solução para o desafio de arquivamento de documentos de forma segura usando a API da Archivemetica. Nele temos um fluxo de autenticação de usuário com JWT e Bcrypt, e seguimos utilizando a api da Archivemetica para fazer as chamadas e realizar as operações da nossa api.

### Tópicos
🔹 [Estrutura do projeto](#-estrutura)

🔹 [Pré-requisitos](#-pré-requisitos)

🔹 [Como rodar](#-como-rodar)

🔹 [Integração com Archivematica](#integração-com-o-arquivemetica)

🔹 [Linguagens, dependências e libs utilizadas](#-linguagens-dependências-e-libs-utilizadas)

## 📁 Estrutura

- `/frontend`: Interface em React (Vite)
- `/backend`: API NestJS + Prisma
- `docker-compose.yml`: Utilização de Docker
- `.env.example`: Variáveis de ambiente

## 📀 Pré-requisitos
- Node.js (v16 ou superior)
- npm ou yarn
- Docker e Docker Compose
- Git

## 🚀 Como rodar
1. **Clone o repositório**
   ```bash
   git clone [https://github.com/juliamenzss/preservacao-digital-fullstack]
   cd preservacao-digital-fullstack

2. **Copie o arquivo `.env.example` para `.env`**
```bash
Edite o arquivo .env com suas configurações.
```
3. **Inicie os container com o Docker**
```bash
docker-compose up --build
```

## 🔐Integração com o Arquivemetica
O backend utiliza as funcionalidades da Archivematica via API.

📌 Requisitos:
O Archivematica deve estar rodando em sua máquina local ou via Docker.

Veja como instalar seguindo os passos da documentação oficial a seguir: https://github.com/artefactual/archivematica/blob/qa/1.x/hack/README.md

## Configure as aplicações 
### 🎨 Acesse o frontend: http://localhost:3000
Configure a aplicação
```bash
cd preservacao-digital-frontend
npm install
npm run dev
```
### ⚙️ Acesse o backend: http://localhost:3001
Configure a aplicação
```bash
cd backend
npm install
npx prisma migrate dev
npm run start:dev
```

## 📚 Linguagens, dependências e libs utilizadas

**Frontend:**
React,
Vite,
TypeScript,
Material UI,
React Router,
React Redux,
Axios

**Backend:**
NestJS,
TypeScript,
Prisma,
Bcripty,
JWT

**DevOps:**
Docker,
Docker-Compose,
PostgreSQL)

**Integração:**
Archivematica API 
