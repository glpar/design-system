# Design System

Monorepo de um design system para aplicações React. Reúne tokens visuais, componentes reutilizáveis, configurações compartilhadas e uma documentação interativa no Storybook.

## Conteúdo

- `packages/tokens`: cores, tipografia, espaçamentos, raios e alturas de linha;
- `packages/react`: componentes como Button, Text, Heading, Box, Avatar, Checkbox, TextInput, TextArea e MultiStep;
- `packages/docs`: documentação e exemplos no Storybook;
- `packages/eslint-config`: configuração compartilhada do ESLint;
- `packages/ts-config`: configurações compartilhadas do TypeScript.

## Tecnologias

React, TypeScript, Storybook, Stitches, Radix UI, tsup, Turborepo e Changesets.

## Como instalar e executar

### Pré-requisitos

- Node.js 18 ou superior;
- npm.

```bash
git clone https://github.com/glpar/design-system.git
cd design-system
npm install
npm run dev
```

O Turborepo inicia os pacotes em modo de desenvolvimento. A documentação do Storybook fica normalmente em `http://localhost:6006`.

Para executar apenas o Storybook:

```bash
cd packages/docs
npm run dev
```

## Build

```bash
npm run build
```

Esse comando gera os pacotes de tokens e componentes e também a versão estática do Storybook.

## Fluxo de versionamento

```bash
npm run changeset
npm run version-packages
```

O Changesets registra alterações e prepara as versões dos pacotes. A publicação em um registro npm exige autenticação e configuração próprias.

