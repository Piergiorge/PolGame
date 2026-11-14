# PolGame — jogos de genética e imunologia

Jogos que rodam direto no navegador, no computador ou no celular. Não precisa instalar nada.

### ▶️ [Abrir o menu de jogos](https://piergiorge.github.io/PolGame/)

| Jogo | Gênero | Tema | Link |
|---|---|---|---|
| 🧬 **Fita Molde** | Plataforma | Replicação do DNA, pareamento de bases, mutações e código genético | [▶️ Jogar](https://piergiorge.github.io/PolGame/fita-molde/) |
| 🧱 **GenoBlocos** | Quebra-cabeça de blocos | Pareamento A–T / C–G, agentes mutagênicos, CRISPR e reparo do DNA | [▶️ Jogar](https://piergiorge.github.io/PolGame/genoblocos/) |
| 🦠 **GULP!** | Roguelike | Imunidade inata: fagocitose, patógenos, citocinas e anticorpos | [▶️ Jogar](https://piergiorge.github.io/PolGame/gulp/) |
| 🪐 **Locus Astra** | Criação e cruzamento | Genética mendeliana: Punnett, cruzamento-teste, epistasia, alelo letal, herança ligada ao X e poligênica | [▶️ Jogar](https://piergiorge.github.io/PolGame/locus-astra/) |
| 🩺 **Surto** | RPG investigativo | Heredogramas humanos: modos de herança, consanguinidade, penetrância incompleta, início tardio e fenocópias | [▶️ Jogar](https://piergiorge.github.io/PolGame/surto/) |

Todos os jogos têm efeitos sonoros e música gerados por código (a tecla **M** liga e desliga) e funcionam no celular.

---

# 🧬 Fita Molde

**Um platformer 2D sobre replicação do DNA.** Você é a DNA polimerase: atravesse a célula coletando nucleotídeos complementares para copiar a fita molde, corrija seus erros com a revisão 3'→5' e chegue ao telômero.

### ▶️ [Jogar o Fita Molde](https://piergiorge.github.io/PolGame/fita-molde/)

## Como jogar

No topo da tela aparece a **fita molde** (3'→5'). Colete, na ordem, os nucleotídeos que pareiam com ela para sintetizar a **fita nova** (5'→3'):

- **A** pareia com **T** (2 pontes de hidrogênio)
- **C** pareia com **G** (3 pontes de hidrogênio)

Se você pegar a base errada, ela é incorporada como **mutação**. Use a **revisão** para remover o último nucleotídeo antes de seguir. Com a fita completa, vá até o **telômero** no fim da fase.

### Controles

| Ação | Teclado | Celular |
|---|---|---|
| Mover | `←` `→` ou `A` `D` | ◀ ▶ |
| Pular (segure para ir mais alto) | `Espaço`, `W` ou `↑` | ▲ |
| Revisão 3'→5' (remove o último nucleotídeo) | `E` ou `↓` | Revisar |
| Reiniciar | `R` | — |
| Mostrar hitboxes | `H` | — |

### Elementos do jogo

| | Elemento | O que faz |
|---|---|---|
| 🧬 | **DNA polimerase** (você) | Sintetiza a fita nova. Os nucleotídeos coletados formam uma cauda atrás dela. |
| 🔤 | **Nucleotídeos** (A, T, C, G) | Peças da fita nova. Reaparecem alguns segundos depois de coletados. |
| 🦠 | **Bacteriófago** | Patrulha as plataformas. Pule em cima para eliminá-lo; encostar de lado causa dano. |
| 💥 | **ERO** (espécie reativa de oxigênio) | Flutua em ondas e causa dano oxidativo ao toque. Não dá para pisar nela. |
| ⬡ | **Helicase** | Abre a dupla hélice e libera o pulo duplo. |
| 🚩 | **Checkpoints G1/S e G2/M** | Pontos de controle do ciclo celular que salvam seu progresso. |
| 🧵 | **Telômero** | Fim do cromossomo e da fase. Só aceita a chegada com a fita completa. |

---

## A biologia por trás

A fita molde da fase é:

```
Molde  3'-TAC CGG ACC ATT-5'
Nova   5'-ATG GCC TGG TAA-3'
```

A fita nova tem a mesma sequência do mRNA desse pequeno gene (com U no lugar de T). Ela começa com o códon de início **ATG** e codifica **Met–Ala–Trp**, terminando no códon de parada **TAA**.

Ao chegar no telômero, o jogo traduz a fita que você sintetizou e classifica cada códon alterado:

| Tipo de mutação | O que acontece | Exemplo no jogo |
|---|---|---|
| **Silenciosa** | O códon muda, mas o aminoácido é o mesmo (código degenerado) | GCC → GCA (Ala → Ala) |
| **Troca de sentido** (missense) | Um aminoácido é trocado por outro | GCC → GAC (Ala → Asp) |
| **Sem sentido** (nonsense) | Surge um códon de parada prematuro e a proteína fica truncada | TGG → TAG (Trp → Stop) |
| **Perda do códon de parada** | O stop vira um aminoácido e a tradução continua além do previsto | TAA → CAA (Stop → Gln) |

O jogo também mostra a **fidelidade** da cópia, quantos erros foram incorporados e quantos foram corrigidos pela revisão. Na célula, a atividade exonuclease 3'→5' da polimerase tem esse mesmo papel: remover nucleotídeos mal pareados logo depois de incorporados.

### Sugestões para usar em aula

- Peça que os alunos errem de propósito para produzir cada tipo de mutação e comparem as proteínas resultantes.
- Discuta por que a terceira posição do códon tolera mais mutações silenciosas.
- Relacione a revisão 3'→5' com a taxa de erro da replicação e com o sistema de reparo de mau pareamento.

---

---

# 🧱 GenoBlocos

Cada peça é um nucleotídeo. Complete linhas para eliminá-las e encaixe **bases complementares lado a lado**: cada par vale pontes de hidrogênio extras (A–T = 2, C–G = 3). Quatro linhas de uma vez formam uma **Tétrade**. Use enzimas como power-ups (helicase, CRISPR-Cas9, DNA ligase, telomerase e reparo NER) e sobreviva à radiação UV, à fumaça de cigarro, aos retrovírus e ao raio-X.

### ▶️ [Jogar o GenoBlocos](https://piergiorge.github.io/PolGame/genoblocos/)

---

# 🦠 GULP!

Em grego, *macrófago* quer dizer "grande comedor". Você é um macrófago e atravessa cinco tecidos fagocitando bactérias, vírus e fungos, evolui com mecanismos reais da imunidade inata e enfrenta a superbactéria **MRSA**. Os mapas mudam a cada partida e a morte é permanente.

### ▶️ [Jogar o GULP!](https://piergiorge.github.io/PolGame/gulp/)

---

# 🪐 Locus Astra

Ano 2187. Você é geneticista na estação **Locus Astra** e cuida dos **astrídeos**, criaturas alienígenas cuja herança segue as regras de Mendel. Capture exemplares em planetas com frequências alélicas diferentes, sequencie genomas, preveja os filhotes com quadros de Punnett, cumpra contratos e dispute a arena com criaturas cujos atributos vêm dos genes. O progresso fica salvo no navegador.

| Característica | Mecanismo de herança |
|---|---|
| Cor | Dominância incompleta (vermelho × azul = roxo) e alelos múltiplos (dourado recessivo) |
| Padrão e olhos | Dominância completa (liso e ciclope são recessivos) |
| Cristais | Alelo letal em homozigose (KK não eclode: proporção 2:1) |
| Albinismo | Epistasia recessiva (cc esconde o gene da cor) |
| Elemento | Alelos múltiplos e codominância, como no sistema ABO |
| Tamanho | Herança poligênica (2 genes aditivos, 5 classes) |
| Bioluminescência | Ligada ao X e recessiva (portadoras não brilham) |

O genótipo aparece com **?** onde ainda é desconhecido: dá para **sequenciar** (custa pesquisa) ou **deduzir por cruzamento-teste**, e o laboratório faz as deduções automaticamente a partir dos filhotes.

### ▶️ [Jogar o Locus Astra](https://piergiorge.github.io/PolGame/locus-astra/)

---

# 🩺 Surto

Você acaba de assumir o Serviço de Genética do **Vale do Sereno**, uma região onde famílias inteiras adoecem sem explicação. Cada caso é uma família: clique nas pessoas do heredograma para **entrevistar** os vivos, **consultar prontuários** dos falecidos e **sequenciar** amostras, sempre contra o relógio (as horas de investigação são limitadas). A Dra. Helena, que está se aposentando, ajuda a avaliar as hipóteses. No fim, você assina um **laudo** com o modo de herança e responde a uma pergunta de aconselhamento genético.

| Caso | O que ensina |
|---|---|
| 1. Família Siqueira | Autossômica recessiva (pais portadores, risco de 1/4) |
| 2. Família Lacerda | Autossômica dominante (transmissão pai → filho) |
| 3. Família Tavares | Recessiva ligada ao X (mães portadoras) |
| 4. Família Nogueira | Consanguinidade (primos compartilham 1/8 dos genes) |
| 5. Família Coutinho | Dominante ligada ao X (pai afetado → todas as filhas) |
| 6. Família Esteves | Herança mitocondrial (só pela mãe) |
| 7. Família Rezende | Início tardio e teste preditivo |
| 8. Família Barros | Penetrância incompleta |
| 9. Família Duarte | Fenocópia ambiental (não é genética!) |

As famílias são geradas aleatoriamente a cada partida, sempre com um heredograma que permite chegar à resposta. As doenças têm nomes fictícios, e o laudo revela o equivalente real (albinismo, Marfan, hemofilia A, fenilcetonúria, raquitismo hipofosfatêmico, MELAS, Huntington, polidactilia e intoxicação por chumbo). Depois da campanha, os **plantões** trazem famílias aleatórias com todos os modos de herança possíveis. Você sobe de nível e escolhe habilidades (mais horas, sequenciamento mais barato, consultas extras…).

### ▶️ [Jogar o Surto](https://piergiorge.github.io/PolGame/surto/)

---

## Detalhes técnicos

Cada jogo é um único arquivo HTML com JavaScript puro, sem bibliotecas nem dependências externas. Os sons e a música são gerados por código (Web Audio API). Os gráficos do Locus Astra são SVG gerados a partir do fenótipo de cada criatura.

```
index.html             menu com os jogos
fita-molde/index.html
genoblocos/index.html
gulp/index.html
locus-astra/index.html
surto/index.html
```

No Fita Molde:
- Renderização em `<canvas>` com física em passo fixo (120 Hz), o que mantém o pulo igual em qualquer taxa de quadros.
- Pulo com tempo de tolerância na borda (*coyote time*), buffer de pulo e altura variável.
- Inimigos com detecção de bordas e paredes para patrulhar sem cair das plataformas.

Para jogar sem internet, baixe o `index.html` do jogo e abra no navegador.

## Próximas fases do Fita Molde (ideias)

- Fita descontínua: fragmentos de Okazaki, primase e DNA ligase
- Transcrição: RNA polimerase, uracila no lugar de timina
- Tradução: ribossomo, tRNAs e anticódons

## Licença

Veja o arquivo [LICENSE](LICENSE).

## Autor

Rafael Piergiorge ([@Piergiorge](https://github.com/Piergiorge))
