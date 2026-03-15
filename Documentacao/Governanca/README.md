# 🌳 Estratégia de Branches (GitHub Flow) <a id="estrategia-branches"></a>

Este projeto adota o modelo **GitHub Flow**, priorizando a simplicidade, integração contínua e entregas frequentes. A branch `main` representa sempre a versão mais estável e atual do sistema.

---

### 🛠️ Fluxo de Trabalho

- [ ] **1. Branch Principal (`main`)**
  - A branch `main` deve estar sempre estável e pronta para uso.
  - Nenhuma alteração é feita diretamente na `main`.

- [ ] **2. Branches de Desenvolvimento**
  - Novas funcionalidades ou correções devem ser desenvolvidas em **branches curtas**, criadas a partir da `main`.
  - Padrão de nomenclatura obrigatório:
    - `feat/nome-da-feature` 
    - `fix/nome-do-bug` 
    - `refactor/nome-da-refatoracao` 

- [ ] **3. Pull Requests (PRs)**
  - Toda alteração deve ser integrada à `main` por meio de um **Pull Request**.
  - O PR deve passar por revisão de código e aprovação de pelo menos um membro da equipe antes do merge.
  - A branch deve estar atualizada com a `main` antes da integração final.

---

### 📌 Padrão de Commits

Para manter o histórico organizado e rastreável, utilizamos o padrão **Conventional Commits** simplificado:

| Tipo | Descrição | Badge |
| :--- | :--- | :--- |
| `feat` | Nova funcionalidade | ![Feature](https://img.shields.io/badge/Tipo-Feature-green) |
| `fix` | Correção de bug | ![Fix](https://img.shields.io/badge/Tipo-Fix-red) |
| `docs` | Mudanças na documentação | ![Docs](https://img.shields.io/badge/Tipo-Docs-blue) |
| `refactor` | Refatoração de código | ![Refactor](https://img.shields.io/badge/Tipo-Refactor-orange) |
| `test` | Adição/alteração de testes | ![Test](https://img.shields.io/badge/Tipo-Test-yellow) |
| `chore` | Manutenção geral | ![Chore](https://img.shields.io/badge/Tipo-Chore-lightgrey) |

**Exemplo de uso:** `feat: implementa login do técnico com JWT`