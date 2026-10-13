# Entrega individual — AV3

Estudante: Gabriel Pedroza Rodrigues · Data: 12/10/2026 · Caso/recorte: Documentação das regras R1–R3 de Fila Clara com apoio de IA (R4)

## Parecer

**1. Recomendação e problema.** Recomendo uso condicionado de IA para propor a documentação das regras R1–R3 de Fila Clara, com revisão humana e confronto de cada trecho com o contrato antes de publicar, para a tarefa de redigir ou atualizar a descrição dessas regras, cujo beneficiário é a manutenção de Fila Clara e resultado esperado é um texto de documentação conferido contra cada regra. As restrições relevantes são: o contrato exige que texto gerado com apoio de IA seja confrontado com R4.

| Alternativa | Processo e recursos | Benefício esperado / pressuposto | Limite, consequência do erro e esforço de verificação |
|---|---|---|---|
| A — sem IA | A equipe redige a documentação a partir de R1–R4 e revisa entre pares (proposta de processo). | Texto de autoria humana; depende de quem conhece o contrato. | Um trecho impreciso pode passar; a verificação é a revisão entre pares. |
| B — outra alternativa | A IA propõe o texto; a equipe confere cada afirmação contra R1–R4 antes de publicar. | Redação possivelmente mais rápida (pressuposto não medido). | A IA pode descrever uma regra de forma diferente do contrato; a verificação é o confronto trecho a trecho. |

**Minha comparação e razão para a recomendação:** a alternativa B só é preferível se cada afirmação for conferida contra o contrato antes da publicação. Sem essa condição, recomendo a alternativa A, porque ela não depende de conferir texto gerado por IA contra R1–R4, enquanto B publicaria trechos que não foram verificados.

**2. Autonomia e responsabilidade.** Etapa/tarefa assistida, se recomendada: a IA propõe um rascunho do texto de documentação de R1–R3, sem publicação direta. 
O que permanece sob aceite humano / critério e responsável: publicação de qualquer trecho, após conferência de cada afirmação contra as regras (R1-R4). Responsável pela conferência: a pessoa que a gestora designar para a revisão da documentação. Condição de intervenção, tratamento de exceção e reversibilidade/recusa: se um trecho divergir do contrato, a equipe o recusa ou reescreve e registra a divergência; a publicação fica suspensa até a correção

**3. Verificação e contraponto.** Evidência E1 do anexo: registro de AV2, caso T2 (chamado V-02, departamento Oficina, estado fechado, solicitante Oficina); critério aplicado: R3, acesso independentemente de estado; resultado/status: retorno falso, esperado verdadeiro, divergente, inferido por inspeção, não executado; interpretação que sustenta a recomendação: a documentação candidata descrevia um filtro de estado que R3 não prevê, e só o confronto com o contrato revelou a divergência, o que sustenta a condição de conferir cada trecho antes de publicar.
Limitação ou evidência contrária E2: os quatro casos da AV2 não cobrem o acesso do Laboratório a chamados do Laboratório, e os resultados são inferidos por inspeção, sem execução; efeito na recomendação e condição que a mudaria: reduz a confiança de que a regra de visibilidade está validada; se essa verificação retornar resultado diferente do que R3 exige, a recomendação de uso condicionado precisa ser revista.

**4. Riscos e mecanismos.**

| Risco e consequência no recorte | Mecanismo | Responsável | Evidência e como conferir o controle | Exceção/interrupção |
|---|---|---|---|---|
| 1 — Publicar documentação que descreve uma regra de forma diferente de R1–R3, como o filtro de estado do caso T2 (AV2). | Conferência de cada afirmação do texto contra R1–R4 antes da publicação. | A pessoa que a gestora designar para a revisão da documentação. | Registro datado de cada revisão, com o trecho conferido, a regra usada e o resultado. Quem confere: outra pessoa da equipe, por amostragem. | Se um trecho divergir, a publicação fica suspensa até correção; a divergência é registrada. |
| 2 — Apresentar a regra de visibilidade como mecanismo de segurança, embora o contrato diga que ela é didática. | Frase obrigatória de escopo didático em qualquer texto sobre visibilidade, e checagem de que o texto não diz "seguro" ou equivalente. | O revisor do texto, o mesmo da revisão da documentação. | Presença da frase de escopo e ausência de afirmações de segurança, conferidas no próprio texto publicado. | Texto sem a frase ou com afirmação de segurança não é publicado; se já publicado, é retirado até correção. |

