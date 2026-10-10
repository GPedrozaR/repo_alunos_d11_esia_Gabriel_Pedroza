# Contexto do pacote Fila Clara

- Disciplina D1.1, 24h; caso didático fictício, sem aplicação real a implantar.
- Runtime de referência: Python 3.13.3, somente biblioteca padrão.
- `caso/`: contrato, funções pequenas e dados sintéticos; `testes/`: unittest; `apoio/`: materiais textuais; `exercicios/aula-1/` a `aula-6/`: registros.
- Comando na raiz desta pasta: `python -B testes/test_fila_clara.py --codigo caso/fila_clara.py`.
- Há nove verificações do material: na versão inicial, seis passam e três falham. Código de saída `1` indica falhas e `0` indica sucesso no conjunto executado. Os testes não atribuem nota ao aluno.
- O argumento `--codigo caminho.py` seleciona a implementação; `--teste TestFilaClara.nome_do_teste` seleciona uma verificação. Resultados textuais observados ficam em `apoio/resultado-textual.md`.
- Leia `caso/regras.md`: entradas válidas controladas, sem ampliar o escopo para validação externa ou implementação de autenticação.
- Conferir qualquer proposta com o contrato do caso e registrar assistência, evidência, decisão e limite.
- Nos modelos de resposta (`template-registro.md`), não alterar perguntas, rótulos nem enunciados; preencher somente os espaços em branco, mantendo o texto do rótulo exatamente como está no modelo.
- Regra: não inventar, supor ou imaginar contratos, papéis, responsabilidades, processos, dados ou informações que não estejam descritos no projeto. Quando algo faltar, dizer que não está descrito e não preencher com suposições. Exemplos de dados fictícios são permitidos somente quando seguem os campos e valores descritos no caso.
