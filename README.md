# LAB - Gerenciando Políticas em Acessos Azure. (AZ900 | DIO)

Este documento tem como objetivo apresentar, de maneira simples e prática, como um estudante de DevOps iniciante pode entender e aplicar os conceitos de **governança**, **conformidade** e **segurança de acessos** na nuvem Microsoft Azure. O conteúdo foi elaborado com base nas aulas da trilha de formação AZ-900.

---

## 🔐 Governança e Conformidade no Azure

Governança em nuvem é o conjunto de regras, diretrizes e processos usados para controlar como os recursos são criados, gerenciados e acessados. Ela anda junto com a conformidade, que garante que sua infraestrutura esteja em linha com leis e políticas internas ou externas (como LGPD, ISO, etc).

---

## ⚖️ Políticas de Acesso e Controle (RBAC)

O Azure utiliza o modelo **RBAC (Role-Based Access Control)** para definir permissões com base em funções.

### ✅ Exemplo de Funções Padrão:
- **Proprietário (Owner)**: controle total
- **Colaborador (Contributor)**: pode alterar recursos, mas não delegar permissões
- **Leitor (Reader)**: acesso apenas leitura

Essas permissões podem ser aplicadas por:
- **Nível de Assinatura**
- **Grupo de Recursos**
- **Recurso Específico**

---

## 📊 Monitoramento com Logs

### 🔢 Tipos de Logs:
- **Activity Logs**: mostram quem fez o quê no ambiente Azure
- **Diagnostic Logs**: mostram eventos específicos de serviços (ex: acesso a banco, upload em blob)
- **Sign-In Logs**: mostram tentativas de login, localização e status (falha, sucesso)

Esses logs podem ser:
- Visualizados no portal
- Exportados para uma conta de armazenamento
- Integrados com ferramentas como Log Analytics e Microsoft Sentinel

### 🌍 Exemplo prático:
- Criar alerta para tentativas de login com falha consecutiva
- Identificar quem excluiu um recurso
- Auditar mudanças em configurações de rede

---

## ⚖️ Azure Policy - Políticas de Governança

O **Azure Policy** permite criar regras para garantir conformidade.

### 🔢 Exemplos:
- Não permitir criação de VMs fora da região "Brazil South"
- Bloquear uso de máquinas de alto custo
- Obrigar uso de tags em todos os recursos

### 🔧 Como aplicar:
1. Acesse "Políticas" no portal
2. Crie uma **iniciativa** ou **definição de política**
3. Aplique à assinatura ou grupo de recursos
4. Acompanhe os recursos que estão ou não em conformidade

---

## 🌐 Portal de Confiança da Microsoft

O **Microsoft Trust Center** é uma página pública com informações sobre:
- Certificações de conformidade (ISO, SOC, GDPR, etc)
- Estrutura de segurança da Azure
- Relatórios e whitepapers de auditoria

Acesse: [https://www.microsoft.com/trust-center](https://www.microsoft.com/trust-center)

---

## 📆 Auditoria: O que Validar?

Se uma auditoria for solicitada, esteja pronto para apresentar:
- Quem tem acesso ao quê (RBAC)
- Quais mudanças foram feitas e por quem (Activity Logs)
- Políticas aplicadas e conformidade (Azure Policy)
- Logs de login e tentativas suspeitas (Sign-In Logs)
- Documentação de justificativas e exceções

---

## 📅 Boas Práticas de Governança

- Sempre use **grupos de recursos bem organizados**
- Crie **orçamentos (budgets)** e **políticas de custo**
- Aplique **políticas obrigatórias** antes da liberação de recursos
- Utilize **logs e alertas** para monitoramento contínuo
- Revise acessos periodicamente com base nas funções

---

## 📄 Conclusão

Governança e conformidade não são apenas "documentação para auditor". São ferramentas que evitam riscos, economizam recursos e ajudam você a manter um ambiente de nuvem seguro e organizado.

---

## 📅 Referências:

- [Documentação Microsoft - Governança](https://learn.microsoft.com/pt-br/azure/governance/)
- [Microsoft Trust Center](https://www.microsoft.com/trust-center)
- [Documentação Azure Policy](https://learn.microsoft.com/pt-br/azure/governance/policy/overview)
- [Trilha AZ-900 DIO](https://www.dio.me/)

---

Desenvolvido por [**Pedro Henrique Gomes dos Santos**](https://www.linkedin.com/in/pedro-henrique-gomes-dos-santos/)
