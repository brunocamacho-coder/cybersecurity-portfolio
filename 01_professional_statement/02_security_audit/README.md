# Auditoria de Segurança – Pequena Empresa

## 1. Introdução
Este projeto apresenta uma auditoria de segurança realizada em um ambiente corporativo simulado de pequena empresa, com o objetivo de identificar riscos, vulnerabilidades e falhas de controle que possam comprometer a confidencialidade, integridade e disponibilidade das informações.

A auditoria foi conduzida com foco em práticas de segurança defensiva, alinhadas a ambientes de SOC e Blue Team.

---

## 2. Escopo da Auditoria
A auditoria abrangeu os seguintes ativos e áreas:

- Estações de trabalho (usuários)
- Servidor local
- Rede interna
- Controle de acessos
- Políticas de segurança
- Gerenciamento de usuários
- Atualizações e patches
- Backup e recuperação

---

## 3. Metodologia
A metodologia utilizada incluiu:

- Levantamento de ativos
- Análise de configurações
- Identificação de riscos
- Avaliação de controles existentes
- Simulação de cenários de ameaça
- Classificação de impacto
- Elaboração de recomendações

---

## 4. Ativos Identificados
| Ativo | Descrição | Criticidade |
|------|-----------|-------------|
| Estações de Trabalho | Computadores dos usuários | Alta |
| Servidor Local | Armazenamento de dados e sistemas | Alta |
| Roteador | Controle de tráfego de rede | Média |
| Switch | Conectividade interna | Média |
| Banco de Dados | Informações de clientes | Alta |

---

## 5. Riscos e Vulnerabilidades Identificados

### 5.1 Falta de Política de Senhas Fortes
- **Descrição:** Senhas fracas e sem política de complexidade.
- **Risco:** Comprometimento de contas e acessos não autorizados.
- **Impacto:** Alto

### 5.2 Ausência de Atualizações Regulares
- **Descrição:** Sistemas sem atualização de segurança.
- **Risco:** Exploração de vulnerabilidades conhecidas.
- **Impacto:** Alto

### 5.3 Falta de Segmentação de Rede
- **Descrição:** Todos os dispositivos na mesma rede.
- **Risco:** Movimentação lateral em caso de ataque.
- **Impacto:** Médio

### 5.4 Backup Inexistente ou Irregular
- **Descrição:** Não há rotina definida de backup.
- **Risco:** Perda total de dados em incidentes.
- **Impacto:** Alto

---

## 6. Controles Existentes
- Antivírus instalado nas estações
- Firewall básico no roteador
- Controle manual de usuários
- Acesso físico restrito ao servidor

---

## 7. Recomendações de Segurança

### 7.1 Implementar Política de Senhas
- Mínimo de 8 caracteres
- Uso de letras maiúsculas, minúsculas, números e símbolos
- Troca periódica

### 7.2 Aplicar Atualizações e Patches
- Rotina mensal de atualização
- Monitoramento de vulnerabilidades críticas

### 7.3 Segmentar a Rede
- Separar usuários, servidores e dispositivos críticos
- Reduzir movimentação lateral

### 7.4 Implementar Rotina de Backup
- Backup diário automatizado
- Testes de restauração periódicos

---

## 8. Conclusão
A auditoria identificou riscos relevantes que podem comprometer a segurança da informação da organização. A implementação das recomendações propostas contribuirá significativamente para a redução da superfície de ataque, aumento da resiliência e fortalecimento da postura de segurança da empresa.
