# Primeiro_Desafio_Copilot
Criando seu primeiro Copiloto no Microsoft Copilot Studio - Clínica Médica
# 🚀 Criando seu Primeiro Copilot no Microsoft Copilot Studio

Este repositório faz parte de uma atividade da **DIO (Digital Innovation One)** sobre **Microsoft Copilot Studio**.  
O objetivo é aprender a criar copilotos de forma didática e prática, passando por três tipos de criação e finalizando com um exemplo aplicado em uma **clínica médica**.

---

## 📘 Conteúdo do Repositório

- `guia_copilot.py` → Arquivo em Python (com comentários) que explica:
  1. Como criar um Copilot baseado em **modelo**  
  2. Como criar um Copilot baseado em **descrição de IA**  
  3. Como criar um Copilot **em branco**  
  4. Exemplo prático: **Copilot para clínica médica**  
  5. Fluxo em **árvore de decisão** para o exemplo  

---

## 🛠️ Como Criar um Copilot no Copilot Studio

### 1️⃣ Copilot baseado em modelo
- Acesse o [portal Copilot Studio](https://copilotstudio.microsoft.com/).
- Clique em **Criar Copilot** → **Baseado em modelo**.
- Escolha um dos modelos prontos (FAQ, Atendimento ao Cliente, etc).
- Personalize fluxos de conversa.
- Publique e teste seu copiloto.

✅ **Vantagem:** rápido e prático para iniciantes.

---

### 2️⃣ Copilot baseado em descrição de IA
- No portal, clique em **Criar Copilot** → **Baseado em descrição de IA**.
- Escreva o que deseja em **linguagem natural**  
  Exemplo:  
  > "Quero um copiloto que ajude clientes a consultar saldo bancário."
- O Copilot gera um modelo inicial automaticamente.
- Ajuste fluxos e conecte a serviços externos.
- Publique e teste.

✅ **Vantagem:** criação intuitiva apenas descrevendo a ideia.

---

### 3️⃣ Copilot em branco
- Clique em **Criar Copilot** → **Em branco**.
- Dê um nome, escolha o idioma.
- Construa fluxos de conversa do zero:
  - Mensagens de boas-vindas.
  - Tópicos personalizados.
  - Integrações com APIs externas.
- Publique e valide.

✅ **Vantagem:** total flexibilidade e personalização.

---

## 🏥 Exemplo Prático - Clínica Médica

### Objetivo:
Copilot que realiza **atendimento inicial de pacientes**:
- Agendamento básico.
- Informações sobre especialidades médicas.
- Localização e horários.
- Opção de falar com atendente humano.

### Fluxo resumido:
1. **Mensagem de boas-vindas**:  
   "Olá, seja bem-vindo à Clínica Saúde Integral! 👩‍⚕️👨‍⚕️"
2. **Menu principal**:  
   - Agendar consulta  
   - Especialidades médicas  
   - Localização e horários  
   - Falar com atendente humano  
3. **Agendamento**: coleta nome, CPF, especialidade, data/hora → confirma consulta.  
4. **Especialidades**: lista as áreas atendidas (clínica geral, pediatria, cardiologia etc).  
5. **Localização e horários**: exibe endereço e período de atendimento.  
6. **Atendente humano**: direciona ou registra contato para retorno.  

---

## 🌳 Árvore de Decisão (Clínica Médica)

```text
INÍCIO
 |
 |--> Mensagem de boas-vindas
       "Posso ajudar com:
        1. Agendar consulta
        2. Especialidades médicas
        3. Localização e horários
        4. Falar com atendente"
 |
 +---> [1] Agendar consulta
 |       |--> Nome completo
 |       |--> CPF/documento
 |       |--> Especialidade
 |       |--> Data/horário
 |       |--> Confirma agendamento ✅
 |
 +---> [2] Especialidades médicas
 |       |--> Lista áreas atendidas
 |       |--> "Deseja agendar?"
 |
 +---> [3] Localização e horários
 |       |--> Exibe endereço e funcionamento
 |
 +---> [4] Falar com atendente
         |--> Transfere ou registra contato
