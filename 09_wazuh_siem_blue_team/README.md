# Wazuh SIEM – Projeto Blue Team / SOC

## 📌 Visão Geral

Este projeto demonstra um **fluxo prático de Blue Team / SOC** utilizando o **Wazuh SIEM** em um ambiente Linux.

O foco está em **detecção, correlação de eventos e resposta a incidentes**, simulando atividades reais de um **Security Operations Center (SOC)**.

O cenário principal simula um **ataque de força bruta via SSH**, desde a geração dos eventos até a análise dos logs, correlação no SIEM e documentação do incidente conforme boas práticas de segurança defensiva.

---

## 🎯 Objetivos

- Detectar atividades maliciosas relacionadas ao SSH utilizando regras de SIEM  
- Correlacionar eventos de segurança para identificar padrões de ataque  
- Analisar logs de autenticação do Linux  
- Documentar o incidente seguindo práticas reais de SOC  
- Mapear a detecção ao **MITRE ATT&CK (T1110 – Brute Force)**  

---

## 🧪 Ambiente

- Ubuntu 22.04 (WSL2)  
- Wazuh SIEM  
- OpenSSH  
- Logs de autenticação Linux (`/var/log/auth.log`)  

---

## 🔍 Detecção do Ataque

O ataque é identificado através de múltiplas tentativas de autenticação SSH com falha em um curto intervalo de tempo.

Eventos monitorados:
- `Failed password for invalid user`
- `Authentication failure`
- Múltiplas tentativas de login a partir do mesmo IP

A correlação de eventos permite identificar **tentativas de força bruta** antes que uma conta seja comprometida com sucesso.

---

## ⚠️ Considerações sobre Falsos Positivos

Possíveis falsos positivos podem ocorrer em situações como:
- Atividades administrativas legítimas
- Scripts automatizados mal configurados
- Ferramentas de varredura de segurança

O uso de **limiares (thresholds)** e **correlação de eventos** ajuda a reduzir ruído e aumentar a precisão dos alertas.

---

## 🧭 Mapeamento MITRE ATT&CK

| Técnica | Descrição |
|-------|----------|
| T1110 | Brute Force |
| T1110.001 | Password Guessing |

---

## 📝 Registro de Incidente (SOC)

- **Tipo de incidente:** Tentativa de força bruta via SSH  
- **Origem:** IP local (ambiente de laboratório)  
- **Impacto:** Nenhum acesso bem-sucedido  
- **Ação tomada:** Monitoramento, correlação e documentação  
- **Status:** Encerrado (ambiente controlado)  

---

## 📚 Aprendizados

- Importância da correlação de eventos em SIEM  
- Visão prática do trabalho de um analista SOC / Blue Team  
- Alinhamento entre logs, detecção e resposta a incidentes  
- Documentação clara e estruturada para auditoria e melhoria contínua  

---

## 🔗 Observação

Este projeto faz parte do meu **portfólio profissional em Cibersegurança**, com foco em:

- SOC Analyst  
- Blue Team  
- SIEM  
- Incident Response  
- Segurança Defensiva  
