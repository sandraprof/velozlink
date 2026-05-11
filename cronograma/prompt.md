# 🚀 Master Prompt: Construção do Core VelozLink (Dia 4)

Aja como um **Desenvolvedor Sênior Full Stack e Web3**. O objetivo é iniciar a codificação do MVP do **VelozLink**, focando na base técnica sólida definida nas etapas anteriores.

---

## 🏗️ Contexto e Arquitetura
- **Stack:** Next.js 14 (App Router), Tailwind CSS, TypeScript.
- **Web3:** Integração com Solana (USDC/SOL) via `@solana/web3.js`.
- **Core Logic:** Algoritmo de matching geolocalizado (Haversine).

---

## 🤖 Prompt para Execução (GitHub Copilot)

> "Vamos construir a base técnica do **VelozLink**. Siga estas instruções passo a passo para garantir uma arquitetura escalável e limpa:
>
> ### 1. Setup de Estado e Contexto (Frontend)
> Crie um arquivo `src/context/TripContext.tsx` que utilize a Context API do React para gerenciar o estado global da aplicação. O estado deve incluir:
> - `userRole`: 'professor' | 'motorista' | null.
> - `currentTrip`: { origin: LatLng, destination: LatLng, entryTime: string }.
> - `matchStatus`: 'searching' | 'found' | 'confirmed' | 'idle'.
> - Implemente as funções básicas de `updateTrip` e `setRole`.
>
> ### 2. Implementação do Algoritmo de Matching (Lib)
> Crie um utilitário em `src/lib/matchEngine.ts`. Implemente a **Fórmula de Haversine** para calcular a distância entre dois pontos (lat/lng). 
> Desenvolva a função `findMatches(demand: ProfessorDemand, drivers: DriverRoute[])` que retorna apenas motoristas que atendam aos critérios:
> - **Distância:** Desvio máximo de 5km da rota original.
> - **Tempo:** Janela de chegada entre 15 e 5 minutos antes do início da aula.
>
> ### 3. Integração Solana (Wallet & Escrow)
> Configure o componente de provider do `@solana/wallet-adapter-react` no layout principal. 
> Crie um hook customizado `useVelozPayments` em `src/hooks/useVelozPayments.ts` que:
> - Verifique o saldo de USDC na carteira conectada.
> - Contenha uma função `initiateEscrow(amount: number)` que crie uma transação simulada enviando o valor para uma conta de custódia (Vault) na Devnet.
>
> ### 4. UI Dashboard (Mobile-First)
> Gere o componente `src/app/dashboard/page.tsx`. A interface deve ser focada em dispositivos móveis, com tema 'Dark Mode Web3' (Fundo escuro, detalhes em #14f195 e #9945FF). 
> - Inclua um mapa interativo simplificado (placeholder).
> - Adicione um Card de 'Status da Carona' que mude de cor conforme o `matchStatus`.
> - Use ícones da biblioteca `lucide-react`."

---

## 🏁 Checklist de Entrega (Dia 4)
- [ ] Repositório estruturado com as pastas `/components`, `/hooks`, `/lib` e `/context`.
- [ ] Algoritmo de Haversine testado e filtrando rotas corretamente.
- [ ] Wallet Adapter funcional no frontend.
- [ ] Layout Mobile responsivo e seguindo a identidade visual.

---
*Instruções geradas para a fase de Construção do ecossistema VelozLink.*
