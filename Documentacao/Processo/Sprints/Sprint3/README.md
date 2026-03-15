# AtlasTech - Projeto IPEM
# Documentação - Sprint 3

<p align="center">
      <h2 align="center"> AtlasTech </h2>
</p>

<p align="center">
  | <a href ="#desafio"> Desafio</a>  |
  <a href ="#us"> User Stories</a>  |   
  <a href ="#dor">DoR</a>  |
  <a href ="#dod">DoD</a>  |
</p>

> Status da Sprint: Planejada 📅

## 🏅 Desafio <a id="desafio"></a>
Finalizar o ecossistema do projeto com a implementação de segurança (Autenticação e Autorização), permitindo que técnicos e administradores tenham acessos restritos. Também serão entregues os filtros por tipo de veículo e os alertas de manutenção preventiva sugeridos pelo cliente.

## 📋 User Stories <a id="us"></a>

| ID | Prioridade | User Story | Est. (h) | Sprint | Status |
| :--: | :---: | --- | :---: | :---: | :---: |
| **US08** | Média | Como administrador, desejo visualizar o histórico de abastecimentos para conferência de dados. | 8 | 3 | 📅 |
| **US09** | Alta | Como usuário (Admin/Técnico), gostaria de ter acesso por login para garantir a segurança das informações. | 13 | 3 | 📅 |
| **US10** | Média | Como técnico, desejo visualizar e editar os registros de abastecimentos realizados por mim. | 13 | 3 | 📅 |
| **US11** | Baixa | Como administrador, desejo filtrar os gastos por tipo de veículo (Utilitário vs Passeio) para análise de custos. | 13 | 3 | 📅 |
| **US12** | Baixa | Como administrador, desejo receber notificações referente a manutenções preventivas de viaturas. | 13 | 3 | 📅 |

## 🏅 DoR - Definition of Ready <a id="dor"></a>
| Critério | Descrição |
| :---: | --- |
| Segurança | Definição de perfis de acesso (Role-Based Access Control). |
| Backend | Configuração do Spring Security e JWT. |

## 🏆 DoD - Definition of Done <a id="dod"></a>
| Critério | Descrição |
| :---: | --- |
| Segurança | Usuários técnicos não acessam telas de cadastro de viaturas ou dashboard global. |
| Alertas | Sistema exibe notificação visual quando a viatura atinge o KM de revisão. | 

