# 🚀 Master Prompt: Desenvolvimento da Aplicação VelozLink (MVP)

Como um **Desenvolvedor Senior Full Stack**, utilize as diretrizes abaixo para gerar a estrutura inicial, arquitetura e código para a aplicação **VelozLink**.

---

## 🎯 Contexto do Projeto
A **VelozLink** é uma plataforma de transporte cooperativo (carona) exclusiva para professores. 
- **Core:** Cruzamento de itinerários acadêmicos.
- **Tech Stack:** Next.js 14 (Frontend), Node.js (Backend), Solana (Web3/Financeiro).
- **Infra:** Integração com APIs de Mapas (Google Maps ou Mapbox).

---

## 🛠️ Requisitos de Engenharia (Prompt para o Copilot)

### 1. Estrutura do Projeto e Frontend (Next.js)
"Crie um boilerplate para uma aplicação Next.js utilizando TypeScript, Tailwind CSS e Lucid React para ícones. A interface deve seguir uma estética 'Dark Mode Web3' com tons de verde (#14f195) e roxo (#9945FF). Implemente as seguintes páginas:
- **/dashboard:** Painel principal para o professor visualizar caronas disponíveis e seu saldo em SOL/USDC.
- **/itinerario:** Formulário complexo para cadastro de horários de aula (janelas) e localização das escolas (usando Autocomplete de mapas).
- **/perfil:** Seção de verificação de documentos e integração com carteira Solana (Phantom/Solflare)."

### 2. Lógica de Cruzamento de Demanda (Algoritmo)
"Desenvolva uma função em TypeScript que receba um array de 'DemandaProfessor' (contendo lat/lng de origem, lat/lng de destino e horário de entrada) e um array de 'RotasMotorista'. A função deve retornar os 'Matches' baseados em uma tolerância de 5km de desvio e 15 minutos de antecedência. Utilize a fórmula de Haversine para cálculos de distância."

### 3. Integração Solana (Web3)
"Escreva um módulo usando `@solana/web3.js` e `@solana/wallet-adapter-react` para:
- Conectar a carteira do usuário.
- Criar uma transação de 'Escrow' onde o valor da carona em USDC é bloqueado em um programa (Smart Contract) na Devnet.
- Implementar a função de 'Release' que libera o pagamento ao motorista mediante a validação de um webhook de geolocalização."

### 4. Segurança e Validação
"Crie um middleware de autenticação que verifique se o usuário possui o metadado de 'Professor Verificado' no banco de dados (PostgreSQL/Prisma) antes de permitir o acesso às rotas de carona."

---

## 🏁 Instruções de Execução para o Copilot
1.  **Modularização:** Separe componentes UI de lógica de negócio (Hooks customizados).
2.  **State Management:** Utilize `Zustand` ou `Context API` para gerenciar o estado da viagem em tempo real.
3.  **Responsive Design:** O layout deve ser Mobile-First, focado no uso do professor durante o deslocamento.

---
*Gerado por Senior Dev Persona para VelozLink Implementation.*
