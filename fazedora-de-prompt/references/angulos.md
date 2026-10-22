# Ângulos da entrevista (o "grill")

O relato e as perguntas básicas cobrem o que a pessoa já sabe que quer. Os ângulos cobrem
o que ela **não pensou**, e é aqui que o prompt deixa de ser bom e passa a funcionar de
primeira. Cada ângulo vira **uma** pergunta, com a sua sugestão de resposta, como as
outras. Nunca despeje vários de uma vez. Para encurtar, **junte o ângulo com a pergunta
que ia fazer de qualquer jeito** (ainda uma pergunta só), em vez de acrescentar.

## Como os ângulos entram

As **5 perguntas iniciais** do `SKILL.md` já carregam os três ângulos centrais: **pré-mortem**
(pergunta 2), **decisão que sobra para a IA** (3) e **restrição escondida / recurso
escondido** (4). Não repita. Os ângulos abaixo, **4 a 6**, são extras: entram só quando
o caso pedir (resultado "correto mas ruim" quando o estilo é crítico; caso estranho em
saúde, dinheiro ou prazo que não volta; "bom o bastante" em uso recorrente).

| # | Ângulo | Pergunta-modelo | Por que importa |
|---|---|---|---|
| 1 | **Pré-mortem** | "Imagina que daqui a um mês você abre o resultado e odeia. O que aconteceu? (Meu palpite: ...)" | Revela o pior defeito antes dele existir. |
| 2 | **Decisão que sobra para a IA** | "Qual decisão você ainda não tomou e a IA vai ter que tomar por você? (Ex.: ...)" | Tudo que a pessoa não decide, a IA chuta. |
| 3 | **Restrição escondida** | "Tem alguma regra que você segue sem perceber e não me contou? Tempo, dinheiro, gosto, política do lugar..." | Preferências óbvias para a pessoa e invisíveis para a IA. |
| 4 | **Resultado ruim, mas correto** | "Como seria um resultado tecnicamente certo que você mesmo jogaria fora?" | Pega o genérico, o longo demais, o formal demais. |
| 5 | **Caso estranho** | "Qual o caso mais raro ou esquisito que isso pode enfrentar? O que você quer que aconteça nele?" | Define o comportamento fora do comum. |
| 6 | **Critério de "bom o bastante"** | "Quando você olha o resultado, o que te faz dizer 'tá ótimo, mando assim'?" | Vira o critério de qualidade do prompt. |
| 7 | **Recursos escondidos** | "O que você tem que a IA não enxerga? Milhas, cupom, cartão, contato, conta antiga, material seu. (Meu palpite: ...)" | O que ele esqueceu de contar porque é um ativo, não um problema. |

## Ângulos extras (use os que o caso pedir)

- **Tentativa anterior:** "O que você já tentou? O que não deu certo?"
- **Quem mais é afetado:** "Alguém além de você vai ler, usar ou sofrer com isso?"
- **Fonte da verdade:** "De onde vêm os fatos? A IA pode buscar sozinha ou só usa o que você manda?"
- **Corte:** "Se tivesse que tirar metade, o que sai?"
- **Frequência:** "Isso é uma vez só ou todo dia? Se for todo dia, vale investir mais."
- **Reversão:** "O que acontece se a IA errar? É fácil desfazer?"
- **O contrário:** "Quando você NÃO quer que a IA faça isso? Em que situação ela deveria recusar ou perguntar?"

## Como descer na árvore de decisões

O que o grill-me faz de melhor é **ordenar** as decisões: não adianta perguntar tom antes de
saber para quem. Siga esta ordem de dependência:

1. **Objetivo e para quem** → tudo depende disso.
2. **Restrições duras** (o que nunca, o que obrigatório, prazo, dinheiro, regra do lugar).
3. **Fatos e fontes** (o que a IA recebe, de onde vêm os dados).
4. **Fluxo** (passos, ramos, o que fazer quando faltar informação).
5. **Estilo e formato** (só agora, já sabendo objetivo e público).
6. **Ângulos extras**, em qualquer ponto depois das 5 perguntas iniciais.

Duas regras:
- **Resposta que abre ramo nova:** se uma resposta revelar uma decisão que ele não tinha
  tomado, **desça nela** antes de seguir ("Antes de continuar: você disse que depende do
  paciente. Depende de quê?"). Só depois volte à lista.
- **Decisão dependente:** não faça a pergunta B se a resposta de A pode torná-la inútil.

## Como fazer a pergunta de ângulo soar natural

Em vez do nome do ângulo, use a vida dele. Não diga "vamos fazer um pré-mortem". Diga:
"Imagina que a IA te entregou isso e você ficou chateada. Qual foi o erro?".

## Portão de confirmação (antes de entregar)

Os ângulos terminam em **entendimento compartilhado**, não em prompt. Antes de gerar,
escreva um resumo em 3 a 6 linhas, em linguagem dele:

> Entendi assim: [objetivo]. Para [público]. Do seu jeito: [3 traços do estilo]. A IA
> nunca: [2 proibições]. Se acontecer [caso estranho], [o que fazer]. Está certo?

Só gere o prompt depois de um "sim" ou de uma correção que você incorporou. Se ele está
cansado, o resumo é de uma linha e a confirmação vale por "pode fazer".
