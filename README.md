# ✝️ Santo Hábito — Plataforma de Devocional e Itinerário Espiritual Diário

> **Projeto desenvolvido para o Desafio MeuNegócio.AI (DIO)**  
> *Construindo um Produto Digital com Agentes de IA e Lovable*

---

## 📌 1. A Dor Escolhida e a Oportunidade de Negócio

Muitos fiéis católicos desejam manter uma rotina consistente de oração, leitura da liturgia diária ou estudo sobre a vida dos santos. No entanto, devido à rotina corrida e à falta de um método estruturado, a maioria enfrenta dificuldades de constância e disciplina espiritual.

O **Santo Hábito** surge para resolver essa dor, oferecendo um plano espiritual diário personalizado entregue diretamente no WhatsApp e E-mail do usuário.

---

## 📊 2. Tamanho de Mercado (TAM, SAM, SOM)

- **TAM (Total Addressable Market):** ~120 milhões de católicos no Brasil (Censo IBGE / Pesquisas de religiosidade).
- **SAM (Serviceable Addressable Market):** ~30 milhões de católicos praticantes que utilizam smartphones e redes sociais diariamente.
- **SOM (Serviceable Obtainable Market):** ~50.000 usuários iniciais alcançados através de parcerias com grupos de jovens, paróquias e influenciadores católicos nos primeiros 12 meses.

---

## 🎨 3. Business Model Canvas (BMC)

| Bloco | Detalhes |
| :--- | :--- |
| **Parceiros-Chave** | Paróquias, movimentos jovens (EJC/Crisma), grupos de oração e criadores de conteúdo católico. |
| **Atividades-Chave** | Curadoria de conteúdo litúrgico, gestão da comunidade e envio automatizado de mensagens. |
| **Proposta de Valor** | Acompanhamento espiritual personalizado, prático e diário direto no WhatsApp. |
| **Relacionamento** | Acolhedor, comunitário e automatizado via mensagens de WhatsApp e alertas por e-mail. |
| **Segmento de Clientes**| Católicos praticantes, jovens e adultos buscando criar um hábito diário de oração. |
| **Recursos-Chave** | Plataforma Lovable, integração com Resend (E-mail) e listas do WhatsApp. |
| **Canais** | Landing Page, redes sociais, grupos de WhatsApp e divulgação paroquial. |
| **Estrutura de Custos**| Custos mínimos no MVP (Lovable Cloud / Resend no plano gratuito). |
| **Fontes de Receita** | Gratuito na fase MVP (foco em engajamento); futuro modelo de doações voluntárias ou plano Premium. |

---

## 🧪 4. A Tese do MVP e o que ficou Manual de Propósito

### **A Tese do MVP:**
Testar se os fiéis estão dispostos a preencher um formulário de personalização e iniciar o contato no WhatsApp para receber um itinerário diário de oração.

### **O que ficou manual de propósito:**
1. **Envio dos conteúdos:** As mensagens diárias são enviadas manualmente pelo organizador via lista de transmissão do WhatsApp.
2. **Confirmação de cadastro:** O link do WhatsApp gera uma mensagem pré-formatada para a equipe cadastrar o contato manualmente.
3. **Gestão de membros:** O painel administrativo armazena as preferências, mas a inclusão nos grupos/listas é executada de forma manual.

---

## 📝 5. O Mega Prompt Utilizado no Lovable

O prompt em Markdown desenhado para a construção do MVP no Lovable encontra-se no arquivo [`docs/mega-prompt-lovable.md`](docs/mega-prompt-lovable.md) e abaixo:

```markdown
# Mega Prompt: Santo Hábito

Crie uma aplicação web responsiva chamada "Santo Hábito", voltada para ajudar fiéis católicos a manterem uma rotina diária de oração.

## Identidade Visual
- Cores: Azul Marinho (#1A2B4C), Dourado (#D4AF37), Off-White (#F8F9FA).
- Vibe: Acolhedora, espiritual, organizada e minimalista.

## Funcionalidades Principais
1. **Landing Page:** Explicativa sobre o impacto do hábito diário de oração com botão para "Montar Meu Plano Espiritual".
2. **Formulário de Personalização:**
   - Campos: Nome, E-mail, WhatsApp, Plano Desejado (Liturgia Diária, Santo do Dia, Consagração, Terço) e Horário de Preferência.
   - Ação: Salva no Lovable Cloud e redireciona para o WhatsApp com os dados preenchidos.
3. **Painel Admin (`/admin`):**
   - Tabela de leads com filtros por plano e horário.
   - Status do usuário (Pendente, Ativo, Inativo).
   - Métricas de inscritos totais e plano mais popular.
