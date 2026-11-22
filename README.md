# SIGE.games — Frontend

Interface web do painel analítico de vendas globais de videogames (**SIGE.games**), integrada à API do [sige-backend](https://github.com/matheusmatta21/sige-backend).

## Stack

- React 19 + TypeScript + Vite
- TanStack Router (`@tanstack/react-router`)
- Tailwind CSS v4 + Radix UI
- Recharts, `d3-geo`, `topojson-client`, `world-atlas`, `lucide-react`

## Como rodar localmente

1. Certifique-se de que o backend (`sige-backend`) esteja rodando em `http://localhost:3000`.
2. Instale as dependências e inicie o servidor de desenvolvimento:

```bash
npm install
npm run dev
```

3. Acesse `http://localhost:5173`.

> Em desenvolvimento, o [vite.config.ts](./vite.config.ts) redireciona automaticamente `/api/*` para `http://localhost:3000/*`. Para apontar para outra URL da API, copie `.env.example` para `.env` e defina `VITE_API_URL`.

## Scripts

- `npm run dev` — inicia o servidor Vite (`http://localhost:5173`)
- `npm run build` — checa TypeScript e gera o bundle de produção em `dist/`
- `npm run preview` — serve o build de produção localmente
