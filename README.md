# 🟦 PROACTIVA  
### Plataforma Inteligente para Capacitação e Inclusão no Futuro do Trabalho

---

## 📘 Descrição do Projeto

O **Proactiva** é uma aplicação SPA (Single Page Application) desenvolvida em **React + TypeScript + Vite**, criada para apoiar usuários na adaptação ao futuro do trabalho, oferecendo conteúdos personalizados, funcionalidades acessíveis e integração completa com API em Java (Quarkus).  

O objetivo principal é criar uma plataforma intuitiva, responsiva e acessível que permita aos usuários explorarem oportunidades de aprendizado, acompanharem trilhas de capacitação e se conectarem com novas possibilidades profissionais.

---

## 📑 Sumário

1. [Sobre o Projeto](#-sobre-o-projeto)
2. [Tecnologias Utilizadas](#-tecnologias-utilizadas)
3. [Instalação](#-instalação)
4. [Como Usar](#-como-usar)
5. [Estrutura de Pastas](#-estrutura-de-pastas)
6. [Endpoints ou Rotas Principais](#-endpoints-ou-rotas-principais)
7. [Autores e Créditos](#-autores-e-créditos)
8. [Screenshots / Demonstração](#-screenshots--demonstração)

---

## 🎯 Sobre o Projeto

O ProActiva foi desenvolvido como parte da **Global Solution** da FIAP, integrando conhecimentos de:

- **Front-End Design Engineering** (React + Vite + TypeScript)
- **Domain Drive Design Using Java** (API REST)
- **Building Relational Database** (Banco de Dados)

### Problema Identificado

Empresas enfrentam desafios crescentes relacionados ao bem-estar dos colaboradores:
- Burnout e estresse ocupacional
- Falta de dados objetivos sobre saúde mental
- Dificuldade em identificar problemas precocemente
- Ausência de ferramentas de monitoramento contínuo

### Solução Proposta

O ProActiva oferece:
- **Timer de Foco** para auxilio das tarefas
- **Técnica de Respiração** para ajudar a acalmar 
- **Dashboard interativo** com estatísticas em tempo real
- **Histórico completo** de avaliações
- **Mensagens personalizadas** baseadas no IBE (Índice de Bem-Estar)
- **Integração com API Java** para armazenamento seguro

### Benefícios

- ✅ Identificação precoce de problemas
- ✅ Dados objetivos para tomada de decisão
- ✅ Acompanhamento longitudinal
- ✅ Interface intuitiva e responsiva
- ✅ Feedback personalizado para colaboradores

---

## 🛠 Tecnologias Utilizadas

O projeto foi desenvolvido com foco em modularidade, escalabilidade e performance, utilizando:

### **Frontend**
- **React** — UI declarativa baseada em componentes  
- **Vite** — build e dev server ultra rápidos  
- **TypeScript** — tipagem estática para segurança  
- **TailwindCSS** — estilização utilitária e responsiva  
- **React Router DOM** — gerenciamento de rotas SPA  
- **Context API** — gerenciamento global (tema, acessibilidade, etc.)  
- **Fetch API** — comunicação com a API Java (sem Axios, conforme regras)

---

## 📌 Status do Projeto – Global Solution 2025/2

A Sprint final contemplou:

- Consumo da API remota (CRUD completo)
- Implementação de rotas dinâmicas
- Tema escuro/claro com **Context API**
- Páginas obrigatórias (Home, Sobre, FAQ, Integrantes)
- Deploy na **Vercel**
- Versionamento com **GitFlow**

---

## 💻 Instalação

### Pré-requisitos

- Node.js  instalado
- npm instalado
- Git instalado

### Passo a Passo

1. **Clone o repositório**
```bash
git clone https://github.com/deryksouza2006/proactivaAPI.git
cd ProActiva
```

2. **Instale as dependências**
```bash
npm install
```

3. **Inicie o servidor de desenvolvimento**
```bash
npm run dev
```

4. **Acesse a aplicação**
```
http://localhost:5173
```

---

## 🎮 Como Usar

### Acesso Online

Acesse a aplicação em produção:
**URL:** [https://pro-activa-tuac.vercel.app/](https://pro-activa-tuac.vercel.app/)

### Fluxo de Uso

#### 1. Página Inicial
- Acesse a home para conhecer o projeto
- Navegue pelo menu para explorar funcionalidades

#### 2. Cadastrar tarefa
1. Acesse `/dashboard/tarefas`
2. Adicione uma nova tarefa com:
   - Título 
   - Descrição
   - Categoria
   - Prioridade
   - Data de Vencimento
3. Conclua, edite ou exclua a tarefa

#### 3. Timer de foco
1. Acesse `/dashboard/timer`
2. Ações do Timer:
   - Iniciar Timer
   - Configurar para o tempo desejado
   - Resetar
   - Mensagem personalizada
3. O timer mostra:
    - Sessões de Hoje
    - Tempo total
    - Progresso

#### 4. Respiração
1. Acesse `/dashboard/respiracao`
    - Pratique a respiração

## 📁 Estrutura de Pastas do Projeto

A estrutura segue padrões de componentização, separação de responsabilidades e modularidade:

```
proactiva/
├── eslint.config.js
├── index.html
├── package.json
├── public/
│   └── assets/
├── src/
│   ├── App.tsx
│   ├── App.css
│   ├── assets/
│   │   └── images/ (ícones e imagens do projeto)
│   ├── components/ (componentes reutilizáveis)
│   ├── context/ (tema, acessibilidade, global state)
│   ├── pages/ (páginas da aplicação)
│   │   ├── Home.tsx
│   │   ├── FAQ.tsx
│   │   ├── About.tsx
│   │   ├── Integrantes.tsx
│   │   ├── Cursos.tsx
│   │   └── CursoDetalhe.tsx
│   ├── services/
│   │   └── apiService.ts (módulo de comunicação fetch)
│   ├── routes/
│   ├── types/
│   ├── main.tsx
│   └── index.css
├── tsconfig.json
└── vite.config.ts
```

---

## 🛣️ Endpoints ou Rotas Principais

### Rotas do Frontend

| Rota | Descrição | Tipo |
|------|-----------|------|
| `/` | Página inicial | Pública |
| `/login` | Login de usuário | Pública |
| `/cadastro` | Cadastro de usuário | Pública |
| `/dashboard/tarefas` | Gerenciador de tarefas | Privada |
| `/dashboard` | Dashboard com estatísticas | Privada |
| `/dashboard/timer` | Timer de foco | Privada |
| `/integrantes` | Página de integrantes | Pública |
| `/sobre` | Sobre o projeto | Pública |
| `/faq` | Perguntas frequentes | Pública |
| `/contato` | Contato | Pública |
| `/dashboard/perfil` | Perfil | Privada |


## 👥 Autores e Créditos

### Equipe de Desenvolvimento

#### Deryk de Souza Queiroz
- **RM:** RM563412
- **Turma:** 1TDSPX
- **GitHub:** [github.com/deryksouza2006](https://github.com/deryksouza2006)
- **LinkedIn:** [linkedin.com/in/deryksouza/](https://www.linkedin.com/in/deryksouza/)

#### Vinicius Paschoeto da Silva
- **RM:** RM563089
- **Turma:** 1TDSPX
- **GitHub:** [github.com/pasva01](https://github.com/pasva01)
- **LinkedIn:** [linkedin.com/in/vin%C3%ADcius-paschoeto-785009349/](https://www.linkedin.com/in/vin%C3%ADcius-paschoeto-785009349/)

#### Lucas Gonçalves Viana
- **RM:** RM563254
- **Turma:** 1TDSPX
- **GitHub:** [github.com/LucasViana130](https://github.com/LucasViana130)
- **LinkedIn:** [linkedin.com/in/lucas-viana-262068367/](https://www.linkedin.com/in/lucas-viana-262068367/)


### Agradecimentos

- **FIAP** - Instituição de ensino
- **Professores** - Orientação e suporte
- **Comunidade Open Source** - Ferramentas e bibliotecas

---

### Vídeo de Demonstração

🎥 **Vídeo de demonstração**
[https://youtu.be/jM7hgQP6cdU](https://youtu.be/jM7hgQP6cdU)
---

## 📄 Licença

Este projeto foi desenvolvido para fins acadêmicos como parte da Global Solution da FIAP.

---

## 🔗 Links Importantes

- **Repositório GitHub:** [https://github.com/deryksouza2006/proactivaAPI.git](https://github.com/deryksouza2006/proactivaAPI.git)
- **Aplicação em Produção:** [https://pro-activa-tuac.vercel.app/](https://pro-activa-tuac.vercel.app/)
- **API Java:** [https://proactivaapi.onrender.com](https://proactivaapi.onrender.com)

---