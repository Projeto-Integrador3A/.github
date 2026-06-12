# Projeto Integrador 3A --> To-do App

Aplicativo mobile de lista de tarefas desenvolvido como projeto integrador do curso de Ciência da Computação do IESB.

## Sobre o projeto
O Todo App é um aplicativo mobile que permite ao usuário gerenciar suas tarefas do dia a dia, organizadas por data. O projeto foi desenvolvido em duas fases:

- **Fase 1:** Construção do Frontend (telas e navegação)
- **Fase 2:** Integração com Backend (API REST e banco de dados)

## Repositórios
- **Frontend:** https://github.com/Projeto-Integrador3A/Front-End
- **Backend:** https://github.com/Projeto-Integrador3A/Back-End
## Tecnologias utilizadas

### Frontend
- React Native
- Expo
- React Navigation
- Axios
- AsyncStorage
- Context API

### Backend
- Node.js
- Express
- PostgreSQL (Neon)
- JWT
- Bcryptjs
- Render (hospedagem)

## Funcionalidades
- Cadastro de usuário
- Login com autenticação JWT
- Listagem de tarefas por data
- Adicionar tarefa com título e data
- Marcar tarefa como concluída
- Deletar tarefa
- Modal com dados do usuário
- Logout

## URL da API
```
https://todo-backend-oiwu.onrender.com
```
> ⚠️ O plano gratuito do Render hiberna após inatividade. A primeira requisição pode demorar até 50 segundos.

## Como rodar o projeto

### Pré-requisitos
- Node.js instalado
- Expo Go instalado no celular ou emulador Android configurado

### 1. Clonar os repositórios
```bash
git clone <link do repositório Front-End>
git clone <link do repositório Back-End>
```

### 2. Rodar o Frontend

```bash
cd Front-End
git checkout final
npm install
npx expo start
```

Abrir no celular escaneando o QR Code com o Expo Go, ou apertar `a` no terminal para abrir no emulador Android.

### 3. Rodar o Backend (opcional)
O backend já está hospedado no Render, não é necessário rodar localmente. Mas se quiser rodar local:

```bash
cd Back-End/final
npm install
```

Criar o arquivo `.env` na raiz da pasta `final`:
```
DATABASE_URL=sua_connection_string_do_neon
JWT_SECRET=seu_jwt_secret
PORT=3000
```
```bash
npm run dev
```

## Estrutura das branches

### Frontend
| Branch | Descrição |
|--------|-----------|
| `davi` | Fase 1 - telas e navegação sem integração |
| `final` | Fase 2 - integração completa com a API |

### Backend
| Branch | Descrição |
|--------|-----------|
| `inicial` | Versão inicial da API |
| `final` | Versão final hospedada no Render |

## Banco de dados
O banco de dados PostgreSQL está hospedado no Neon (nuvem) e compartilhado entre o ambiente local e o Render.

### Tabelas
- **users** → armazena os usuários cadastrados
- **tasks** → armazena as tarefas vinculadas a cada usuário

## Equipe
| Membro | Responsabilidade |
|--------|-----------------|
| Lucca e Iury | Backend - API REST |
| Davi e Caio | Frontend - Integração com a API |

## Instituição
Centro Universitário IESB - Projeto Integrador 3A (CCO089)

Docente: Marcelo Alves Farias
