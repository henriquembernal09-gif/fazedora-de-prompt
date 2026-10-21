# Arquitetura do prompt entregue

Todo prompt que a skill entrega tem estas oito partes, nesta ordem, com estes títulos
(em português, em maiúsculas, para a IA e o médico acharem rápido). Parte que não se
aplica entra com uma linha dizendo por que não se aplica, nunca some em silêncio.

## 1. PERSONALIDADE
Quem a IA é neste trabalho e para quem ela trabalha. Em 3 a 6 linhas: a especialidade,
o jeito de falar, a postura com o paciente ou com o colega. Escrita **na voz do médico**
("Você escreve como eu escrevo: ...").

## 2. ENFOQUE
O objetivo único do prompt e o que é "bom" aqui. Uma frase de objetivo, depois os
critérios de um bom resultado (curto? completo? acolhedor? com número?). Se há mais de
uma tarefa, liste cada uma e diga qual manda quando conflitarem.

## 3. RESTRIÇÕES
O que a IA nunca faz. Duas camadas:

**Travas fixas (entram em todo prompt, sem exceção):**
- Não inventar referência, estudo, autor, ano, número de página ou DOI. Se não tiver
  certeza, dizer "não tenho a fonte, confira antes de usar".
- Não usar nem pedir dado que identifique paciente. Se aparecer um, avisar e não repetir.
- Não decidir conduta clínica: o texto é rascunho para o médico revisar e assinar.
- Dizer quando não sabe, em vez de preencher com algo plausível.
- Não prometer resultado, cura ou prazo.

**Travas do caso:** o que este médico disse que a IA não pode fazer (assunto proibido,
termo que ele não usa, tom que ele evita). Use as palavras dele.

## 4. FLUXO
Os passos que a IA segue, em ordem. Inclui: o que fazer antes de responder (perguntar
se faltar informação? quais?), como organizar a resposta, e o que fazer quando o pedido
sair do escopo. Se há ramos ("se for criança, ...; se for idoso, ..."), escreva-os
explicitamente.

## 5. ESTILO
Como o texto soa. É a parte que mais faz diferença e a que mais falha por ser vaga.
Proibido: "tom profissional e acolhedor". Obrigatório: **comportamentos observáveis**
tirados do texto real do médico.
- Como abre e como fecha.
- Tamanho médio de frase e de parágrafo.
- Vocabulário em **pares "digo / não digo"** (ex.: digo "use", não digo "utilize"; digo
  "pressão alta", não "hipertensão arterial sistêmica"). Pelo menos 3 pares. Sem texto
  real, pergunte: "que palavra você troca por outra para o paciente entender?".
- Trata por "você", "senhor(a)", pelo nome?
- Usa emoji? lista? negrito?
- Inclua **um trecho curto do texto real dele** como modelo ("Escreva neste ritmo:
  ..."), já sem identificadores.

## 6. INSUMOS
O que a IA recebe a cada uso e em que formato, e o que fazer quando faltar. Ex.: "Eu
vou colar a transcrição da consulta, sem nome. Se não vier a idade, pergunte antes."

## 7. TEMPLATES
O formato exato da saída, com os campos e a ordem. Se a saída varia, um template por
tipo. Use marcadores `[ASSIM]` para o que a IA preenche. Se não há formato fixo, diga
"formato livre" e descreva o tamanho esperado.

## 8. OBSERVAÇÕES
Tudo que não coube acima: o que ficou em aberto na entrevista, o que foi assumido, em
que casos o médico quer ser avisado, e uma nota de versão (data e "o que mudou"), para
ele saber o que está usando.

---

## Bloco final: vícios de IA a evitar

Todo prompt entregue termina com um bloco "EVITAR" contendo a lista de
`vicios-de-ia.md` (adaptada ao caso: tire o que o médico usa de verdade).

## Regras de escrita do prompt em si

- **Instrução afirmativa antes de proibição.** "Comece pela resposta" funciona melhor
  do que "não enrole". Proibição só para o que é perigoso ou recorrente.
- **Explique o porquê** das regras importantes em meia frase. A IA obedece melhor ao que
  entende ("Sem sigla, porque o paciente idoso não conhece").
- **Um exemplo vale dez adjetivos.** Prefira um trecho real a "seja claro e humano".
- **Sem contradição.** Releia: se uma regra manda ser breve e outra manda ser completa,
  diga qual vence.
- **Linguagem que o médico entende.** Ele vai ler o prompt e precisa reconhecê-lo como
  dele. Nada de termos em inglês sem necessidade.
- **Tamanho proporcional.** Prompt para tarefa simples cabe em uma página. Passou de
  duas, corte o que a IA já faz bem sem ser mandada.
