# AtlasTech - Projeto IPEM
# Documentação - Sprint 1

<p align="center">
      <h2 align="center"> AtlasTech </h2>
</p>

<p align="center">
  | <a href ="#desafio"> Desafio</a>  |
  <a href ="#us"> User Stories</a>  |   
  <a href ="#dor">DoR</a>  |
  <a href ="#dod">DoD</a>  |
</p>

> Status da Sprint: Em Andamento ⏳

## 🏅 Desafio <a id="desafio"></a>
Estabelecer o fluxo funcional de entrada e saída de dados de abastecimento. Isso inclui a criação da interface de lançamento para o técnico e o motor de exportação de relatórios para o administrador, garantindo a integridade mínima das informações coletadas.

---

## 📋 User Stories <a id="us"></a>

| ID | Prioridade | User Story | Est. (h) | Sprint | Status |
| :--: | :---: | --- | :---: | :---: | :---: |
| **US01** | Alta | Como técnico, desejo registrar um abastecimento para digitalizar as informações da planilha física. | 13 | 1 | ⚙️ |
| **US02** | Alta | Como administrador, desejo exportar os dados mensais para facilitar o input manual no sistema SGI. | 20 | 1 | ⚙️ |

---

## 🏃‍ DoR - Definition of Ready <a id="dor"></a>
Para que uma User Story seja considerada pronta para o desenvolvimento nesta Sprint, ela deve atender aos seguintes critérios:

-  **Clareza**: User Story escrita no formato padrão com critérios de aceitação específicos para abastecimento e exportação.
- **Modelagem**: Tabela de `abastecimento` configurada.
-  **Integração Back-end**: Endpoints Java/Spring Boot mapeados para persistência dos dados de consumo.
-  **Design**: Protótipo da tela de lançamento de abastecimento (formulário) validado no **Figma**.
- **Contrato de Saída**: Layout do arquivo CSV/Excel definido de acordo com os requisitos do sistema SGI.

## 🏆 DoD - Definition of Done <a id="dod"></a>
Uma funcionalidade é considerada concluída quando atende aos seguintes requisitos de entrega:

-  **Código Revisado**: Pull Request aprovado por pelo menos um membro da equipe seguindo o *GitHub Flow*.
-  **Persistência**: Dados inseridos via front-end (**Vue.js**) salvos corretamente no banco através da API Java.
-  **Funcional (Técnico)**: Registro de abastecimento permite salvar Data, KM, Litros, Valor e Nota Fiscal.
-  **Funcional (Admin)**: Exportação gera um arquivo funcional com os registros realizados no período.
-  **Estabilidade**: O código foi integrado à branch `main` e passa nos testes básicos de execução.
-  **Documentação**: README da Sprint atualizado com as evidências da entrega.