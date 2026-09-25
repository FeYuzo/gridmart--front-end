# GridMart - Frontend

Interface web do mini mercado autônomo GridMart, desenvolvida com **React**, **TypeScript** e **Vite**.

## 📌 Funcionalidades

- **Totem de Autoatendimento:** Busca e adição de produtos por código de barras ou seleção rápida, resumo de carrinho e pagamento com QR Code Pix em tempo real.
- **Controle de Acesso:** Validação de CPF para entrada de clientes no mercado e liberação de saída.
- **Gestão de Produtos:** Cadastro, edição, exclusão e listagem de produtos do catálogo.

## 🚀 Como Executar

### 1. Pré-requisitos
- [Node.js](https://nodejs.org/) (versão 18+ recomendada)

### 2. Instalação das dependências
Caso esteja configurando em uma máquina nova:
```bash
npm install
```

### 3. Configuração da API (Backend)
Por padrão, o Vite já possui um proxy configurado em `vite.config.ts` apontando as rotas `/products`, `/access` e `/sales` para a API local em `http://127.0.0.1:8787`.

Se desejar definir uma URL explícita (por exemplo em produção ou outro endereço), crie um arquivo `.env`:
```env
VITE_API_URL=http://localhost:8787
```

### 4. Rodar em modo de desenvolvimento
```bash
npm run dev
```
O frontend estará acessível em: [http://localhost:3000](http://localhost:3000)

### 5. Build de Produção
Para gerar os arquivos estáticos otimizados para deploy:
```bash
npm run build
```
Os arquivos gerados ficarão na pasta `dist/`.

## 🛠️ Scripts Disponíveis

- `npm run dev`: Inicia o servidor Vite de desenvolvimento.
- `npm run build`: Valida tipagem com TypeScript e gera o build de produção.
- `npm run preview`: Visualiza o build de produção localmente.
