# Desafio de Penetration Testing: Medusa & Metasploitable 2

Este repositório documenta o passo a passo realizado durante o desafio de invasão controlada, utilizando a máquina virtual **Metasploitable 2** como alvo e o **Kali Linux** como estação de ataque. O foco principal foi o uso da ferramenta **Medusa** para ataques de força bruta.

## 🛠️ Cenário de Teste
* **Atacante:** Kali Linux
* **Alvo:** Metasploitable 2 (Vulnerable VM)
* **IP do Alvo:** `192.168.56.102/24`
* **Ferramentas:** Medusa, Enum4linux, Bash.

---

## 📋 Metodologia e Preparação

### 1. Enumeração do Sistema
Antes do ataque, foi utilizada a ferramenta `enum4linux` para coletar informações sobre usuários, grupos e compartilhamentos do alvo. O resultado foi espelhado no terminal e salvo em um arquivo de log.

```bash
enum4linux -a 192.168.56.102 | tee enum4_output.txt# AULA-Simulando-ataque-brute-force
