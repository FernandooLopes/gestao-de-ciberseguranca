# CVSS — Common Vulnerability Scoring System

Avalia a gravidade de uma vulnerabilidade com uma nota de **0 a 10**: perto de 0 é pouco preocupante, perto de 10 é crítico.

## Exemplo de divulgação responsável

1. O pesquisador descobre a falha.
2. Avisa a empresa.
3. A empresa confirma e solicita um identificador CVE.
4. A empresa tem até 90 dias para corrigir.
5. Depois de 90 dias, a CVE é publicada para que todos tomem cuidado.

## Grupos de métricas

| Grupo | O que mede |
|---|---|
| **Base** | Quão perigosa é a vulnerabilidade em si (o significado padrão do CVSS). |
| **Temporal** | Como o perigo muda com o tempo, por exemplo quando sai um exploit (piora) ou um patch (melhora). |
| **Ambiental** | Quão perigosa é no *meu* ambiente: afeta um banco de dados ou servidor importante? |
