# AtlasTech - Projeto IPEM
# Documentação - Sprint 2

<p align="center">
      <h2 align="center"> AtlasTech </h2>
</p>

<p align="center">
  | <a href ="#desafio"> Desafio</a>  |
  <a href ="#us"> User Stories</a>  |   
  <a href ="#dor">DoR</a>  |
</p>

> Status da Sprint: Planejada 📅

---

## 🏅 Desafio <a id="desafio"></a>
Expandir o ecossistema do sistema garantindo a gestão da frota e dos usuários. O foco é permitir o controle administrativo completo (Viaturas e Técnicos), implementar as travas de segurança de quilometragem para evitar erros humanos e fornecer a primeira visão analítica de consumo médio para os gestores.

---

## 📋 User Stories & DoD <a id="us"></a>

Nesta seção, detalhamos as histórias de usuário e seus respectivos **DoD (Definition of Done)** específicos.

### **US03 - Gestão de Viaturas**
> **Como administrador, desejo cadastrar viaturas para manter a frota atualizada no sistema.**

* **Prioridade:** Alta | **Estimativa:** 13h | **Status:** 📅
* **DoD (Critérios de Sucesso):**
    * Interface funcional para Cadastro/Edição/Listagem (CRUD) de veículos.
    * Campos obrigatórios conforme Boletim de Tráfego: Marca, Modelo, Ano, Placa, Prefixo e Tipo de Combustível.
    * Persistência dos dados no **Supabase** garantindo que o Prefixo seja único.

### **US04 - Gestão de Técnicos**
> **Como administrador, desejo cadastrar técnicos para que eles possam acessar o sistema e realizar apontamentos.**

* **Prioridade:** Alta | **Estimativa:** 8h | **Status:** 📅
* **DoD (Critérios de Sucesso):**
    * Interface para cadastro de funcionários com Nome e Número da Carteira Funcional (conforme Boletim).
    * Vinculação do usuário ao perfil de "Técnico" para acesso restrito à tela de apontamento.
    * Lista de técnicos ativos disponível para seleção no formulário de jornada.

### **US05 - Validação de Integridade (KM)**
> **Como administrador, desejo validar a quilometragem inserida para garantir a integridade dos dados.**

* **Prioridade:** Alta | **Estimativa:** 13h | **Status:** 📅
* **DoD (Critérios de Sucesso):**
    * Regra de Backend: Bloqueio de inserção se o KM de Saída for menor que o último KM de Chegada registrado para aquela viatura.
    * Regra de Frontend: Exibição de alerta impeditivo caso o usuário tente finalizar com KM incoerente.
    * Log de erros para tentativas de inserção inválidas.

### **US06 - Dashboard de Consumo Médio**
> **Como administrador, desejo visualizar um Dashboard de consumo para monitorar a eficiência da frota.**

* **Prioridade:** Média | **Estimativa:** 20h | **Status:** 📅
* **DoD (Critérios de Sucesso):**
    * Gráficos em tempo real utilizando os dados de Abastecimento (Litros) e KM Rodados.
    * Cálculo automático da média de consumo ($km/l$) por veículo e por período.
    * Filtros por Prefixo da Viatura e intervalo de datas (mês corrente).

---

## 🏃‍ DoR - Definition of Ready (Sprint 2) <a id="dor"></a>
Critérios necessários para iniciar o desenvolvimento:

* **Regra de Negócio**: Lógica de cálculo de rendimento ($km/l$) validada com o cliente.
* **Backend**: Estrutura de tabelas para `usuarios` e `veiculos` espelhada no Supabase.
* **Frontend**: Biblioteca de gráficos (Chart.js ou similar) definida e integrada ao projeto Vue.js.
* **Design**: Protótipo das telas de CRUD e Dashboard aprovado no Figma.

---

## 🏆 Critérios de Conclusão da Sprint
Para o fechamento da Sprint 2, a equipe deve garantir:
* Pull Requests aprovados por membros da TechForce seguindo o **GitHub Flow**.
* Código funcional integrado à branch `main`.
* Documentação do README da Sprint atualizada com evidências dos novos cadastros e do Dashboard.