**5. Maturidade e próximo passo.** Objeto e estágio: uso de IA pela manutenção para propor documentação das regras R1–R3; estágio: protótipo; definição adotada: artefato demonstrável em ambiente controlado; fatos que o sustentam: M1, M2 e M3; estágio rival e motivo da distinção: piloto, porque M5 e M6 indicam ausência de execução e de resultados; lacuna: nenhuma execução do plano nem resultado medido.
Passo proposto — tarefa, participantes, duração, dados e responsável: execução do plano de duas semanas de M4, com duas pessoas da manutenção e dados sintéticos; responsável: a pessoa designada conforme M2.
Métrica (fórmula/unidade e, se taxa, numerador/denominador): proporção de propostas aprovadas sem divergência na conferência contra R1–R4; numerador: propostas sem divergência; denominador: propostas conferidas.
Coleta e referência de comparação: registro de cada conferência, comparado com texto redigido pela equipe pelo mesmo critério; limite da medida: mede apenas aderência ao contrato com dados sintéticos, não tempo nem incidentes.
Condição proposta de avanço / quem decide: meta a ser definida pela gestora; decide: a gestora.
Condição proposta de interrupção / quem age: proposta publicada com divergência de R1–R4 ou proporção abaixo da meta; age: a pessoa responsável designada conforme M2.

**6. Fundamentação aplicada.** Integre estes argumentos às seções anteriores ou registre-os aqui com remissão explícita:

- **F1:** afirmação da fonte em minhas palavras e localização: artefatos de engenharia gerados por LLMs podem estar incorretos e ainda assim parecer plausíveis (Fan et al., v4, Seção I, Introdução); decisão do parecer a que se aplica: condição de conferir cada trecho antes de publicar; o que a fonte sustenta: o risco de um texto plausível estar errado; minha inferência sobre o caso: um texto de documentação pode soar correto e, ainda assim, descrever um filtro de estado que R3 não prevê, como ocorreu com a documentação candidata do caso T2; isso é semelhante ao que foi comentado em aula, que a fluência não garante utilidade para a decisão; limite/contraponto: é um levantamento de informações, e não mede taxa de erro em documentação de Fila Clara.
- **F2:** afirmação da fonte em minhas palavras e localização: métricas como acurácia podem não capturar todos os efeitos de um modelo; um modelo pode ter bom resultado médio e falhar em situações específicas (Hou et al., v6, Seção 8.1.3); decisão do parecer a que se aplica: limite da métrica de proporção na Parte 5; o que a fonte sustenta: um resultado geral pode esconder falhas em casos específicos; minha inferência sobre o caso: a proporção de propostas aprovadas sem divergência pode esconder falhas nos casos que o contrato cobre pouco, como o acesso do Laboratório a chamados do Laboratório; limite/contraponto: a fonte trata de avaliação de LLMs em engenharia de software em geral, e não desta métrica nem deste caso.

## Anexo — evidências, referências e procedência

**E1 — origem/atividade, arquivo ou identificação e trecho exato:** registro de AV2, `avaliacoes/av2/registro-av2-gabriel_pedroza.md`, seção 3 e caso T2 da tabela de casos (chamado V-02, departamento Oficina, estado fechado, solicitante Oficina).
Entrada ou fato / esperado ou critério / resultado e método / status observado, inferido ou simulado: entrada V-02, solicitante Oficina, estado fechado; esperado por R3: verdadeiro, independentemente do estado; resultado do candidato: falso; método: inspeção por leitura do código; status: inferido, não executado.
**E2 — origem e trecho ou limitação/contraponto da evidência:** registro de AV2, seção 4: os quatro casos não cobrem o acesso do Laboratório a chamados do Laboratório; o aceite do ajuste é condicionado a essa verificação. Status: inferido por inspeção.
**Outros trechos essenciais de apoio às decisões, se necessários:** nenhum além de E1 e E2.

**F1 — referência de L0:** autores: Angela Fan et al.; título: "Large Language Models for Software Engineering: Survey and Open Problems"; ano/versão: 2023, v4 (revisada em 11/11/2023); seção/página consultada: Seção I, Introdução; referência/link identificável: arxiv.org/abs/2310.03533v4.
**F2 — referência de L0:** autores: Xinyi Hou et al.; título: "Large Language Models for Software Engineering: A Systematic Literature Review"; ano/versão: 2024, v6 (revisada em 10/04/2024); seção/página consultada: Seção 8.1.3; referência/link identificável: arxiv.org/abs/2308.10620v6.

**Procedência:** materiais simulados reaproveitados: caso Fila Clara, registros de AV2 e cartão M1–M6 de AV1.6; observações próprias: a leitura de T2 e de E2 foi feita por mim, sem execução; inferências: as relacionadas a R3 e à documentação candidata; passos e metas propostos: Parte 5, todos propostos e não executados.

**IA:** utilizada. Ferramenta-modelo visível: OpenCode, modelo claude-haiku-5-5; data: 12/10/2026; tarefa/contexto: leitura dos materiais e do enunciado, criação do arquivo a partir do modelo, transcrição dos textos aprovados por mim e sugestões pontuais de redação; trecho aproveitado e verificação própria: textos aprovados por mim antes da transcrição, com ajustes; conferência de cada texto em relação ao enunciado, ao modelo, ao contrato e aos registros de AV1/AV2; os rejeitados não entraram no arquivo. O recorte, as alternativas, a recomendação, as fontes e as conclusões são minhas.

**Checklist:** [x] alternativas; [x] autonomia; [x] evidência/contraponto; [x] dois riscos; [x] maturidade/métrica; [x] duas fontes aplicadas; [x] procedência; [x] 3+2 páginas.
