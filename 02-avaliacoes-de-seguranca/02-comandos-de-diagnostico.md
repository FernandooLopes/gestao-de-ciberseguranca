# Utilitários de diagnóstico de linha de comando

> Os exemplos de saída abaixo usam valores fictícios (faixas de IP reservadas para documentação) para não expor nenhuma rede real.

| Comando | Para que serve | Equivalente Linux/Mac |
|---|---|---|
| `ipconfig` | Mostra a configuração TCP/IP (IP, máscara, gateway, DNS, MAC) | `ifconfig` / `ip a` |
| `ping` | Testa conectividade enviando ICMP e verifica se há rota até o host | `ping` |
| `arp` | Tabela que mapeia IPs para endereços MAC; achar o MAC de um dispositivo | `arp` |
| `tracert` | Rastreia a rota (saltos) de um pacote até o destino | `traceroute` |
| `nslookup` | Consulta um servidor DNS | `dig` |
| `netstat` | Lista portas em escuta e conexões ativas | `netstat` / `ss` |
| `nbtstat` | Diagnostica resolução de nomes NetBIOS (Windows) | — |
| `nmap` | Auditoria de segurança: localiza hosts, detecta SO e identifica serviços | `nmap` |
| `netcat` | Coleta informações de conexões TCP/UDP; varredura de portas, monitoramento, captura de banner, cópia de arquivos | `nc` |
| `hping` | Monta e analisa pacotes; varredura de portas, descoberta de caminho, impressão digital do SO, teste de firewall | `hping3` |

## Exemplos

### ipconfig
```text
Adaptador de Rede sem Fio Wi-Fi:

   Endereço IPv4. . . . . . . . . . . . . . : 192.0.2.25
   Máscara de Sub-rede . . . . . . . . . . . : 255.255.255.0
   Gateway Padrão. . . . . . . . . . . . . . : 192.0.2.1
```

### ping
```text
> ping 1.1.1.1

Resposta de 1.1.1.1: bytes=32 tempo=9ms TTL=54
Resposta de 1.1.1.1: bytes=32 tempo=16ms TTL=54
Resposta de 1.1.1.1: bytes=32 tempo=10ms TTL=54
Resposta de 1.1.1.1: bytes=32 tempo=9ms TTL=54

Pacotes: Enviados = 4, Recebidos = 4, Perdidos = 0 (0% de perda)
Mínimo = 9ms, Máximo = 16ms, Média = 11ms
```

### arp
```text
> arp -a 192.0.2.1

Endereço IP     Endereço físico      Tipo
192.0.2.1       00-00-5e-00-53-01    dinâmico
```

### tracert
```text
> tracert 1.1.1.1

  1     2 ms     3 ms     3 ms  192.0.2.1
  2     *        *        *     Esgotado o tempo limite do pedido.
  3    16 ms    17 ms    10 ms  (provedor)
  ...
 10     9 ms     9 ms     9 ms  one.one.one.one [1.1.1.1]

Rastreamento concluído.
```
O `*` indica um salto que não respondeu. Ajuda a localizar onde o pacote está sendo perdido.

### nslookup
```text
> nslookup one.one.one.one

Não é resposta autoritativa:
Nome:    one.one.one.one
Addresses:  2606:4700:4700::1111
            2606:4700:4700::1001
            1.1.1.1
            1.0.0.1
```

### netstat
```text
> netstat

Proto  Endereço local       Endereço externo      Estado
TCP    192.0.2.25:49417     198.51.100.10:https   ESTABLISHED
TCP    192.0.2.25:54566     198.51.100.20:https   ESTABLISHED
TCP    192.0.2.25:56911     198.51.100.30:https   TIME_WAIT
TCP    127.0.0.1:57225      127.0.0.1:17713       SYN_SENT
```
Estados comuns: `ESTABLISHED` (conexão ativa), `TIME_WAIT` (encerrando), `SYN_SENT` (tentando conectar).
