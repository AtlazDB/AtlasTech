# AtlasTech - Projeto IPEM
# Documentação - Sprint 3

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
Finalizar o ecossistema do projeto com foco em segurança e governança de dados. O desafio desta etapa é implementar o controle de acesso (Autenticação e Autorização), permitir a rastreabilidade através do histórico de lançamentos e automatizar os alertas de manutenção preventiva (como a troca de óleo prevista no boletim físico), transformando dados brutos em inteligência operacional.

---

## 📋 User Stories & DoD <a id="us"></a>

Nesta seção, detalhamos as histórias de usuário e seus respectivos **DoD (Definition of Done)** específicos.

### **US07 - Histórico Administrativo**
> **Como administrador, desejo visualizar o histórico de abastecimentos para conferência de dados.**

* **Prioridade:** Média | **Estimativa:** 8h | **Status:** 📅
* **DoD (Critérios de Sucesso):**
    * Tela de listagem global com todos os apontamentos realizados.
    * Funcionalidade de ordenação por data e filtros por técnico ou viatura.
    * Visualização detalhada de cada registro (Km, litros, valor e nota fiscal).

### **US08 - Autogestão do Técnico**
> **Como técnico, desejo visualizar e editar os registros realizados por mim para correção de eventuais erros.**

* **Prioridade:** Média | **Estimativa:** 13h | **Status:** 📅
* **DoD (Critérios de Sucesso):**
    * Interface de "Meus Lançamentos" restrita aos dados inseridos pelo usuário logado.
    * Permissão de edição liberada apenas enquanto o registro não for exportado para o SGI.
    * Garantia de que um técnico não consiga visualizar ou alterar dados de outros colegas.

### **US09 - Análise por Categoria de Frota**
> **Como administrador, desejo filtrar os gastos por tipo de veículo (Utilitário vs Passeio) para análise de custos.**

* **Prioridade:** Baixa | **Estimativa:** 13h | **Status:** 📅
* **DoD (Critérios de Sucesso):**
    * Inclusão do campo "Tipo de Veículo" no cadastro de viaturas.
    * Filtro dinâmico no Dashboard que segrega custos e consumo médio por categoria.
    * Relatório de exportação refletindo a categoria do veículo para o SGI.

### **US10 - Alertas de Manutenção Preventiva**
> **Como administrador, desejo receber notificações referente a manutenções preventivas de viaturas.**

* **Prioridade:** Baixa | **Estimativa:** 13h | **Status:** 📅
* **DoD (Critérios de Sucesso):**
    * Implementação dos campos de "Última Troca de Óleo" e "Próxima Troca (Km)" conforme Boletim de Tráfego.
    * Sistema de alerta visual (ícone ou cor diferenciada) quando a quilometragem atual estiver a menos de 500km da revisão prevista.
    * Notificação automática na tela principal do administrador ao identificar veículos com manutenção vencida.

---

## 🏃‍ DoR - Definition of Ready (Sprint 3) <a id="dor"></a>
Critérios necessários para iniciar o desenvolvimento:

* **Segurança**: Definição clara dos perfis de acesso (Admin vs Técnico).
* **Backend**: Configuração do ambiente para Spring Security e geração de Tokens JWT.
* **Regra de Manutenção**: Definição dos intervalos de quilometragem para cada tipo de serviço (Óleo, Pneus, etc.).
* **Design**: Protótipo das telas de histórico e componentes de notificação validados.

---

## 🏆 Critérios de Conclusão da Sprint
Para o fechamento da Sprint 3, a equipe deve garantir:
* Segurança: Técnicos impedidos de acessar rotas administrativas via URL ou interface.
* Integração: Todos os filtros de histórico e Dashboard funcionando com dados reais do Supabase.
* Pull Requests aprovados e código consolidado na branch `main`.
* README da Sprint atualizado com as evidências de segurança e alertas funcionais.
