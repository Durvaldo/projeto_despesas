# 💸 Gestão de Finanças Pessoais

Projeto prático para aprender a usar **React + Firebase Firestore** com operações CRUD completas. Neste projeto, vamos criar um gerenciador de receitas e despesas pessoais com saldo automático e estilização com Tailwind CSS.

---

## 🧱 Tecnologias Utilizadas

- React com Vite
- Tailwind CSS
- Firebase Firestore
- Deploy (Indico vercel)
- **StackBlitz** como ambiente de desenvolvimento

---

## 🛠️ Primeiros Passos (StackBlitz)

### 1. **Crie o Projeto no StackBlitz**
- Acesse: [https://stackblitz.com/](https://stackblitz.com/)
- Escolha **"React + Vite"**

> O Vite já vem instalado automaticamente. na versão 7, vamos voltar ela para o 6

---

### 2. **Instale o Firebase**

No terminal do StackBlitz, digite:

```bash
npm install firebase
```

---

### 3. **Volte o Vite para a versão 6**

StackBlitz cria o projeto com Vite 7+. Para evitar problemas, vamos usar a versão 6:

```bash
npm install vite@^6
```

Depois disso, verifique o `package.json` para verificar se estamos usando a versão correta:

```json
"vite": "^6.0.0"
```

---

### 4. **Instale o Tailwind CSS**

Execute:

```bash
npm install tailwindcss @tailwindcss/vite
```

Em seguida, crie o arquivo de configuração:

---

### 5. **Configure o Tailwind**

Edite o arquivo `vite.config.ts`:

```js
import { defineConfig } from 'vite'
import tailwindcss from '@tailwindcss/vite' // Essa linha

export default defineConfig({
  plugins: [
    tailwindcss(), // Essa linha
  ],
})
```

Depois, no arquivo `src/index.css`, substitua tudo por:

```css
@import "tailwindcss";
@tailwind base;
@tailwind components;
@tailwind utilities;
```

E importe esse CSS em `main.jsx`:

```js
import './index.css';
```

---

### ✅ Pronto! Agora você pode começar a codar a aplicação.

---

## 🪜 Desenvolvimento por Etapas

### 1. Criar formulário para adicionar transações:
- Tipo: Receita ou Despesa (Recomendo um select)
- Descrição
- Valor
- Categoria (Recomendo um select, coloque "Outro" para outras categorias)
- Data e Hora

### 2. Salvar transações no Firestore

### 3. Listar todas as transações

### 4. Calcular e exibir:
- Total de Receitas
- Total de Despesas
- Saldo Atual

### 5. Adicionar funcionalidades de:
- Edição de transações
- Exclusão de transações

### 6. Estilizar com Tailwind (verde para receitas, vermelho para despesas)

### 7. (Extra) Adicionar filtros:
- Por mês, por categoria, ou tipo

---

## 📌 Conceitos Aprendidos

- React com Vite no StackBlitz
- CRUD com Firebase Firestore
- Hooks do React (`useState`, `useEffect`) -> Lembrando do uso de useEffect para evitar loop infinito.
- Estilização com Tailwind CSS
- Organização de componentes

---

## 🚀 Deploy (Obrigatorio)

O projeto pode ser hospedado no [Vercel](https://vercel.com/) conectando seu GitHub e adicionando as variáveis do Firebase.

---

## 📝 Observações

Enviar email com nome dos integrantes do grupo e link para o projeto para o email: `durvaldo.marques@prozeducacao.com.br`
