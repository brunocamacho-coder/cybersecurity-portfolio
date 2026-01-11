# Diário de Resposta a Incidentes – SOC

## 1. Introdução
Este projeto apresenta um registro estruturado de resposta a incidentes em um ambiente corporativo simulado, com foco em práticas de SOC e Segurança Defensiva.

O objetivo é demonstrar o processo de identificação, análise, contenção, erradicação e lições aprendidas.

---

## 2. Cenário do Incidente
- **Tipo de incidente:** Tentativa de acesso não autorizado (força bruta)
- **Origem:** Endereço IP externo desconhecido
- **Sistema afetado:** Servidor interno
- **Data/Hora:** Simulado

---

## 3. Detecção

### Fonte de Detecção:
- Logs de autenticação
- Monitoramento de eventos
- Alertas de tentativas de login mal sucedidas

### Evidência:
Múltiplas tentativas de login em curto intervalo de tempo a partir do mesmo IP.

---

## 4. Análise

- Identificado padrão de ataque automatizado
- Repetição de tentativas em diferentes usuários
- Indício de ataque de força bruta

**Classificação:** Incidente de segurança – Tentativa de comprometimento de credenciais

---

## 5. Contenção

Ações tomadas:
- Bloqueio do IP no firewall
- Restrição temporária da conta alvo
- Monitoramento intensificado

---

## 6. Erradicação

- Verificação de integridade do sistema
- Reset de senhas das contas afetadas
- Revisão de permissões
- Aplicação de patches, se necessário

---

## 7. Recuperação

- Restauração de acessos legítimos
- Validação dos serviços
- Monitoramento contínuo pós-incidente

---

## 8. Lições Aprendidas

- Necessidade de política de senhas mais forte
- Implementação de autenticação multifator
- Melhoria nas regras de alerta
- Treinamento de usuários

---

## 9. Conclusão
O incidente foi tratado de forma controlada, sem impacto significativo ao negócio. O processo de resposta demonstrou a importância de monitoramento contínuo, procedimentos definidos e atuação rápida para mitigação de riscos.
