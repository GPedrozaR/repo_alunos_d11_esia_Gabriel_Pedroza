# Registro individual — AV1.1

Estudante: Gabriel Pedroza Rodrigues — Data: 10/10/2026

Origem: cartões C1–C3 fictícios do enunciado.

| Cartão | Como faria sem IA / entrada e resultado | Modalidade e justificativa ligada ao cartão | O que conferir para aprovar | Responsável humano |
|---|---|---|---|---|
| C1 | Leria R2 e escreveria um critério para cada obrigação: inclusão de aberto, inclusão de em_andamento, exclusão de fechado e preservação da ordem relativa. Produto: lista de critérios de aceite. | Com assistência. A IA redige a primeira versão; eu revisaria cada critério contra R2. | (1) A saída não contém nenhum registro com estado fechado; (2) todo registro aberto e em_andamento da entrada aparece na saída; (3) a ordem relativa dos registros mantidos é igual à da entrada; (4) nenhum critério acrescenta filtro, ordenação ou regra fora de R2. | Responsável Manutenção |
| C2 | Por R3, para a entrada departamento=Laboratório e estado=aberto com solicitante Oficina, espero `False`, pois a pessoa só visualiza chamados do próprio departamento, independentemente do estado. | Sem IA. O teste é curto e o esperado vem de R3. | A saída retornada é `False` para solicitante de outro departamento, independentemente do estado. | Responsável Testes |
| C3 | Ler o resumo "facilitar acesso entre áreas" e listar o que falta: regra nova, dados afetados, verificações e responsável pela aprovação. Resultado: decisão de não autorizar nas condições atuais. | Sem delegar a decisão. A regra, os dados, as verificações e o aprovador não foram confirmados, então a decisão fica com uma pessoa. | Autorizar somente se todas as condições forem satisfeitas: (1) a regra nova estiver descrita por escrito; (2) os dados afetados estiverem listados; (3) houver verificação para esses dados; (4) o responsável pela aprovação estiver identificado. Sem isso, não autorizar. | Responsável Gestão |

**Exemplo que sustenta minha decisão (C3):** Falta a regra nova, os dados afetados, as verificações e o responsável pela aprovação. Sem essas informações, não é possível verificar se a mudança atende à visibilidade de R3, ainda que o pedido seja urgente.

**Alternativa para o cartão C3:** usar o resumo "facilitar acesso entre áreas" como base para autorizar a mudança.
**Comparação com minha escolha (restrição e consequência):** não autorizar é mais conservador; a alternativa autoriza sem a regra, os dados e as verificações, então não há como conferir o resultado.
**Limite da delegação e condição para rever a escolha:** a decisão de autorizar a mudança em produção permanece com uma pessoa. Revejo a escolha se a regra nova, os dados afetados, as verificações e o aprovador identificado estiverem disponíveis.

**Uso de IA na elaboração deste registro:** utilizada. Ferramenta e modelo: OpenCode, modelo claude-haiku-5-5. Tarefa e contexto: revisão das linhas C1, C2 e C3 contra os critérios da atividade e contra R2 e R3. Trecho aproveitado: parte da redação das linhas C1, C2 e C3. Minha verificação/intervenção: conferi cada critério e cada saída esperada com os critérios da atividade e com R2 e R3; corrigi ou removi trechos sem base no caso e reescrevi com minhas palavras o que mantive. O raciocínio e a decisão registrados são meus.

**Revisão:** [x] três decisões; [x] exemplo explicado; [x] alternativa e limite; [x] até uma página.
