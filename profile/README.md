# 🪷 Buddha Spa — Tecnologia & Governança de IA

> *Harmonizando bem-estar, inteligência artificial e excelência em engenharia de software.*

---

## 📌 Sobre a Organização

Bem-vindo ao ecossistema tecnológico do **Buddha Spa**. Este repositório central reúne os projetos de engenharia, integrações de sistemas (TOTVS, SULTS, Feedz) e agentes de Inteligência Artificial que sustentam nossa rede de franquias e operações corporativas.

Nosso objetivo é desenvolver soluções escaláveis, seguras e focadas em eliminar gargalos operacionais com o apoio da tecnologia.

---

## 🚀 Nossa Stack Tecnológica

| Camada | Tecnologias & Ferramentas |
| :--- | :--- |
| **Linguagens & Runtimes** | TypeScript, Node.js, Python |
| **Frontend & Web** | Next.js (App Router), React, Tailwind CSS |
| **Backend & Dados** | Node.js (Async/Await), PostgreSQL, Prisma / Drizzle ORM, SQLite |
| **IA & Orquestração** | Anthropic Claude API, OpenAI / Azure OpenAI, Groq SDK, Auramind, Hermes Agent |
| **Infraestrutura & DevOps** | Docker, Vercel, GitHub Actions (CI/CD) |
| **Segurança & SAST** | Snyk, Gatekeepers de segurança OWASP, CODEOWNERS |

---

## 🛡️ Diretrizes de Desenvolvimento e Segurança

Para manter a integridade, o versionamento correto e a segurança do código em produção, todos os colaboradores e desenvolvedores externos devem seguir este fluxo:

### 1. Padrão de Branching e Commits
* **Branches:** `feat/nome-da-funcionalidade`, `fix/correcao-bug`, `chore/manutencao`
* **Commits:** Seguir o padrão [Conventional Commits](https://www.conventionalcommits.org/) (`feat: ...`, `fix: ...`, `docs: ...`)

### 2. Fluxo de Pull Request (PR) & Deploy
1. **Nunca faça commits diretos na `main`.** Sempre crie um PR a partir da sua branch de funcionalidade.
2. Todo PR dispara automaticamente o pipeline `ci-security-gate.yml` para análise SAST/SCA.
3. PRs com vulnerabilidades de segurança críticas ou graves serão **bloqueados automaticamente**.
4. É obrigatória a aprovação de pelo menos um revisor definido no arquivo `CODEOWNERS` antes do merge e deploy na Vercel.

### 3. Governança e Variáveis de Ambiente
* **Zero Hardcoding:** Nenhuma credencial, token de API, chave privada ou string de conexão deve ser inserida no código.
* **Uso do `.env`:** Utilize variáveis de ambiente gerenciadas via GitHub Secrets / Vercel Environment Variables.
* **LGPD & Dados Sensíveis:** É estritamente proibido trafegar ou armazenar dados pessoais não anonimizados (PII) de clientes ou franqueados em logs ou ambientes não homologados.

---

## 🤖 Governança de Inteligência Artificial

A utilização de IA no Buddha Spa segue nossas políticas internas centralizadas:

* **Plataforma Corporativa (Auramind):** Canal padrão para automações, consultas operacionais e suporte diário às áreas de negócio.
* **Uso Avançado (Claude Team / APIs):** Restrito às equipes de engenharia, arquitetura e análise técnica sob supervisão.
* **Guardrails Ativos:** Todas as integrações com LLMs possuem filtros de moderação, proteção contra *prompt injection* e limitação de contexto sensível.

---

## 🤝 Suporte e Contato

* **Arquitetura & Governança de IA:** [adm-engenharia@buddhaspa.com.br](mailto:adm-engenharia@buddhaspa.com.br)
* **Documentação Interna:** Consulte nossos manuais no SharePoint / Teams corporativo.

---
<p center>
  <sub>Buddha Spa &copy; 2026. Todos os direitos reservados.</sub>
</p>