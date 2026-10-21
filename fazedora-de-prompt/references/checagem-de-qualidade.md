# Checagem de qualidade (interna)

Antes de mostrar o prompt, dê nota de 0 a 10 em cada um dos 11 critérios. Só entregue se **todos**
estiverem em 9 ou mais (exceto por falta de informação dele, ver "Honestidade na entrega"). Se algum for menor, conserte e confira de novo. Não mostre esta
lista ao médico, a menos que ele peça; mostre, se pedir, a nota e o que foi consertado.

| # | Critério | Nota 10 quando... |
|---|---|---|
| 1 | **Escopo fechado** | Uma pessoa estranha lê e sabe exatamente o que a IA faz e o que não faz. Nada de "ajude com o que for preciso". |
| 2 | **Cobre as oito partes** | Personalidade, enfoque, restrições, fluxo, estilo, insumos, templates e observações presentes. Parte não aplicável explica por quê. |
| 3 | **Estilo observável** | O estilo descreve comportamentos (como abre, tamanho da frase, palavras) e tem trecho real do médico. Nenhum "tom acolhedor e profissional" solto. |
| 4 | **Voz do médico** | O prompt está escrito na linguagem dele. Ele leria e diria "isso sou eu". |
| 5 | **Travas fixas presentes** | Não inventar referência nem fato que muda ([CONFERIR]), dizer quando não sabe, não prometer, rascunho para revisar. Se o assunto é saúde: também não usar dado de paciente nem decidir conduta. |
| 6 | **Vícios de IA** | Bloco "EVITAR" adaptado ao caso, sem itens que o médico usa de verdade. |
| 7 | **Sem contradição nem excesso** | Nenhuma regra briga com outra. Nada repetido. Cabe em uma ou duas páginas. |
| 8 | **Insumos e lacunas** | Diz o que a IA recebe e o que faz quando falta. |
| 9 | **Saída definida** | Formato, tamanho e campos claros. |
| 10 | **Ângulos cobertos e confirmados** | Os 3 ângulos centrais de `angulos.md` foram perguntados (e os extras que o caso pedia), pelo menos uma resposta mudou uma regra do prompt, e a pessoa confirmou o resumo antes da entrega. |
| 11 | **Testado** | Rodou em caso fictício, o médico viu o resultado e os ajustes dele entraram no prompt. |

## Sinais de que ainda não está 9,5

- A palavra "adequado", "apropriado" ou "de forma clara" aparece sem exemplo.
- O estilo ficou igual ao de qualquer médico (troque o nome e continua servindo).
- Nenhuma pergunta da entrevista rendeu uma regra que o médico não esperava.
- O teste foi aprovado de primeira, sem ajuste, mas o médico não leu com calma.
- Há instrução que a IA já cumpriria sozinha ("seja educado").
- Faltou dizer o que fazer na exceção (paciente em risco, pedido fora de escopo).

## Honestidade na entrega

Se um critério ficou abaixo de 9 por falta de informação do médico (ex.: sem texto real
para o estilo), **entregue assim mesmo** e diga qual critério ficou fraco e o que ele
pode trazer para subir a nota. Nunca disfarce lacuna com texto bonito.
