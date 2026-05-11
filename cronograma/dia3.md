
# 🚀 VelozLink - Documento Consolidado de Desenvolvimento

Este documento reúne a evolução estratégica e técnica do ecossistema **VelozLink**, seguindo a metodologia de 3 dias: Descoberta, Estruturação e Definição de MVP/Blockchain.

---

## 🟢 DIA 1: DESCOBERTA & IDEAÇÃO
*Foco: Entendimento do problema e validação da proposta de valor.*

### **🔍 Processo de Descoberta**
* **Problema Real:** Professores itinerantes sofrem com logística fragmentada entre múltiplas escolas, resultando em altos custos e cansaço físico.
* **Dores Identificadas:** Insegurança em apps genéricos, janelas de aula não atendidas por transporte público e taxas bancárias abusivas.

### **🏁 Entregável Dia 1**
* **Problema Definido:** A falta de coordenação entre rotas convergentes de docentes compromete até 30% da renda líquida da categoria.
* **Ideia Validada:** Malha cooperativa Web3 para rateio de custos de deslocamento.
* **Proposta de Valor:** Economia real para o professor, monetização de trajeto para o motorista cooperado e inclusão em DeFi para o ecossistema.

---

## 🟣 DIA 2: ESTRUTURANDO A SOLUÇÃO
*Foco: Mapeamento de fluxos, jornada do usuário e blueprint técnico.*

### **⚙️ Funcionamento do Sistema**
O VelozLink utiliza um algoritmo de **Clustering** para agrupar professores que saem e entram em instituições de ensino em janelas de horários similares.

### **🏁 Entregável Dia 2**
* **Fluxo do Usuário:** Jornada completa desde o Onboarding (validação via Gov.br + Wallet Solana) até a finalização da viagem via Geofencing.
* **Desenho da Solução:** Arquitetura integrando Frontend Mobile (Next.js), Backend de Inteligência de Rotas e Layer Blockchain (Solana).
* **Diferencial Técnico:** O uso de geolocalização preditiva garante que o professor chegue antes do sinal da primeira aula.

---

## 🔵 DIA 3: MVP & BLOCKCHAIN
*Foco: Definição de tecnologias Web3 e escopo enxuto para lançamento.*

### **⛓️ Estratégia Web3**
* **Solana:** Escolhida pela alta performance e taxas de transação desprezíveis (~$0,00025).
* **Escrow:** O valor da carona fica retido em um Smart Contract (Anchor) e só é liberado após a confirmação geolocalizada do destino.

### **🏁 Entregável Dia 3**
* **MVP Enxuto:** Foco no "Match Crítico" (Raio de distância + Janela de Horário) e Liquidação Financeira via USDC (SPL Token) para evitar volatilidade.
* **Prioridades Claras:**
    1. Deploy do contrato de Escrow na Devnet.
    2. Algoritmo de Haversine para cálculo de distância.
    3. Validação de identidade docente on-chain (Soulbound Tokens).

---

## 🚀 Conclusão Geral do Entregável
O **VelozLink** está agora documentado desde a sua concepção filosófica (ajuda mútua entre professores) até a sua execução técnica (infraestrutura em Solana). O projeto está pronto para a fase de desenvolvimento do protótipo funcional.

*Documento consolidado conforme especificações metodológicas dos Dias 1, 2 e 3.*
