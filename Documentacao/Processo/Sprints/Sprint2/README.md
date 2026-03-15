# AtlasTech - Projeto IPEM
# Documentação - Sprint 2

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
Digitalizar o processo de campo através do formulário de abastecimento. Nesta etapa, o foco é garantir a integridade dos dados através da validação automática de quilometragem e fornecer a primeira visão analítica para os gestores através do Dashboard de consumo médio.

## 📋 User Stories <a id="us"></a>

| ID | Prioridade | User Story | Est. (h) | Sprint | Status |
| :--: | :---: | --- | :---: | :---: | :---: |
| **US03** | Alta | Como administrador, desejo cadastrar viaturas para manter a frota atualizada no sistema. | 13 | 2 | 📅 |
| **US04** | Alta | Como administrador, desejo cadastrar técnicos para que eles possam acessar o sistema e realizar apontamentos. | 8 | 2 | 📅 |
| **US05** | Alta | Como administrador, desejo validar a quilometragem inserida para garantir a integridade dos dados. | 13 | 2 | 📅 |
| **US07** | Média | Como administrador, desejo visualizar um Dashboard de consumo para monitorar a eficiência da frota. | 20 | 2 | 📅 |

## 🏅 DoR - Definition of Ready <a id="dor"></a>
| Critério | Descrição |
| :---: | --- |
| Regra de Negócio | Lógica de cálculo de KM médio ($km/l$) definida. |
| Backend | API pronta para receber os campos de data, litros e valor. |
| Frontend | Componentes de gráficos escolhidos para o Dashboard. |

## 🏆 DoD - Definition of Done <a id="dod"></a>
| Critério | Descrição |
| :---: | --- |
| Validação | Sistema bloqueia registros com KM inferior ao último lançamento. |
| Dashboards | Gráficos refletindo os dados reais inseridos pelos técnicos. |

