# 🚀 NexTraceWeb — Deploy & Infraestrutura

Sistema dividido em:

- `frontend/` → React + Vite (Vercel)
- `backend/` → Node.js + Express + Sequelize (Render)
- `docker-compose.yml` → Banco PostgreSQL local (opcional)

---

## 📦 Estrutura do Backend

- `/controllers` → Lógica de autenticação e usuários
- `/models` → Definição das tabelas via Sequelize
- `/routes` → Rotas protegidas e públicas
- `/middlewares` → Validação de token JWT
- `/config` → Conexão com banco de dados

---

## 🛠️ Rodar localmente

```bash
# Backend
cd backend
npm install
npm start

# Testar rota de saúde
GET http://localhost:3000/health

🐳 Docker
# Backend
docker build -t nextraceweb_backend .
docker run -p 3000:3000 nextraceweb_backend

🔧 Render (Backend)
- Root directory: backend
- Start command: node server.js
- Environment: Node
- Variáveis de ambiente:
DB_NAME=nextrace
DB_USER=postgres
DB_PASS=senha123
DB_HOST=db
JWT_SECRET=segredoSuperSecreto
PORT=3000

💻 Vercel (Frontend)
- Root directory: frontend
- Framework preset: Vite
- Variáveis de ambiente:
NODE_ENV=production
VITE_API_URL=https://seu-backend.onrender.com

🔑 Licenciamento
A API valida a chave de ativação enviada pelo frontend. Sem chave válida, o acesso é bloqueado.

🧪 Teste rápido
- Acesse: https://seu-frontend.vercel.app/login
- Faça login
- Verifique se o dashboard carrega os dados
- Teste a rota /api/me com token JWT

📡 Monitoramento
Use UptimeRobot para monitorar:
- Backend: https://seu-backend.onrender.com/health
- Frontend: https://seu-frontend.vercel.app

🤝 Apoie este projeto
Este backend está sendo desenvolvido com dedicação total e sem recursos externos.
- 💸 Pix: diogo.felde@gmail.com
- 🧑‍💼 GitHub Sponsors (em breve)

