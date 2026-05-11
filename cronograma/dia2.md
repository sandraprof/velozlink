
# 🚀 VelozLink - Estruturação da Solução

Este documento consolida as etapas de **Dia 1 (Descoberta & Ideação)** e **Dia 2 (Estruturando a Solução)** para o ecossistema VelozLink, conforme a metodologia de design de produto proposta.

---

## 🟢 DIA 1: DESCOBERTA & IDEAÇÃO (Revisão)

### **⚠️ Problema Real & Dores Identificadas**
* **Logística Fragmentada:** Professores "itinerantes" sofrem com o custo e cansaço de deslocamentos entre múltiplas unidades escolares.
* **Insegurança Financeira e Física:** Taxas abusivas em apps tradicionais e falta de confiança em caronas aleatórias.

### **💡 Ideia Validada**
Criação de um sistema de **carona cooperativa exclusiva para docentes** com liquidação financeira via **Solana**, garantindo taxas mínimas e segurança via Smart Contracts.

---

## 🟣 DIA 2: ESTRUTURANDO A SOLUÇÃO

### **⚙️ Como a Solução Funciona**
O VelozLink opera como um orquestrador de rotas. O sistema não busca apenas "um motorista para um passageiro", mas sim **otimizar veículos existentes**.
1.  **Input de Grade:** O professor insere sua grade horária semanal e locais de trabalho.
2.  **Engine de Match:** O algoritmo agrupa perfis com trajetos e janelas de horários similares (Ex: Professores que saem da Escola A às 12h e entram na Escola B às 13h).
3.  **Liquidação Web3:** O pagamento em USDC/SOL é processado via rede Solana para evitar o "spread" bancário.

### **🗺️ Jornada do Usuário (Fluxo Principal)**
1.  **Onboarding:** Validação de identidade docente e carteira Solana (Phantom/Solflare).
2.  **Agendamento:** Definição de rotas recorrentes.
3.  **Match & Confirmação:** O sistema sugere o grupo de carona; usuários confirmam.
4.  **Execução:** Acompanhamento via GPS.
5.  **Finalização:** Confirmação de chegada via Geofencing libera o Smart Contract.

### **🎨 Desenho Inicial (Wireframe Concepts)**
* **Tela de Rotas:** Mapa interativo destacando os "Clusters de Professores" no trajeto.
* **Painel Financeiro:** Extrato de economia gerada e saldo em criptoativos.

---

## 🏁 CONCLUSÃO: ENTREGÁVEL (DETALHAMENTO DIA 2)

Conforme a orientação metodológica, o entregável final desta fase consiste em:

### **1. Fluxo do Usuário Consolidado**
Um mapeamento lógico que garante zero fricção entre o cadastro da demanda e a realização da carona. O fluxo elimina a necessidade de negociação manual, tornando a cooperação automática.

### **2. Desenho Inicial da Solução (Blueprint)**
A arquitetura de sistema que integra:
* **Frontend Mobile:** Interface intuitiva para professores em trânsito.
* **Backend de Inteligência:** Algoritmo de cruzamento de itinerários (Clustering).
* **Layer Blockchain:** Contratos inteligentes de custódia (Escrow) que garantem que o motorista só recebe após o professor ser entregue no destino.

### **3. Proposta de Valor Técnica**
A solução está estruturada para escalar de forma descentralizada, onde a confiança é garantida pelo código (Blockchain) e pela identidade profissional comum (Comunidade Acadêmica).

---
*Documento gerado para o projeto VelozLink conforme especificações de Dia 2: Estruturando a Solução.*
