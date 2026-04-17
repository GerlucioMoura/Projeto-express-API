# Projeto Express API com Prisma + MongoDB

Este projeto é uma API REST desenvolvida com **Node.js**, **Express** e **Prisma**, utilizando **MongoDB Atlas** como banco de dados.  
Ela implementa um CRUD completo para gerenciar usuários.

---

## 🚀 Tecnologias utilizadas
- Node.js
- Express
- Prisma ORM
- MongoDB Atlas
- Nodemon (para desenvolvimento)

---

## 📂 Estrutura do projeto

Projeto-express-API/
├── prisma/
│   ├── schema.prisma
│   └── prisma.config.ts
├── server.js
├── package.json
└── .env

---

## ⚙️ Instalação e execução

1. Clone o repositório:
   ```bash
   git clone https://github.com/seuusuario/Projeto-express-API.git
   cd Projeto-express-API

2. Instale as dependências:
   npm install
   
3. Configure o arquivo .env com sua conexão MongoDB:
  DATABASE_URL="mongodb+srv://gerlucio_db_user:SUA_SENHA@cluster0.lezdn17.mongodb.net/projeto_api?retryWrites=true&w=majority"
 
4. Gere o cliente Prisma:
 npx prisma generate

5. Execute o servidor:
   npm run dev

O servidor estará rodando em:
http://localhost:8080

📌 Endpoints da API
Rota inicial
GET /  
Retorna mensagem de status da API.

Usuários
Listar todos
GET /usuarios  
Retorna todos os usuários cadastrados.

Buscar por ID
GET /usuarios/:id  
Retorna um usuário específico pelo ID.

Criar usuário
POST /usuarios  
Cria um novo usuário.

Body (JSON):

{
  "nome": "João",
  "email": "joao@email.com",
  "age": 25
}

Atualizar usuário (PUT)
PUT /usuarios/:id  
Atualiza todos os campos de um usuário.

Body (JSON):

{
  "nome": "João Silva",
  "email": "joao@novo.com",
  "age": 30
}

Atualizar parcialmente (PATCH)
PATCH /usuarios/:id  
Atualiza apenas os campos enviados.

Body (JSON):

{
  "email": "joao@editado.com"
}

Deletar usuário
DELETE /usuarios/:id  
Remove um usuário pelo ID.

🛠️ Ferramentas de teste
Thunder Client (VS Code)

Postman

MongoDB Compass (para visualizar os dados no banco)

📖 Próximos passos
-Implementar autenticação (JWT).
-Adicionar validações mais robustas.
-Criar testes automatizados.







  
