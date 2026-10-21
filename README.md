# Fazedora de Prompt

**Fale 2 minutos do seu jeito. A IA faz as perguntas que faltam, uma por vez, e entrega
um prompt pronto, com a sua cara e não com cara de IA.**

Uma skill gratuita para médicos, criada pela [Monet Health](https://www.instagram.com/monet.health).

## Como funciona

1. **Você fala.** Liga o microfone (ou dita) e conta o que quer que a IA faça. Pode ser
   bagunçado.
2. **Ela pergunta.** Uma pergunta por mensagem, em linguagem de consultório, sem
   repetir o que você já contou. São de 10 a 30 perguntas, conforme o tamanho do que
   você pediu. Ela para quando já entendeu tudo.
3. **Você recebe o prompt pronto**, em bloco, para copiar. Vem com oito partes:
   personalidade, enfoque, restrições, fluxo, estilo, insumos, templates e observações.
4. **Ela testa** o prompt num caso fictício e ajusta até soar como você.

Para o texto ficar com a sua cara, ela pede pelo menos uma mensagem ou orientação real
sua (sem nome de paciente) e copia o estilo dali.

## Instalação (3 passos, no Claude gratuito)

1. **Baixe o arquivo** [`fazedora-de-prompt.zip`](fazedora-de-prompt.zip) (botão
   "Download" na página do arquivo).
2. No Claude, vá em **Configurações → Capacidades** e ligue **Execução de código e
   criação de arquivos**.
3. Ainda em Configurações, abra **Skills**, clique em **Enviar skill** e escolha o
   `.zip`. Pronto.

Para usar, abra uma conversa nova e escreva: **"Quero fazer um prompt"**.

> Os nomes dos menus podem mudar de lugar com o tempo. Se não achar, procure por
> "Skills" nas configurações do Claude ou na Central de Ajuda da Anthropic.

## Exemplos do que dá para pedir

- Orientações de pós-consulta no seu jeito de falar com o paciente
- Respostas padrão de WhatsApp para a secretária
- Resumo de artigo com os pontos que importam para você
- Roteiro de aula, post ou legenda sem soar como robô
- Estrutura de relatório ou parecer

## Cuidados que a skill já toma por você

- **Não pede nem aceita dado de paciente.** Se você colar um nome por engano, ela avisa e
  segue sem ele.
- **O prompt entregue proíbe inventar referência bibliográfica.** IA inventa citação
  com cara de verdade; o prompt já vem com a trava.
- **Não decide conduta.** O prompt gera rascunho para você revisar e assinar.

Mesmo assim: **você é responsável pelo que a IA escrever em seu nome.** Leia antes de enviar.
Não coloque dados identificáveis de pacientes em nenhuma ferramenta de IA sem
entender a política de privacidade dela e a LGPD.

## O que tem aqui

```
fazedora-de-prompt/
├── SKILL.md                         ← o método (a entrevista, passo a passo)
└── references/
    ├── arquitetura-do-prompt.md     ← as oito partes do prompt entregue
    ├── banco-de-perguntas.md        ← cardápio de perguntas de consultório
    ├── vicios-de-ia.md              ← o que a IA faz que denuncia o texto
    ├── checagem-de-qualidade.md     ← a régua interna antes de entregar
    └── exemplo-completo.md          ← um prompt entregue, caso fictício
```

Tudo em texto simples. Pode abrir e ler. Se quiser mudar algo, é só editar o `SKILL.md`.

## Sobre a Monet Health

A Monet Health é uma empresa para médicos. Siga
[@monet.health](https://www.instagram.com/monet.health) no Instagram para mais materiais
como este.

## Licença

[MIT](LICENSE): use, copie e adapte à vontade.
