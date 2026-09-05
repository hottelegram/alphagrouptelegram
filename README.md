# 🔥 Frontend - Página de Vendas & Checkout Pix

Aplicação Web React + Vite estática (SPA), 100% pronta para **GitHub** e **GitHub Pages**.

## 🚀 Como Rodar Localmente

1. Abra a pasta `frontend` no terminal:
   ```bash
   cd frontend
   ```
2. Instale as dependências:
   ```bash
   npm install
   ```
3. Inicie o servidor de desenvolvimento:
   ```bash
   npm run dev
   ```
4. Acesse no navegador: `http://localhost:5173`

> [!TIP]
> Certifique-se de que o `backend` esteja rodando na porta `3001` (ou aponte o `VITE_API_URL` no `.env` para sua URL da Netlify) para que a geração de Pix funcione.

---

## 🌐 Como Publicar no GitHub / GitHub Pages

### Opção 1: Via GitHub Pages (Automático com build)
1. Crie um repositório no seu GitHub e suba os arquivos desta pasta `frontend`.
2. Em **Settings > Pages** do seu repositório GitHub:
   - Em **Build and deployment > Source**, você pode escolher **GitHub Actions** (usando o template padrão do Vite) ou **Deploy from a branch**.
3. Se fizer o build local antes de subir:
   ```bash
   npm run build
   ```
   A pasta `dist` gerada contém todo o site pronto para qualquer hospedagem estática!

### Conectar com o Backend da Netlify
Quando você tiver o link da Netlify do seu backend (exemplo: `https://seu-pix-backend.netlify.app`), basta editar o arquivo `.env` do frontend:
```env
VITE_API_URL=https://seu-pix-backend.netlify.app
```
E executar novamente `npm run build`.
