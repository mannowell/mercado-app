# 🛒 Mercado App

[![Build Status](https://img.shields.io/github/actions/workflow/status/mannowell/mercado-app/ci.yml?style=flat-square)](https://github.com/mannowell/mercado-app/actions)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT)
[![Version](https://img.shields.io/github/v/release/mannowell/mercado-app?style=flat-square)](https://github.com/mannowell/mercado-app/releases)
[![Ionic](https://img.shields.io/badge/Ionic-8.0-3880FF?style=flat-square&logo=ionic&logoColor=white)](https://ionicframework.com/)
[![Vue](https://img.shields.io/badge/Vue-3.4-4FC08D?style=flat-square&logo=vue.js&logoColor=white)](https://vuejs.org/)
[![Pinia](https://img.shields.io/badge/Pinia-3.0-FFC107?style=flat-square)](https://pinia.vuejs.org/)

> Aplicativo completo de gerenciamento de supermercado com Ionic Vue 8, Pinia para estado global e SQLite para armazenamento local.

---

## ✨ Funcionalidades

- 📋 **Listas de Compras Avançadas** — Crie, edite e organize múltiplas listas de compras com itens detalhados
- 🛍️ **Catálogo de Produtos** — Gerencione produtos com preços, categorias e marca
- 🏪 **Gerenciamento de Mercados** — Cadastre e compare preços entre diferentes supermercados
- 💾 **Armazenamento Local SQLite** — Seus dados ficam salvos offline com SQLite
- 🧮 **Cálculo Automático** — Total automático da compra com base nos itens adicionados
- 📊 **Histórico** — Acompanhe suas compras anteriores
- 📱 **Multiplataforma** — Android, iOS e Web (PWA)

---

## 🛠️ Tecnologias

- **[[Ionic](https://ionicframework.com/)]** 8.0 — Framework de componentes mobile
- **[[Vue.js](https://vuejs.org/)]** 3.4 — Framework progressivo para UI
- **[[Pinia](https://pinia.vuejs.org/)]** 3.0 — Gerenciamento de estado
- **[[Capacitor SQLite](https://github.com/capacitor-community/sqlite)]** 7.0 — Banco de dados local
- **[[Vue Router](https://router.vuejs.org/)]** 4.2 — Roteamento oficial
- **[[TypeScript](https://www.typescriptlang.org/)]** 5.3 — Tipagem estática
- **[[Vite](https://vitejs.dev/)]** 5.0 — Build tool
- **[[Sass](https://sass-lang.com/)]** 1.70 — Estilos CSS
- **[[Cypress](https://www.cypress.io/)]** 13.6 — Testes end-to-end
- **[[Vitest](https://vitest.dev/)]** 1.2 — Testes unitários

---

## 📋 Pré-requisitos

- **Node.js** 18+
- **npm** 9+ ou **yarn**
- **Android Studio** (para Android)
- **Xcode** (para iOS — apenas macOS)
- **JDK 17+** (para desenvolvimento Android)

---

## 🚀 Instalação e Execução

```bash
# Clone o repositório
git clone https://github.com/mannowell/mercado-app.git
cd mercado-app

# Instale as dependências
npm install

# Execute em modo desenvolvimento
npm run dev

# Build de produção
npm run build

# Verificação de tipos
npm run type-check

# Executar testes unitários
npm run test:unit

# Executar testes unitários com coverage
npm run test:unit:coverage

# Executar testes e2e
npm run test:e2e

# Obrir testes e2e interativos
npm run test:e2e:open
```

---

## 📁 Estrutura do Projeto

```
mercado-app/
├── android/                    # Projeto Android nativo
├── src/
│   ├── components/            # Componentes reutilizáveis
│   │   └── MenuLateral.vue
│   ├── views/                 # Páginas da aplicação
│   │   ├── HomePage.vue
│   │   ├── ListaComprasView.vue
│   │   ├── DetalhesListaView.vue
│   │   ├── NovaListaView.vue
│   │   ├── ProdutosView.vue
│   │   └── MercadosView.vue
│   ├── stores/                # Estado global (Pinia)
│   │   └── modules/
│   │       ├── index.ts
│   │       ├── auth.ts
│   │       ├── markets.ts
│   │       ├── products.ts
│   │       └── shoppingLists.ts
│   ├── services/              # Serviços
│   │   └── DatabaseService.ts
│   ├── types/                 # Definições de tipos
│   │   └── index.ts
│   ├── router/                # Configuração de rotas
│   │   └── index.ts
│   ├── theme/                 # Tema CSS
│   │   └── variables.css
│   ├── main.ts               # Entry point
│   └── App.vue               # Componente raiz
├── public/                    # Assets públicos
├── tests/                     # Testes
├── docs/                      # Documentação extra
├── .github/                   # Configuração GitHub
├── capacitor.config.ts        # Configuração Capacitor
├── vite.config.ts             # Configuração Vite
├── vitest.config.ts           # Configuração Vitest
└── package.json               # Dependências
```

---

## 🔌 Principais Telas

| Tela | Descrição |
|------|-----------|
| **Home** | Dashboard com resumo das compras e atalhos |
| **Listas de Compras** | Visualização e gerenciamento de todas as listas |
| **Detalhes da Lista** | Visualização detalhada com itens e totais |
| **Nova Lista** | Criação de nova lista de compras |
| **Produtos** | Catálogo de produtos cadastrados |
| **Mercados** | Lista de supermercados cadastrados |

---

## 📱 Build para Plataformas

```bash
# Adicionar plataforma Android
npx cap add android

# Adicionar plataforma iOS
npx cap add ios

# Sincronizar projeto web com nativo
npx cap sync

# Compilar versão de release (Android)
npx cap build android

# Abrir no Android Studio
npx cap open android

# Abrir no Xcode
npx cap open ios
```

---

## 🤝 Contribuindo

1. Faça um **fork** do projeto
2. Crie uma branch para sua feature: `git checkout -b feature/minha-feature`
3. Commit suas mudanças: `git commit -m 'feat: adiciona nova feature'`
4. Push para a branch: `git push origin feature/minha-feature`
5. Abra um **Pull Request**

---

## 👤 Autor

**Wellison Oliveira (mannowell)**

[![GitHub](https://img.shields.io/badge/GitHub-mannowell-181717?style=flat-square&logo=github)](https://github.com/mannowell)
[![Upwork](https://img.shields.io/badge/Upwork-Wellison%20Oliveira-6FDA44?style=flat-square&logo=upwork)](https://www.upwork.com/freelancers/mannowell)
[![Portfolio](https://img.shields.io/badge/Portfolio-mannowell.github.io-FF6B35?style=flat-square)](https://mannowell.github.io)

---

## 📄 Licença

Este projeto está sob a licença **MIT**. Veja o arquivo [LICENSE](./LICENSE) para mais detalhes.

---

<p align="center">
  Desenvolvido com ❤️ por <a href="https://github.com/mannowell">Wellison Oliveira</a>
</p>
