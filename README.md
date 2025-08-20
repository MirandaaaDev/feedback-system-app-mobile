# 📱 Feedback System App (Mobile)

Aplicativo mobile desenvolvido em **React Native com Expo** para integração com a [Feedback System API](https://github.com/MirandaaaDev/feedback-system-api).  
O app permite que funcionários enviem feedbacks e acompanhem suas interações, enquanto administradores podem visualizar relatórios e informações de forma simplificada.

---

## 🎯 Objetivo e Público-Alvo

O objetivo do app é oferecer uma **interface simples e prática** para que funcionários e administradores utilizem os recursos da API diretamente em seus dispositivos móveis.  

- **Funcionários (EMPLOYEE):** enviar feedbacks, visualizar seus envios e acompanhar status.  
- **Administradores (ADMIN):** visualizar feedbacks, aplicar filtros e acessar estatísticas.  

---

## ✅ Funcionalidades

- 🔐 **Autenticação e Autorização**  
  - Login com token JWT (integração com a API).  
  - Armazenamento do token com AsyncStorage.  

- 💬 **Feedbacks**  
  - Envio de feedback (anônimo ou identificado).  
  - Listagem de feedbacks do usuário.  
  - Visualização filtrada de feedbacks (para admins).  

- 📊 **Relatórios e Consultas**  
  - Visualização de relatórios por setor e data.  
  - Dashboard simplificado para administradores.  

---

## ⚙️ Tecnologias Utilizadas

- [React Native](https://reactnative.dev/)  
- [Expo](https://expo.dev/)  
- [TypeScript](https://www.typescriptlang.org/)  
- [Axios](https://axios-http.com/) – requisições HTTP  
- [React Navigation](https://reactnavigation.org/) – navegação de telas  
- [AsyncStorage](https://react-native-async-storage.github.io/async-storage/) – armazenamento local  

---

## 🛠️ Como Rodar o Projeto

### 🔧 Pré-requisitos

- Node.js 18+  
- npm ou yarn  
- Expo Go instalado no celular *(Android/iOS)*  
- API em execução local (`feedback-system-api`) ou hospedada em servidor  

---

### 🚀 Executando o Projeto

```bash
# Clone o repositório
git clone https://github.com/MirandaaaDev/feedback-system-app-mobile.git

# Acesse a pasta do projeto
cd feedback-system-app-mobile

# Instale as dependências
npm install
# ou
yarn install

# Inicie o projeto com Expo
npx expo start
```

📱 Escaneie o QR Code exibido no terminal (ou na página web que abre automaticamente) com o **app Expo Go** no seu celular.  

---

## 🔐 Configuração da API

O app consome dados da [Feedback System API](https://github.com/MirandaaaDev/feedback-system-api).  

Para alterar a URL base da API, edite o arquivo de configuração (exemplo `src/config/api.ts`):

```ts
export const API_URL = "http://192.168.0.100:8080/api"; 
```

> ⚠️ Use o IP da sua máquina local (não `localhost`) quando rodar em celular físico.  

---

## 🧪 Testando o App

1. Cadastre um usuário ou admin via API.  
2. Faça login pelo app usando o e-mail e senha cadastrados.  
3. Explore as funcionalidades: envio de feedback, listagem, relatórios.  

---

## 📘 Estrutura de Pastas (exemplo)

```
src/
  ├── api/            # Configuração de chamadas HTTP
  ├── components/     # Componentes reutilizáveis
  ├── navigation/     # Rotas e navegação
  ├── screens/        # Telas principais (Login, Dashboard, Feedback, etc.)
  ├── storage/        # Utilitários de AsyncStorage
  └── utils/          # Funções auxiliares
```

---

## 🧩 Futuras Melhorias

- 🔔 Push notifications para novos feedbacks.  
- 🎨 Tema escuro/claro.  
- 📊 Dashboard mais detalhado com gráficos.  

---
