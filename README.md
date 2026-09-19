# O Conselho

Uma skill para o Claude que leva uma decisão difícil a um conselho de seis personalidades, uma para cada área de uma empresa. Cada conselheiro olha a decisão só pelo ângulo dele. Depois eles revisam uns aos outros, e um Presidente do Conselho fecha com um veredito, um placar de votos e **a única coisa pra fazer primeiro**.

Nasceu como o conselho de gestão da Império Desentupidora e Dedetizadora (Grande São Paulo). Esta é a versão aberta, pra qualquer empresa ou decisão pessoal.

## Quem senta à mesa

| Conselheiro | Área | A pergunta dele |
|---|---|---|
| Warren Buffett | Financeiro e compras | Isso fica de pé daqui a 10 anos? Vale o que custa? E se der errado, você sobrevive? |
| W. Edwards Deming | Qualidade | Isso sai bem feito toda vez, ou só quando dá sorte? |
| Neil Rackham | Vendas | Quem compra isso, por que compraria, e como essa venda avança? |
| Washington Olivetto | Criatividade e marca | O que o cliente vê, sente e conta pro vizinho? |
| Márcio Fernandes | Pessoas | Quem vai fazer isso acontecer, e vai querer? |
| Andy Grove | Operação | O que sai daqui segunda de manhã, e como a gente mede? |

O Buffett também faz o papel do cético da mesa: se ninguém procurar o furo, ele procura.

## Como usar

Depois de instalada, é só conversar com o Claude:

- **Conselho completo:** "leva pro conselho: abro uma segunda loja ou invisto em delivery?"
- **Um conselheiro só:** "pergunta pro Deming…", "o que vendas acha?", "chama o Olivetto pra pensar a fachada".

A sessão completa segue sempre a mesma ordem:

1. A pergunta reescrita de forma neutra.
2. As seis vozes.
3. A revisão entre os conselheiros.
4. O veredito: placar, onde concordam, onde brigam, a recomendação e o primeiro passo.

## Como instalar

**No claude.ai:** baixe o arquivo `o-conselho.skill` em [Releases](../../releases) e vá em **Configurações → Habilidades → Adicionar → Fazer upload de habilidade**.

**No Claude Code:** copie a pasta `o-conselho/` para `~/.claude/skills/`.

## Deixar com a cara da sua empresa

O conselho fica muito melhor quando conhece o seu negócio. No `SKILL.md` há um bloco **"Contexto da empresa"** pra preencher:

```
Empresa:            [nome, cidade ou região, tempo de mercado, o que vende]
Cliente:            [quem compra e quem DECIDE a compra]
Valores:            [os valores que a empresa leva a sério]
Tom de voz:         [como a empresa fala com o cliente]
Marca:              [cores, fontes, elementos visuais]
Operação:           [como o produto ou serviço chega ao cliente]
```

Sem esse bloco preenchido, o conselho usa o que você contar na conversa. Se faltar o essencial, ele faz uma pergunta antes de começar.

Dá pra trocar uma personalidade também. A regra que mantém o método de pé é uma pessoa por área e no máximo seis na mesa.

## Sobre as personalidades

Cada conselheiro é uma leitura dos **princípios públicos** de uma personalidade real, aplicados à sua decisão. Não é a pessoa, e ela não tem nenhuma relação com este projeto nem o endossa. A skill proíbe inventar citações: só vão entre aspas frases que a pessoa reconhecidamente disse.

## Créditos

- Método **LLM Council**, de [Andrej Karpathy](https://github.com/karpathy).
- Skill **5 Conselheiros**, de Tedson Santos ([@tedsonsantos_](https://instagram.com/tedsonsantos_)), licença MIT. É a versão em português que deu origem a esta.
- Adaptação e personalidades: Luiz Henrique Alves ([@luizalves.me](https://instagram.com/luizalves.me)).

Licença MIT. Veja [LICENSE](LICENSE).
