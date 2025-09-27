🚀 NexTraceWeb
NexTraceWeb é uma plataforma de rastreamento, sanitização e proteção de dados sensíveis em aplicações Python, com foco em ambientes Django.
Criada por um desenvolvedor independente, sem verba, sem equipe — apenas com propósito, visão e código.
Segurança não é um recurso. É uma cultura.
NexTraceWeb existe para proteger quem constrói.

📦 Componentes do Sistema
O projeto é composto por três repositórios integrados:
 
Repositório                    Função Principal

nextraceweb_backend     -->    API REST, sanitização, autenticação
nextraceweb_frontend    -->    Interface web responsiva e segura
nextraceweb             -->    Orquestração via Docker, documentação

🧠 Backend (API)
- Linguagem: Python 3.13
- Framework: Django
- Sanitização: Scanner de arquivos .py com limpeza automática
- Autenticação: JWT com controle de sessão
- Relatórios: Logs detalhados com rastreamento de ocorrências
- Testes: pytest com cobertura de segurança
- Ambiente: venv, requirements.txt, .env
- Licenciamento: Módulo de ativação por chave (25 dígitos), com validação pós-pagamento

💻 Frontend (Interface Web)
- Linguagem: JavaScript
- Framework: React.js
- Build Tool: Vite
- Estilo: Tailwind CSS
- Integração: Consumo da API via Axios
- Deploy: Firebase Hosting ou Docker
- Licenciamento: Interface de ativação com chave virtual

🐳 Infraestrutura & DevOps
- Docker: Containers isolados para frontend e backend
- Docker Compose: Orquestração dos serviços
- Portainer: Gerenciamento visual via navegador
- GitHub Actions: CI/CD automatizado
- UptimeRobot: Monitoramento em tempo real
 
🔐 Segurança
- Variáveis sensíveis via .env, protegidas por .gitignore
- Sanitização de código: busca por tokens, senhas, chaves e dados pessoais
- Logs de rastreamento com timestamp, tipo de dado e ação tomada
- Licenciamento obrigatório para uso completo do sistema

📊 Monitoramento & Deploy
- Status em tempo real via UptimeRobot
- Deploy automatizado com GitHub Actions
- Hospedagem alternativa: Vercel, Firebase, ou VPS via Docker
📈 Último status:
- 🔴 nextraceweb.vercel.app ficou fora do ar por 9h38min (erro 404)
- 🟢 Voltou ao ar há 22h32min — uptime geral: 72.86% nas últimas 24h

🚀 Como rodar localmente
git clone https://github.com/diogofelde/nextraceweb.git
cd nextraceweb

# Subir tudo com Docker
docker-compose up --build -d

# Backend: http://localhost:3000
# Frontend: http://localhost:5173

🔑 Licenciamento
O NexTraceWeb requer ativação para uso completo.
Após aquisição, o usuário recebe uma chave de licença de 25 dígitos, semelhante ao modelo de ativação do Windows.
Exemplo:
XXXX-XXXX-XXXX-XXXX-XXXXX
A chave é validada automaticamente via API e libera o sistema para uso.
Licenças podem ser adquiridas diretamente com o autor ou via plataforma de distribuição (em desenvolvimento).

🤝 Apoie este projeto
Este sistema está sendo desenvolvido sem patrocínio, sem verba, sem equipe — apenas com dedicação e propósito.
Se você acredita em segurança acessível e quer apoiar um projeto independente:
- 💸 Faça uma doação via Pix: diogo.felde@gmail.com
- 🧑‍💼 Patrocine via GitHub Sponsors (em breve)
- 📢 Compartilhe com sua rede
Toda ajuda é bem-vinda — e será usada para manter o projeto vivo, seguro e gratuito.

👨‍💻 Autor
Diogo Felde Ferreira
Analista em Segurança da Informação
Desenvolvedor Python & Front-end
- GitHub: github.com/diogofelde
- LinkedIn: linkedin.com/in/diogofelde
- E-mail: diogofelde@gmail.com

📄 Licença
Este projeto utiliza um modelo de licenciamento proprietário com ativação digital.
O código-fonte está disponível para fins educacionais e demonstração, mas o uso completo requer chave de ativação.

🏁 Roadmap
- [x] Backend com sanitização e autenticação
- [x] Frontend integrado com interface de ativação
- [x] Orquestração com Docker Compose
- [x] Painel de administração
- [x] Exportação de relatórios em PDF
- [x] Modo CLI para uso em pipelines
- [ ] Integração com GitHub Secrets
- [ ] Sistema de compra e ativação de licenças








