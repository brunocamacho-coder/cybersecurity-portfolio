# Análise de Logs – Investigação de Eventos de Segurança

## 1. Introdução
Este projeto demonstra a análise de logs de sistemas para identificação de atividades suspeitas, comportamentos anômalos e possíveis incidentes de segurança.

A abordagem é alinhada à operação de SOC e ao uso de SIEM para monitoramento contínuo.

---

## 2. Objetivo
Analisar registros de eventos para:
- Identificar tentativas de acesso não autorizado
- Detectar padrões suspeitos
- Apoiar a investigação de incidentes
- Fornecer evidências para resposta

---

## 3. Fontes de Log Analisadas
- Logs de autenticação (Linux / Windows)
- Logs de sistema
- Logs de aplicação
- Logs de firewall (conceitual)

---

## 4. Ferramentas Utilizadas
- Arquivos de log (auth.log, syslog, event viewer)
- Linux
- Terminal
- SIEM (conceitual – Wazuh)

---

## 5. Eventos Identificados

### 5.1 Tentativas de Login Mal Sucedidas
- **Descrição:** Múltiplas falhas de autenticação em curto período
- **Risco:** Ataque de força bruta
- **Impacto:** Alto

---

### 5.2 Acessos Fora do Horário Padrão
- **Descrição:** Logins realizados fora do horário comercial
- **Risco:** Atividade suspeita
- **Impacto:** Médio

---

### 5.3 Execução de Comandos Suspeitos
- **Descrição:** Execução de comandos administrativos por usuários comuns
- **Risco:** Escalada de privilégio
- **Impacto:** Alto

---

## 6. Análise

- Correlação de eventos por IP
- Verificação de horários incomuns
- Identificação de padrões repetitivos
- Avaliação de impacto potencial

Os eventos foram classificados como indicadores de possível incidente.

---

## 7. Recomendações

- Implementar regras de alerta no SIEM
- Restringir acessos administrativos
- Aplicar autenticação multifator
- Monitorar continuamente
- Revisar políticas de acesso

---

## 8. Conclusão
A análise de logs é fundamental para a detecção precoce de incidentes. A interpretação correta dos eventos permite resposta rápida, redução de impacto e fortalecimento da postura de segurança do ambiente.
