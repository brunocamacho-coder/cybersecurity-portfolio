# Análise de Rede e Superfície de Ataque

## 1. Introdução
Este projeto apresenta uma análise da rede e da superfície de ataque de um ambiente corporativo simulado, com o objetivo de identificar exposições, serviços desnecessários e potenciais vetores de ataque.

A análise foi realizada com foco em práticas de Blue Team e Segurança Defensiva.

---

## 2. Escopo da Análise
A análise abrangeu:

- Hosts ativos na rede
- Portas abertas
- Serviços em execução
- Protocolos utilizados
- Possíveis pontos de entrada

---

## 3. Metodologia
A metodologia incluiu:

- Descoberta de hosts
- Varredura de portas
- Identificação de serviços
- Análise de risco por serviço exposto
- Avaliação de impacto
- Proposição de mitigação

---

## 4. Ferramentas Utilizadas
- Nmap
- Kali Linux
- Wireshark (análise conceitual)
- Ambiente virtualizado

---

## 5. Resultados da Análise

### 5.1 Hosts Identificados
Foram identificados múltiplos dispositivos ativos na rede interna, incluindo estações de trabalho, servidor e roteador.

### 5.2 Portas e Serviços Abertos (Exemplo)
| Porta | Serviço | Risco |
|------|--------|------|
| 22 | SSH | Médio |
| 80 | HTTP | Médio |
| 445 | SMB | Alto |
| 3389 | RDP | Alto |

---

## 6. Análise de Riscos

### 6.1 Serviço SMB (Porta 445)
- **Risco:** Exploração de vulnerabilidades conhecidas e movimentação lateral.
- **Impacto:** Alto
- **Observação:** Serviço comum em ataques internos.

### 6.2 Serviço RDP (Porta 3389)
- **Risco:** Ataques de força bruta e acesso remoto indevido.
- **Impacto:** Alto
- **Observação:** Requer controle rigoroso.

---

## 7. Recomendações de Segurança

- Restringir serviços desnecessários
- Implementar firewall interno
- Utilizar VPN para acessos remotos
- Monitorar tentativas de conexão
- Segmentar a rede
- Aplicar princípio do menor privilégio

---

## 8. Conclusão
A análise demonstrou que a exposição de serviços críticos aumenta significativamente a superfície de ataque. A aplicação das recomendações propostas contribuirá para reduzir riscos, fortalecer a postura de segurança e aumentar a resiliência do ambiente.
