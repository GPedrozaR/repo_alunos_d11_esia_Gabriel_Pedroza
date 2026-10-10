# Registro individual — AV1.3

Estudante: Gabriel Pedroza Rodrigues — Data: 10/10/2026

**O que a listagem e a documentação precisam cumprir, conforme R2/R4:** Para R2, as obrigações são: incluir `aberto` e `em_andamento`, excluir `fechado` e preservar a ordem de entrada. Para R4, a obrigação é a documentação descrever o mesmo comportamento do contrato.

| Caso / estado a verificar | Entrada (IDs e ordem) | IDs esperados na ordem | Obrigação de R2 e como verificar |
|---|---|---|---|
| 1 / aberto | TR-33, Oficina, aberto, 2, 3 | [TR-33] | Incluir `aberto`. Conferir: TR-33 aparece na saída. |
| 2 / em_andamento | TR-31, Oficina, em_andamento, 1, 1 | [TR-31] | Incluir `em_andamento`. Conferir: TR-31 aparece na saída. |
| 3 / fechado | TR-32, Laboratório, fechado, 3, 3 | [] | Excluir `fechado`. Conferir: saída vazia, sem TR-32. |

**Entrada combinada TR-31, TR-32, TR-33 → IDs esperados:** TR-31, TR-33. TR-32 é excluído por estar `fechado`. Saída esperada calculada por R2; execução não realizada.

**Como conferiria a ordem (compare a posição dos IDs na entrada e na saída esperada):** na entrada, TR-31 está na posição 1 e TR-33 na posição 3. Na saída esperada, TR-31 vem antes de TR-33, mantendo a sequência relativa. Como conferir: a posição relativa de TR-31 e TR-33 na saída deve ser igual à da entrada.

**Documentação proposta (até três frases):** A listagem de chamados ativos devolve, na ordem de entrada, somente os chamados com estado `aberto` ou `em_andamento`. Chamados com estado `fechado` são excluídos da lista.

**Etapa em que admitiria IA / tarefa que ela faria / pessoa responsável por conferir:** etapa de rascunho dos três casos a partir de R2 / tarefa delegada: gerar o rascunho da tabela de casos / Eu.

**O que essa pessoa deve verificar antes de aprovar:** cada saída esperada igual à regra de R2 (`aberto` e `em_andamento` incluídos, `fechado` excluído); TR-31 antes de TR-33 na saída.

**Alternativa sem IA e comparação:** redigir os três casos e a documentação diretamente a partir de R2. Diferença de esforço ou de possibilidade de erro: não descrita no projeto.

**O que os casos não verificam e o que me faria rever a aprovação:** os casos não tratam entradas inválidas e não cobrem R1 nem R3. Revisaria o aceite se a execução retornasse lista diferente das esperadas ou se a documentação divergisse de R2.

**Origem dos dados e como fiz a análise:** entrada fictícia do enunciado; esperado por contrato: R2; inspeção própria: cálculo manual de cada caso contra R2; execução opcional (comando/resultado, se houver): não realizada.

**Uso de IA neste registro:** utilizada. Ferramenta-modelo visível: OpenCode, modelo claude-haiku-5-5; contexto/tarefa: leitura dos materiais e rascunho dos casos; trecho aproveitado: estrutura dos casos; minha verificação: conferi cada saída esperada, a ordem e a documentação contra R2.

**Revisão:** [x] três estados; [x] ordem; [x] texto; [x] aceite/limite; [x] uma página.
