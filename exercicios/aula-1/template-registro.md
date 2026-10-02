# Registro individual — AV1.1

Estudante: Gabriel Pedroza Rodrigues — Data: 01/10/2026

Origem: cartões C1–C3 fictícios do enunciado.

| Cartão | Como faria sem IA / entrada e resultado | Modalidade e justificativa ligada ao cartão | O que conferir para aprovar | Responsável humano |
|---|---|---|---|---|
| C1 | Ler os critérios de R2 e fornecê-los para o responsável. Produziria um documento descrevendo que a listagem inclui `aberto` e `em_andamento`, exclui `fechado`, preservando a ordem de entrada. | Sem IA, os critérios já estão bem definidos e comprovados. | A listagem de chamados deve respeitar os critérios de R2. Por exemplo: Não exibir chamados fechados, abrir dois chamados e verificar se o primeiro inserido é o primeiro exibido. | Manutenção |
| C2 | entrada: chamado fechado para oficina, saída esperada: pessoas do laboratório sem visualização de chamados da oficia, justificativa: segregação das solicitações com base em escopo de atuação | Sem IA, cenário de teste simples e com poucas variáveis envolvidas. | O filtro de chamados deve respeitar R3, os chamados de laboratório não devem estar visíveis para oficina | gestão responsável |
| C3 | Não autorizar a mudança, sem verificações e aprovações disponíveis | Sem delegar a decisão, a aprovação depende de confirmação humana | Verificar quais dados foram afetados e cobrar aprovação pelo responsável | gestão responsável |

**Exemplo que sustenta minha decisão (C3)** Falta a regra nova, a aprovação pelo responsável e principalmente os dados afetados. Sem essas informações não é possível garantir assertividade na mudança, por mais emergencial que ela seja, o impacto do rollback é maior que o de não autorizar.

**Alternativa para o cartão C3:** Utilizar como base para aprovação da mudança apenas o resumo “facilitar acesso entre áreas”.
**Comparação com minha escolha (restrição e consequência):** Minha escolha é mais conservadora e não permite a mudança sem as validações e regras necessárias, já a alternativa é arriscada e sem a mínima garantia.
**Limite da delegação e condição para rever a escolha:** Aprovação de mudança em produção não pode ser delegada, apenas a gestão responsável tem a permissão nesse caso. Revejo minha escolha caso os dados afetados, as verificações e principalmente as aprovações necessárias fossem aprovadas pelos responsáveis.

**Uso de IA na elaboração deste registro:** não utilizada / ferramenta e modelo visíveis: não utilizada. O raciocínio e a decisão registrados são meus.

**Revisão:** [x] três decisões; [x] exemplo explicado; [x] alternativa e limite; [x] até uma página.
