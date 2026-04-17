# 🚀 Portfólio de Dados & Engenharia — Xavier

Bem-vindo ao meu espaço de experimentação e exposição de projetos! Sou o **Xavier**, estudante de **Engenharia de Software (IFPE)** e entusiasta apaixonado por transformar dados brutos em inteligência estratégica.

Aqui você encontrará a documentação técnica do meu portfólio, focado em soluções robustas com o "DNA de Pernambuco" 🌵☀️.

## 🧑‍💻 Perfil Profissional

Atualmente, dedico meus estudos ao ecossistema de dados, com foco em:
- **Arquitetura Medallion**: Implementação de camadas (Bronze, Silver, Gold) em ambientes GCP (BigQuery).
- **Modelagem de Dados**: Especialista em Star Schema e processos de ETL/ELT.
- **Visualização**: Dashboards avançados em Power BI com DAX complexo para finanças e operações.
- **Inovação Regional**: Membro ativo do ecossistema de empresas juniores via FEJEPE.

---

## 🛠️ Tecnologias e Clean Code (Frontend)
Recentemente, o portfólio passou por uma **refatoração arquitetural intensa** para garantir manutenibilidade, escalabilidade e performance no Frontend:

* **Arquitetura CSS Modular (ITCSS)**: Estilos fragmentados logicamente via `main.css` centralizado (`base`, `components`, `layout`, `utilities` e rotas de `pages`). Redução drástica da redundância e do recarregamento desnecessário do DOM.
* **Componentes de UI / UX**: Tema Dark "Neon Architect" com variáveis globais (CSS Tokens), Glassmorphism, Micro-interaçoes, e Design System independente.
* **Comunicação Assíncrona e Anti-Spam**: O formulário da página de contato (`/pages/contact.html`) possui uma lógica JS avançada isolada que utiliza:
  * Inteface Fetch Nativa (REST API) consumindo o **EmailJS**.
  * **Toast Notifications** dinâmicos que se auto destroem sem travar a thread de Javascript principal.
  * Proteção Anti-Spam (Honeypots invisíveis injetados no DOM limitando web-scrappers básicos).
  * Timestamps Cooldown system (prevenção de flood de requisições).

---

## 📂 Principais Projetos

### 🔋 [Case AutoVolt](pages/projeto-autovolt.html)
Desenvolvimento de uma solução de ponta a ponta para uma fábrica de baterias.
- **Destaque:** Implementação de pipeline de dados usando arquitetura Medallion e criação de dashboard operacional para monitoramento de produção.
- **Skills:** SQL, GCP, Star Schema.

### 💰 [Performance Diária de Vendas](pages/analise-performance-vendas.html)
Modelo Star Schema contendo monitoramentos de faturamento, tickets e margens operacionais.
- **Destaque:** Controle dinâmico unindo planilhas legadas de Excel transformadas e automatizadas em um Flow robusto no PowerBI. 

---

## 🌐 Conecte-se comigo
- **LinkedIn:** [Pedro Xavier](https://www.linkedin.com/in/pedrohenriquereisxavier/)
- **Site:** [xavier9190.github.io](https://xavier9190.github.io/)

---

## 📂 Estrutura do Projeto

```text
├── assets/             # Imagens, ícones e recursos visuais
├── pages/              # Páginas de conteúdo (Cases, Sobre, Contato)
├── scripts/            # Lógica abstrata e isolada em Frontend Javascript (ex: contact.js)
├── styles/
│   └── css/            # Arquitetura ITCSS Modular (Variáveis, Reset, Components Layouts)
│       ├── base/       # Arquivos globais e reset (reset.css, variables.css)
│       ├── components/ # Pedaços reutilizáveis da UI (navbar.css, buttons.css)
│       ├── layout/     # Constraints visuais de contêineres 
│       ├── pages/      # Sobrescritas específicas e únicas de cada view web
│       ├── utilities/  # Modificadores de classes auxiliares 
│       └── main.css    # Ponto de encadeamento da importação principal do site
├── index.html          # Ponto de entrada root
└── README.md           # Documentação técnica do repositório
```
