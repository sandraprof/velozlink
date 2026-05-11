# 🚀 VelozLink - Documento Consolidado & Guia de Execução (Dia 4)

Este documento representa a transição do planejamento estratégico para a **Construção Técnica**. Ele consolida as conclusões dos Dias 1, 2 e 3 e fornece o **Master Prompt** para execução via GitHub Copilot.

---

## 🏁 REVISÃO DOS ENTREGÁVEIS (DIAS 1, 2 E 3)

### **🟢 DIA 1: DESCOBERTA & IDEAÇÃO**
* **Conclusão:** O problema central é a **fragmentação logística** do professor itinerante. Validamos que uma malha cooperativa exclusiva reduz custos em até 30% e aumenta a segurança. A proposta de valor foca em economia para o passageiro e monetização de trajeto para o motorista cooperado.

### **🟣 DIA 2: ESTRUTURANDO A SOLUÇÃO**
* **Conclusão:** Definimos a arquitetura como um ecossistema integrando Next.js (Frontend), algoritmos de clustering para rotas e Solana (Blockchain). A jornada do usuário foi mapeada do onboarding via Gov.br até o desembarque verificado por Geofencing.

### **🔵 DIA 3: MVP & BLOCKCHAIN**
* **Conclusão:** Definimos um MVP enxuto focado em **Match + Pagamento Seguro**. A rede Solana será usada para custódia (Escrow) em USDC, garantindo taxas baixas. Priorizamos o algoritmo de Haversine para cálculos de distância e a validação de identidade on-chain.

---

## 🏗️ DIA 4: CONSTRUÇÃO (GUIA TÉCNICO)

Nesta fase, organizamos o repositório e iniciamos o desenvolvimento do núcleo da aplicação.

### **1. Arquitetura Proposta**
- **Frontend:** Next.js 14+ (App Router), Tailwind CSS, Shadcn/UI.
- **Backend/API:** Next.js Server Actions ou Node.js (Hono/Express).
- **Web3:** Solana Web3.js, Anchor Framework (Smart Contracts).
- **Geolocalização:** Google Maps Platform (Distance Matrix & Autocomplete).

### **2. Organização do Repositório**
```text
/apps/velozlink
  ├── /src
  │    ├── /components  # UI (Shadcn)
  │    ├── /hooks       # Wallet connection & Geolocation logic
  │    ├── /lib         # Utils (Haversine Formula)
  │    └── /contracts   # Anchor/Rust (Solana Programs)
```

---

## 🤖 MASTER PROMPT PARA GITHUB COPILOT (EXECUÇÃO)

Copie e cole o prompt abaixo no seu Copilot Chat para iniciar a codificação do núcleo do sistema:

> **PROMPT:** "Aja como um Desenvolvedor Sênior Full Stack e Web3. Vamos iniciar a construção do **VelozLink**, um sistema de transporte cooperativo para professores na Solana.
>
> **PASSO 1 (Frontend & State):** Crie uma estrutura Next.js 14 (App Router) com Tailwind CSS. Configure um contexto de Gerenciamento de Estado para a 'Viagem' (TripContext) que armazene: Origem (Lat/Lng), Destino (Lat/Lng), Horário de Entrada e Status do Match.
>
> **PASSO 2 (Algoritmo Core):** Implemente uma função utilitária em TypeScript utilizando a **Fórmula de Haversine**. A função deve receber as coordenadas do Professor e uma lista de rotas de Motoristas, retornando matches que estejam dentro de um raio de 5km de desvio e 15 minutos de tolerância de horário.
>
> **PASSO 3 (Web3 Integration):** Configure o `@solana/wallet-adapter-react`. Crie um componente de botão 'Reservar Carona' que, ao ser clicado, inicia uma transação simulada de Escrow enviando 5 USDC para um endereço de custódia na Devnet da Solana.
>
> **PASSO 4 (UI Mobile-First):** Gere uma página de Dashboard sombria (estética Web3) com um card de 'Próxima Viagem' e um botão de 'Check-in via GPS'. Use Lucid React para ícones."

---

## 🏁 CONCLUSÃO: ENTREGÁVEL DIA 4
O entregável deste dia é o **MVP em desenvolvimento** com uma base técnica sólida. Ao final deste guia, você terá:
1.  Repositório estruturado.
2.  Algoritmo de match funcional.
3.  Conexão de carteira Solana operacional.
4.  Interface inicial de agendamento de rotas.

---
*Documento orientado para a execução do Dia 4 - VelozLink Ecosystem.*
