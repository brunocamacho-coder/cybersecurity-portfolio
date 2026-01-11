# Análise de Eventos com SQL (Detecção de Incidentes)

## 1. Introdução
Este projeto demonstra a utilização de consultas SQL para análise de eventos de segurança, com foco na identificação de atividades suspeitas, tentativas de acesso indevido e possíveis incidentes de segurança.

A abordagem é alinhada às práticas de SOC e monitoramento contínuo.

---

## 2. Objetivo
Utilizar filtros SQL para:
- Identificar tentativas de login mal sucedidas
- Detectar acessos fora do horário comercial
- Localizar atividades incomuns
- Apoiar a resposta a incidentes

---

## 3. Cenário Simulado
Foi utilizado um conjunto de registros de eventos (logs) simulados contendo:
- Tentativas de login
- Acessos autorizados e negados
- Alterações de permissões
- Eventos administrativos

---

## 4. Ferramentas Utilizadas
- Banco de dados relacional (MySQL / SQLite)
- SQL
- Ambiente de laboratório

---

## 5. Consultas SQL Utilizadas

### 5.1 Tentativas de Login Mal Sucedidas
```sql
SELECT * 
FROM logs 
WHERE event_type = 'FAILED_LOGIN';
