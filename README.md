# Você no Controle

Aplicativo web de organização financeira **em família**, com sincronização na nuvem, site institucional, curso e metas de longo prazo.

**Versão documentada:** 24

**App online:** https://jaquelinegentillazzarin-create.github.io/Financeiro/

**Site (Framer):** https://vocênocontrole.framer.website

**Repositório:** https://github.com/jaquelinegentillazzarin-create/Financeiro

---

## Objetivo

Ajudar famílias a controlar gastos, contas e cartões **juntas**, em uma conta compartilhada, com linguagem simples e foco no Brasil (Pix, boleto, carnê, crédito parcelado).

---

## Arquitetura (No-code + Low-code + Web)

| Camada | Tecnologia | Papel |
|--------|------------|--------|
| **No-code** | Framer | Site institucional / marketing |
| **Low-code** | Supabase | Autenticação, banco de dados PostgreSQL e APIs |
| **Web (código)** | HTML, CSS e JavaScript | Aplicativo completo (uma página) |
| **Hospedagem** | GitHub Pages | Publicação gratuita do app |

Essa combinação atende propostas de disciplina sobre **padrões web, no-code e low-code**: o site nasce sem código no Framer; a base de dados e o login usam plataforma low-code (Supabase); a experiência principal é personalizada em HTML/CSS/JS.

---

## Funcionalidades principais

- Login e criação de conta (Supabase Auth)
- Conta compartilhada pela família (mesmo e-mail e senha)
- Pessoas da família e filtro de gastos por pessoa
- Gastos do mês (categorias e formas de pagamento brasileiras)
- Contas futuras e recorrentes (marcar como paga / desfazer)
- Cartões e compras parceladas
- Análises e insights do mês
- Importação de boleto, Pix, PDF e foto (leitura no aparelho)
- Documentos importados com busca
- Aba **Sonhos e objetivos** com calendário (várias metas no mesmo dia)
- Curso e SAC com contato WhatsApp
- Site Framer embutido no app
- Assistente de dicas financeiras (chat)
- Backup exportar / importar JSON
- Política de Privacidade e Termos de Uso (LGPD)

---

## Como usar

1. Abra o link do app.
2. Crie uma conta ou entre com e-mail e senha (mínimo 8 caracteres).
3. Cadastre as pessoas da família em **Configurações**.
4. Lance gastos, contas e, se quiser, metas em **Sonhos e objetivos**.

---

## Supabase (low-code)

O projeto usa um backend Supabase com:

- **Auth** — e-mail e senha
- **Tabelas** — expenses, cards, purchases, bills, documents (conforme SQL do projeto)
- **Chave anônima (anon)** no front-end do app estático

Regras de acesso (RLS) garantem que cada conta só veja os próprios dados. A família compartilha **a mesma conta de login**.

---

## Estrutura do repositório

- `index.html` — aplicativo completo (versão atual)
- `README.md` — este arquivo

Não é obrigatório framework (React, Vue etc.): o app é propositalmente **single-file** para facilitar publicação no GitHub Pages e entendimento em disciplina de padrões web.

---

## Links de entrega

| Item | URL |
|------|-----|
| Aplicativo | https://jaquelinegentillazzarin-create.github.io/Financeiro/ |
| Site no-code | https://vocênocontrole.framer.website |
| Código | https://github.com/jaquelinegentillazzarin-create/Financeiro |

---

## Autora

Jaqueline Gentil Correia

Contato (curso / SAC): WhatsApp (47) 99771-3795

---

## Observação

Este README descreve o produto em texto. **Prints de tela** ficam na **parte teórica** do trabalho acadêmico, não neste arquivo.
