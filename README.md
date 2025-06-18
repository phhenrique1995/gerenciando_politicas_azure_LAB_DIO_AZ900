# LAB - Gerenciando Políticas em Acessos Azure. (AZ900 | DIO)

Este guia foi elaborado com base nas aulas do curso AZ-900 da Microsoft Azure, com foco em **governança, conformidade e gerenciamento de políticas de acesso** dentro da nuvem Azure. Ele é escrito com linguagem acessível e prática, como se fosse feito por um estudante iniciante na área de DevOps.

---

## 📅 O que é Governança na Nuvem Azure?

Governança na nuvem é o conjunto de regras, processos e ferramentas que ajudam a controlar o uso e o comportamento dos recursos em ambientes de nuvem, garantindo **segurança, conformidade, eficiência e transparência**.

---

## 🔐 Políticas de Acesso e Controle

### RBAC (Controle de Acesso Baseado em Função)

- Com RBAC você define **quem pode fazer o quê** dentro do Azure.
- Exemplos de funções:
  - Leitor (Read-only)
  - Colaborador (pode criar e editar recursos)
  - Administrador de rede (pode editar configurações de rede)

### Azure Policy

- Permite **criar e aplicar regras de conformidade** para seus recursos.
- Exemplo: impedir a criação de VMs fora da região "Brasil Sul".
- Ótimo para ambientes com auditoria ou padrões ISO/LGPD.

### Azure Blueprints

- Pacotes de configuração que já incluem:
  - Políticas
  - Grupos de recursos
  - Modelos ARM
  - Controle de acesso (RBAC)
- Ótimo para criar ambientes padronizados com conformidade.

---

## 📊 Logs e Auditoria

### Azure Activity Log

- Registra **todas as ações administrativas** no portal (criação, exclusão, modificação de recursos).

### Azure Monitor + Log Analytics

- Permite criar **dashboards e consultas personalizadas** sobre eventos e métricas dos recursos.

### Microsoft Sentinel (opcional)

- SIEM nativo da Azure para **correlação de logs de segurança**, alerta e resposta a incidentes.

---

## 🛡️ Portal de Confiança da Microsoft (Service Trust Portal)

- Acesse: [https://servicetrust.microsoft.com/](https://servicetrust.microsoft.com/)
- Disponibiliza documentações sobre:
  - Conformidade com ISO, GDPR, LGPD
  - Auditorias realizadas pela Microsoft
  - Práticas de segurança e privacidade na nuvem

---

## 🐺 Microsoft Purview (Compliance e Governança de Dados)

- Plataforma de governança de dados corporativa.
- Ajuda a **identificar, classificar e proteger dados sensíveis**.
- Ótimo para quem trabalha com dados de clientes ou regulamentações como LGPD e GDPR.

### Principais Recursos do Purview:
- Catálogo de dados
- Mapeamento de linhagem (data lineage)
- Insights de conformidade

---

## 🗓️ Ações para se Preparar para uma Auditoria

1. **Ative e mantenha o Azure Policy em recursos sensíveis**
2. **Use RBAC corretamente e documente os acessos**
3. **Ative e mantenha logs de atividade e segurança**
4. **Valide se as regiões e recursos estão em conformidade com padrões internos**
5. **Use o Service Trust Portal como referência para requisitos de conformidade**
6. **Implemente tags para rastrear finalidade e responsáveis por cada recurso**

---

## 📅 Conclusão

Ao aplicar boas práticas de governança e controle de acesso, você não só melhora a segurança do seu ambiente Azure como também se prepara para auditorias e expansões futuras.

---

## 📑 Referências:

- [Azure RBAC - Microsoft Docs](https://learn.microsoft.com/pt-br/azure/role-based-access-control/overview)
- [Azure Policy](https://learn.microsoft.com/pt-br/azure/governance/policy/overview)
- [Microsoft Purview](https://learn.microsoft.com/pt-br/azure/purview/)
- [Service Trust Portal](https://servicetrust.microsoft.com/)
- [Curso AZ-900 - DIO](https://www.dio.me/)

---

Desenvolvido por [**Pedro Henrique Gomes dos Santos**](https://www.linkedin.com/in/pedro-henrique-gomes-dos-santos/)
