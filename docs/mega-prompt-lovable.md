# ✝️ Mega Prompt: Santo Hábito — Plataforma de Devocional Diário

Crie uma aplicação web responsiva, moderna e acolhedora chamada "Santo Hábito", voltada para ajudar fiéis católicos a manterem uma rotina diária de oração e liturgia.

---

## 🎨 Design e Identidade Visual
- **Paleta de Cores:** Estilo sacro e moderno.
  - Principal: Azul Marinho (`#1A2B4C`)
  - Destaque/Acentos: Dourado (`#D4AF37`)
  - Fundo: Off-White / Sálvia Suave (`#F8F9FA`)
  - Detalhes Secundários: Vinho (`#6B1D2F`)
- **Tipografia:** Elegante, limpa e de fácil leitura.
- **Vibe Geral:** Acolhedora, espiritual, organizada e minimalista.

---

## 📄 Estrutura da Página Principal (Landing Page)

### 1. Hero Section
- **Título:** "Construa uma rotina de oração com o Santo Hábito"
- **Subtítulo:** "Receba diariamente no seu WhatsApp e E-mail o plano espiritual ideal para a sua jornada."
- **Botão Principal (CTA):** "Montar Meu Plano Espiritual" (deve rolar suavemente até o formulário).

### 2. Sessão de Benefícios / Como Funciona (3 Cards)
1. **Escolha seu objetivo:** Selecione o itinerário litúrgico ou de oração que mais se adapta ao seu momento espiritual.
2. **Defina os horários:** Escolha os melhores horários para receber seus lembretes e meditações.
3. **Receba no WhatsApp:** Mantenha a constância diária direto no seu celular.

### 3. Formulário de Personalização do Plano
- **Campos Obrigatórios:**
  - Nome Completo (`text`)
  - E-mail (`email`)
  - WhatsApp com DDI/DDD (`tel` com máscara)
  - **Plano de Oração Desejado (`select`/`radio`):**
    - Liturgia Diária + Meditação
    - Santo do Dia + História
    - Preparação para Consagração
    - Santo Terço e Intenções
  - **Horário de Preferência (`select`):**
    - Manhã (06:00)
    - Meio-dia (12:00)
    - Noite (18:00)
- **Botão de Envio:** "Finalizar Inscrição e Abrir WhatsApp"
- **Comportamento ao Submeter:**
  - Salva os dados do lead no banco de dados interno (Lovable Cloud).
  - Redireciona o usuário para o WhatsApp com uma mensagem pré-formatada contendo os dados do cadastro.

---

## 🛠️ Painel de Administração (`/admin`)

Criar uma área administrativa protegida e minimalista para gestão dos inscritos:

- **Cards de Métricas (Topo):**
  - Total de Fiéis Inscritos
  - Plano Mais Popular
  - Novas Inscrições Hoje
- **Tabela de Leads/Fiéis:**
  - Colunas: Nome, E-mail, WhatsApp, Plano Escolhido, Horário Preferido, Status, Data do Cadastro.
  - Filtros: Por Plano de Oração e por Horário.
  - Status do Usuário: Selecionável entre "Pendente", "Ativo" e "Inativo".
  - Ação Rápida: Botão "Enviar WhatsApp" ao lado de cada registro que abre a conversa direta com o número do usuário.

---

## 🚀 Requisitos Técnicos e Integração
- **Banco de Dados:** Utilizar a estrutura nativa do Lovable Cloud.
- **Responsividade:** Design *Mobile First* adaptável para celulares, tablets e computadores.
- **Validação:** Validação de formato de e-mail e telefone no formulário antes do envio.
