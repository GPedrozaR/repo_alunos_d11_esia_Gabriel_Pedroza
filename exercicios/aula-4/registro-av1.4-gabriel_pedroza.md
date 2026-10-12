# Registro individual — AV1.4

Estudante: Gabriel Pedroza Rodrigues — Data: 11/10/2026

**Critério de aceite por R2:** Para R2, as obrigações são: incluir `aberto` e `em_andamento`, excluir `fechado` e preservar a ordem de entrada.

| Entrada | IDs esperados por R2 | IDs do candidato | Status: inferido/observado | Mecanismo/trecho essencial |
|---|---|---|---|---|
| TR-41, TR-42, TR-43, TR-44 | TR-41, TR-42, TR-44 | TR-42, TR-44, TR-41 | inferido por inspeção | `ativos = [c for c in chamados if c["estado"] in ("aberto", "em_andamento")]`; `return sorted(ativos, key=lambda c: c["impacto"] + c["urgencia"], reverse=True)` |

**Teste entregue — o que verifica e o que não consegue distinguir:** Verifica a lista de IDs retornada, e não confere o estado, mas detecta a inclusão de TR-43.

**Trecho do teste (entrada e comparação de IDs) que sustenta minha análise:** entrada do teste: os mesmos registros na ordem TR-42, TR-44, TR-41, TR-43; asserção: compara os IDs retornados a `["TR-42", "TR-44", "TR-41"]`.

**Decisão (aceitar, aceitar com condições ou rejeitar) e motivo:** Rejeitar. Motivo: O candidato não cumpre R2 porque não cumpre a obrigação de preservar a ordem de entrada.

**Comparação entre manter e ajustar / responsável pelo aceite:** Manter a regra vai tornar o comportamento incorreto, ajustá-lo e preservar a ordem de entrada. Responsável pelo aceite: responsável pela manutenção do Fila Clara.

**Ajuste proposto (texto ou código):** remover a ordenação por impacto e urgência, mantendo a ordem de entrada.

```python
def listar_ativos_proposta(chamados):
    ativos = [c for c in chamados if c["estado"] in ("aberto", "em_andamento")]
    return ativos
```

| Caso para conferir o ajuste: entrada e ordem | IDs esperados | Resultado previsto ou observado / status |
|---|---|---|
| TR-41, TR-42, TR-43, TR-44 | TR-41, TR-42, TR-44 | previsto por leitura; execução não realizada |

**Limite remanescente e condição para rever o parecer:** A análise não cobriu o estado. A evidência que faria rever o parecer seria chamados com estado fechado serem persistidos no retorno.

**Origem dos dados e da análise:** candidato/teste/entrada simulados; método próprio: inspeção por leitura; comando e trecho de saída, se executado: não realizado.

**Uso de IA neste registro:** utilizada. Ferramenta-modelo visível: OpenCode, modelo claude-haiku-5-5. Tarefa/contexto: leitura dos materiais, criação do arquivo a partir do modelo, transcrição de textos aprovados por mim, explicação do processo, exemplo com outra função (`listar_pendentes`) e conferência das respostas. Trecho aproveitado: transcrições de frases e decisões que eu escrevi ou aprovei, e o código de ajuste que eu conferi. Minha verificação: conferi cada lista de IDs, a linha de `sorted` e a comparação com a asserção do teste; corrigi frases com erro de leitura; a análise, a decisão, o motivo, o limite e a condição para rever são minhas.

**Revisão:** [x] comparação com R2; [x] alcance do teste; [x] ajuste/revalidação; [x] status; [x] uma página.
