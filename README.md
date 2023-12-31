# Teste de Automação

Este projeto contém um boilerplate para criar um teste automatizado para o site https://todomvc.com/ usando a biblioteca Playwright em TypeScript.

## Pré-requisitos

Antes de executar o teste automatizado, você precisa ter instalado o Node.js e o gerenciador de pacotes npm (Node Package Manager) no seu sistema.

## Stack
- Playwright
- TypeScript

## Estrutura
```
projeto
│
├── node_modules
│   ├── (dependências do projeto)
│   └── ...
│
├── playwright-report
│   ├── index.html
│   └── ...
│
├── tests
│   ├── fixture
│   │   ├── task.model.ts
│   │   └── task.json
│   │
│   ├── spec
│   │   ├── tasks.spec.ts
│   │   └── ...
│   │
│   └── support
│       ├── pages
│       │   ├── tasksPages.ts
│       │   └── ...
│       ├── helpers.ts
│       └── ...
│
├── utils
│   ├── .env
│   └── ...
│
├── package-lock.json
├── package.json
├── README.md
└── playwright.config.ts
```
.



## Instalação

1. Clone o repositório ou crie um novo diretório para o projeto:

```bash
git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio
```
.

Necessário instalar o node, disponivel no site:
```
https://nodejs.org/en/download/
```

Instalação do PlayWright:
```
npm init playwright@latest
```

Executar os testes:
```
npx playwright test
```

## Gerando Relatório do Teste Executados

Após a execução do teste automatizado, um relatório em HTML será gerado para facilitar a visualização dos resultados. O relatório é criado automaticamente e estará disponível na pasta reports após a conclusão do teste.

```
 npx playwright show-report
```

## Integração Contínua com GitHub Actions

Este projeto está configurado com o GitHub Actions para automatizar a execução dos testes. Os testes são agendados para serem executados em horários específicos usando uma expressão cron.

### Agenda dos Testes

Os testes serão executados nos seguintes horários todos os dias:

- 9:00 AM
- 12:00 PM
- 3:00 PM
- 6:00 PM
- 9:00 PM






