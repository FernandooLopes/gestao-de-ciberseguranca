# Perfilamento e testes de rede

## Perfilamento de rede

Criar um perfil do tráfego do dia a dia da empresa para detectar anomalias, que podem indicar uma invasão.

| Elemento | Descrição |
|---|---|
| Duração de sessão | Tempo entre o início e o fim de um fluxo de dados. |
| Taxa de transferência total | Quantidade de dados que trafegam de uma origem a um destino em um período. |
| Portas usadas | Lista de processos TCP/UDP disponíveis para aceitar dados. |
| Espaço de endereço de ativo crítico | IPs ou localização lógica de sistemas e dados essenciais. |

## Teste de vulnerabilidade de rede

A maioria das organizações se conecta à rede pública, então testes periódicos de segurança são essenciais.

| Termo | Descrição | Ferramentas |
|---|---|---|
| **Análise de risco** | Avalia os riscos que a organização enfrenta (rede, software, tudo que possa comprometer a empresa). Visão mais estratégica. Simula o impacto de um ataque aos principais ativos. | Consultores internos ou externos, frameworks de gestão de risco |
| **Avaliação de vulnerabilidade** | Varre portas, IPs e softwares para identificar falhas antes de um invasor, gera relatórios e corrige. Inclui gerenciamento de patches. | Nessus, Nmap |
| **Teste de penetração** | Parte mais prática: usa o que foi coletado para tentar invadir, e gera relatório com falhas, como foi feito e como melhorar. | John the Ripper, Metasploit |
