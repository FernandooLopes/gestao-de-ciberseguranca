# STIX, TAXII, MISP e plataformas de inteligência de ameaças

## Padrões de compartilhamento

| Sigla | Papel |
|---|---|
| **STIX** | Forma de escrever e organizar informações sobre ameaças (alertas, malwares, IOCs, campanhas). |
| **TAXII** | Forma de transferir essas informações (o "correio" do STIX), usando HTTPS. |
| **CybOX** | Modelo de dados que descrevia eventos observáveis (logs, pacotes, processos). Hoje faz parte do STIX. |
| **MISP** | Plataforma onde várias organizações trocam dados em STIX e outros formatos. |

## Plataformas de inteligência de ameaças (TIP)

Sistemas que centralizam informações de ataques e ameaças vindas de várias fontes e as transformam em dados mais fáceis de entender para os analistas.

Tipos de informação:

- **IOC (Indicadores de Comprometimento):** rastros técnicos, como IPs maliciosos, logs, hashes e domínios.
- **TTP (Táticas, Técnicas e Procedimentos):** como os atacantes pensam e agem.
- **Reputação:** confiabilidade de domínios, IPs etc.

## Honeypot

Rede ou sistema falso criado para atrair e capturar invasores e observar o que fazem.
