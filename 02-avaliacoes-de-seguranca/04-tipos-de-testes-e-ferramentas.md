# Tipos de testes de rede e ferramentas

## Tipos de teste

| Teste | Descrição |
|---|---|
| **Teste de penetração** | Tenta achar uma brecha (porta, falha) para acessar rede, sistema ou conta. |
| **Varredura de rede** | Coleta portas, IPs e equipamentos sem DNS, entre outros dados. |
| **Varredura de vulnerabilidade** | Verifica funções incorretas e versões desatualizadas em um sistema. |
| **Cracking de senhas** | Testa senhas; contas com senha fraca podem ser quebradas (ex.: John the Ripper). |
| **Revisão de logs** | Verifica rastros do que aconteceu (ex.: quem apagou um app de um servidor). |
| **Verificação de integridade** | Monitora os hashes dos arquivos em tempo real. |
| **Detecção de vírus/malware** | O antivírus detecta malware em atividade. |

## Aplicando os resultados

Corrigir as falhas encontradas (fechar portas, trocar senhas) e tomar decisões conforme as políticas da empresa e o melhor custo-benefício.

## Ferramentas

| Ferramenta | Para que serve |
|---|---|
| **Nmap** | Explorar DNS, portas, SO e serviços. |
| **SuperScan** | Varredura básica TCP/IP, somente Windows (parecida com o Nmap, mas não igual). |
| **SIEM** | Relatórios automáticos de vulnerabilidades e incidentes a partir de logs. |
| **GFI LanGuard** | Faz a varredura e sugere melhorias e correções. |
| **Tripwire** | Avalia se as operações estão em conformidade com as políticas de TI (integridade). |
| **Nessus** | Encontra os pontos mais fracos da rede e ajuda a priorizá-los; foco em acesso remoto, erros de configuração e DoS contra a pilha TCP/IP. |
| **L0phtCrack** | Auditoria e recuperação de senhas. |
| **Metasploit** | Informações sobre vulnerabilidades e apoio à penetração. |
| **John the Ripper** | Cracking de senhas. |
