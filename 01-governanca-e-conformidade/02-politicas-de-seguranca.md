# Políticas de segurança

## Três níveis de política

### Política de segurança digital (cibersegurança)
É a teoria do que precisa acontecer na prática. Exemplos:
- Proteger os dados contra acesso não autorizado.
- Exigir senhas fortes.
- Ter controle de acesso, backup, criptografia etc.

### Política específica do sistema (ex.: firewall)
Define o que pode ou não entrar na rede ou nos sistemas. Exemplos:
- Bloquear portas não utilizadas.
- Permitir acesso apenas a serviços essenciais.
- Restringir IPs externos.
- Monitorar tráfego suspeito.

### Política específica do problema (ex.: uso aceitável de e-mail e internet)
Parecida com a do firewall, mas aplicada ao comportamento do usuário. Exemplos:
- Bloquear e-mails com links suspeitos (phishing).
- Proibir AnyDesk ou TeamViewer sem autorização.
- Restringir sites não relacionados ao trabalho.
- Monitorar e registrar atividades online.

## Tipos de políticas

| Política | O que define |
|---|---|
| **Identificação e autenticação** | Identificação = ter um usuário de rede que diz quem você é. Autenticação = confirmar essa identidade (senha, 2FA, biometria, reconhecimento facial). |
| **Senhas** | Padrão seguro (ex.: 8 caracteres, maiúscula, minúscula, número) e troca periódica (ex.: a cada 3 meses). |
| **Utilização aceitável** | O que é permitido fazer com os recursos da empresa. |
| **Acesso remoto** | Diretrizes de acesso remoto e como se conectar à rede (ex.: VPN). Usar recursos da empresa para acessar outros sistemas fora dela é proibido. |
| **Manutenção de rede** | Como atualizar dispositivos corporativos. Ex.: após formatar, a máquina deve entrar no domínio, ter o antivírus da empresa e estar em conformidade. |
| **Tratamento de incidentes** | Priorizar o caso com calma, avisar diretores e supervisores, registrar o incidente, conter a propagação, corrigir e documentar para não se repetir. |
| **Dados** | Como os dados são classificados e tratados (alto, médio, baixo, confidencial, crítico, privado) e se podem ser descartados ou devem ser mantidos. |
| **Credenciais** | Regras de senha: tamanho mínimo (ex.: 8) e máximo (ex.: 16 ou 20), complexidade, frequência de troca (ex.: 90 dias), proibição de senhas fracas ou repetidas (`123456`, `senha`, `admin`). |
| **Corporativa** | Políticas internas e boas práticas da organização. |
