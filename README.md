# Vale do Sereno: jogos de genética e biologia

Jogos de genética, imunologia e biologia que rodam direto no navegador, no computador ou no celular. Não precisa instalar nada.

Todos se passam no mesmo lugar: o **Vale do Sereno**, uma cidade fictícia fundada por descendentes de um punhado de colonos. Por isso algumas doenças hereditárias são muito mais comuns ali, e cada família tem uma lenda para explicá-las. Os jogos sobem e descem essa escada: a população que chegou à ilha, as famílias, as pessoas, as células e as moléculas de quem vive no vale.

### ▶️ [Abrir o mapa do Vale do Sereno](https://piergiorge.github.io/Vale-do-Sereno/)

> Este projeto se chamava **PolGame**. O endereço antigo (`piergiorge.github.io/PolGame`) não funciona mais: use o link acima.

| Jogo | Gênero | Tema | Link |
|---|---|---|---|
| 🧬 **Fita Molde** | Plataforma | Replicação do DNA, pareamento de bases, mutações e código genético | [▶️ Jogar](https://piergiorge.github.io/Vale-do-Sereno/fita-molde/) |
| 🧱 **GenoBlocos** | Quebra-cabeça de blocos | Pareamento A–T / C–G, agentes mutagênicos, CRISPR e reparo do DNA | [▶️ Jogar](https://piergiorge.github.io/Vale-do-Sereno/genoblocos/) |
| 🦠 **GULP!** | Sobrevivência | Imunidade inata e o início da adaptativa: fagocitose, opsonização, complemento, interferon, linfócitos T, febre e resistência | [▶️ Jogar](https://piergiorge.github.io/Vale-do-Sereno/gulp/) |
| 🪐 **Locus Astra** | Criação e cruzamento | Genética mendeliana: Punnett, cruzamento-teste, epistasia, alelo letal, herança ligada ao X e poligênica | [▶️ Jogar](https://piergiorge.github.io/Vale-do-Sereno/locus-astra/) |
| 🩺 **Surto** | RPG investigativo | Heredogramas humanos: modos de herança, consanguinidade, penetrância incompleta, início tardio e fenocópias | [▶️ Jogar](https://piergiorge.github.io/Vale-do-Sereno/surto/) |
| 🌳 **Linhagem** | RPG de gerações | Herança poligênica, endogamia, vantagem do heterozigoto, herança ligada ao X e história da genética | [▶️ Jogar](https://piergiorge.github.io/Vale-do-Sereno/linhagem/) |
| 🎡 **Herança** | Jogo de tabuleiro (1 a 4 jogadores) | Genética humana: ABO e Rh, lactase, daltonismo, ACTN3, portadores, vantagem do heterozigoto, teste do pezinho | [▶️ Jogar](https://piergiorge.github.io/Vale-do-Sereno/heranca/) |
| 🦠 **Operon** | Simulação em tempo real | Regulação gênica em bactérias: óperons lac e trp, repressor, indutor, CAP-AMPc, diauxia, atenuação e diagnóstico de mutantes (IPTG, merodiploides F′) | [▶️ Jogar](https://piergiorge.github.io/Vale-do-Sereno/operon/) |
| 🏝️ **Fundadores** | Estratégia por turnos (anos) | Genética de populações: efeito fundador, gargalo, deriva, endogamia, fluxo gênico, seleção balanceadora | [▶️ Jogar](https://piergiorge.github.io/Vale-do-Sereno/fundadores/) |
| 🖥️ **Laudo** | Investigação (tela de computador de 8 bits) | Genética forense: STR, DNA degradado, misturas, Y-STR, mtDNA, paternidade, espécie por DNA, toxicologia e entomologia | [▶️ Jogar](https://piergiorge.github.io/Vale-do-Sereno/Laudo/) |
| 🗼 **Torre 3** | Vigilância em tempo real (uma tela, câmeras e rádio) | Ecologia e saúde: incêndio x neblina, fauna ferida ou saudável, caça e garimpo, febre amarela em bugios, lendas e suas explicações | [▶️ Jogar](https://piergiorge.github.io/Vale-do-Sereno/torre-3/) |

Todos os jogos têm efeitos sonoros e música gerados por código (a tecla **M** ou o botão de som liga e desliga) e funcionam no celular.

### O mapa

O menu é um mapa ilustrado do vale ao anoitecer. Cada jogo é um lugar:

| Lugar | Jogo |
|---|---|
| Ilha da Bruma | Fundadores |
| Casarão da família | Linhagem |
| Bairro Sereno | Surto |
| Feira de domingo | Herança |
| Hospital Regional | GULP! |
| Rio Sereno | Operon |
| Universidade do Sereno | Fita Molde e GenoBlocos |
| Instituto de Criminalística | Laudo |
| Torre de vigia, na encosta da Serra da Bruma | Torre 3 |
| A estrela de Kepler-Rubra | Locus Astra |

---

# 🧬 Fita Molde

**Um platformer 2D sobre replicação do DNA.** Você é a DNA polimerase: atravesse a célula coletando nucleotídeos complementares para copiar a fita molde, corrija seus erros com a revisão 3'→5' e chegue ao telômero.

### ▶️ [Jogar o Fita Molde](https://piergiorge.github.io/Vale-do-Sereno/fita-molde/)

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

### ▶️ [Jogar o GenoBlocos](https://piergiorge.github.io/Vale-do-Sereno/genoblocos/)

---

# 🦠 GULP!

Em grego, *macrófago* quer dizer "grande comedor". Você é um macrófago cercado por ondas de patógenos, num jogo de sobrevivência no estilo *Vampire Survivors*: você só se move (teclado ou toque) e as defesas disparam sozinhas. Os patógenos derrotados deixam **antígenos**; a cada nível, você escolhe um mecanismo novo ou melhora um que já tem (até o nível 5).

| Fase | Patógenos | O que ensina |
|---|---|---|
| Ferida na pele | Staphylococcus, E. coli; chefe: colônia de *S. aureus* | Inflamação; lisozima contra Gram-positivas |
| Corrente sanguínea | Gram-negativas, pneumococo; chefe: tempestade de LPS | Endotoxina e sepse; cápsula e **opsonização** |
| Pulmão | Influenza, células infectadas, tuberculose | **Interferon** e linfócitos **T CD8**; macrófagos precisam de **IFN-γ** contra a tuberculose |
| Linfonodo | Tudo junto; chefe: superbactéria | **Resistência** como seleção natural: ela fica imune ao mecanismo que mais a fere |
| Intestino | Candida, biofilmes; chefe final: uma **tênia** gigante que ocupa quase a tela toda | Microbiota como defesa; helmintos são grandes demais para fagocitar, e o corpo responde com **Th2**, **IgE** e **eosinófilos** |

Armas: fagocitose, explosão respiratória, lisozima, complemento (MAC), neutrófilos (com NETs), anticorpos IgG, interferon, linfócitos T CD8, febre e, na fase final, eosinófilos. Passivas: receptores Toll-like, lisossomos, receptor de manose, integrinas, glicólise, ativação por IFN-γ e apresentação de antígeno (MHC II). No fim de cada partida, um gráfico mostra quanto cada mecanismo contribuiu, e os pontos de **memória imunológica** compram melhorias permanentes (inclusive uma "vacina" que revive uma vez). Uma Imunopédia registra os patógenos encontrados.

### ▶️ [Jogar o GULP!](https://piergiorge.github.io/Vale-do-Sereno/gulp/)

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

### ▶️ [Jogar o Locus Astra](https://piergiorge.github.io/Vale-do-Sereno/locus-astra/)

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

### ▶️ [Jogar o Surto](https://piergiorge.github.io/Vale-do-Sereno/surto/)

---

# 🌳 Linhagem

**Um RPG de gerações.** Você guia a família de um fundador ruivo do Vale do Sereno por **nove gerações**, de 1780 até o século XXI. Em cada geração, o herdeiro vive um evento na infância, realiza dois feitos (a chance depende de Força, Mente e Vista), escolhe com quem casar, vive um evento na vida adulta e decide qual filho herda a casa. Os filhos herdam metade dos alelos de cada genitor, sorteados.

| No jogo | O que ensina |
|---|---|
| Força e Mente (3 genes cada) | Herança poligênica e regressão à média |
| Cabelo ruivo | Herança recessiva: o traço "pula" gerações |
| Olhar de águia | Herança dominante |
| Daltonismo | Herança ligada ao X |
| Casar com primos | Endogamia: o jogo calcula o coeficiente F e doenças recessivas escondidas do fundador reaparecem |
| Febre do pântano | Vantagem do heterozigoto (alelo S e malária) |
| Treinar e educar o herdeiro | O ambiente muda o fenótipo, mas não se herda (contra Lamarck) |
| Eventos de infância e vida adulta | Febre (traço falciforme), pitangas e exame de maquinista (daltonismo), vacina, guerra, gripe espanhola, doação de sangue e teste de ancestralidade |
| Eras históricas | Mendel (1866), Hardy-Weinberg (1908), DNA (1953), testes de portador (anos 1980) e genoma (2003) liberam ferramentas novas |

A árvore da família é um heredograma de verdade, colorido pela característica escolhida, com portadores obrigatórios marcados e casais aparentados em linha dupla. Cada partida sorteia três ambições para a casa.

### ▶️ [Jogar o Linhagem](https://piergiorge.github.io/Vale-do-Sereno/linhagem/)

---

# 🎡 Herança

**Uma vida inteira num tabuleiro de roleta e carrinho.** Até 4 jogadores no mesmo computador (pessoas ou computador) percorrem as etapas da vida: infância (teste do pezinho, vacinas, escola e esporte), adolescência (ENEM, pressão dos amigos), juventude (🪖 serviço militar, 🎓 faculdade ou 💼 trabalho direto), vida adulta (casamento, filhos, casa, pós-graduação), 🏛️ serviço público ou 🏢 iniciativa privada, meia-idade, aposentadoria aos 65 e velhice até os 90.

Cada jogador escolhe seu peão (carro, pipeta, DNA, célula, ervilha de Mendel, drosófila ou cromossomo). O tabuleiro tem 134 casas grandes em serpentina, com a idade marcada em cada uma, e há um modo de **partida rápida** (+3 casas por jogada) para caber numa aula.

Cada jogador recebe **6 cartas viradas para baixo**: genes (traço falciforme, falso O/Bombay, APOE ε4, hipercolesterolemia familiar, FOXO3…), riscos poligênicos (diabetes, hipertensão), hábitos (sedentarismo, tabagismo, álcool, dieta) e crenças (negacionismo). Elas só se revelam com o laboratório, check-ups, exames do quartel, doação de sangue e as surpresas da vida.

| No jogo | O que ensina |
|---|---|
| Casas de saúde 🫀 | Doenças multifatoriais: risco = base + genes + hábitos (diabetes, hipertensão, infarto, câncer de pulmão, fígado, Alzheimer) |
| Check-up | Hábitos se mudam (com recaídas); genes não, mas saber o genótipo muda o desfecho |
| Hemocentro e REDOME | ABO, Rh, fenótipo Bombay e cadastro de doadores de medula |
| Transplantes 🫘 | Compatibilidade ABO e HLA: irmãos têm 25% de chance de ser idênticos; gêmeos idênticos sempre são |
| Bebês e gêmeos | Cada filho herda um alelo de cada genitor; gêmeos idênticos × fraternos; incompatibilidade Rh |
| 80 anos e legado 🏆 | Início tardio (Alzheimer e APOE) e longevidade: a idade final soma genes, hábitos e doenças |
| Eventos globais 🌍 | Pandemias, desinformação, mar subindo, chuvas, calor, secas e crises alagam casas do tabuleiro, mudam salários e preços |
| Carreira, setor e investimentos | Estabilidade × salário, previdência e juros compostos |

Vence quem chegar ao fim com o maior legado: dinheiro + casa + investimentos + filhos + anos vividos acima da média + doações − dívidas com juros. No fim, todas as cartas e genótipos da família são revelados.

### ▶️ [Jogar o Herança](https://piergiorge.github.io/Vale-do-Sereno/heranca/)

---

# 🦠 Operon

**Seja uma *Escherichia coli* no intestino.** Nade (clique, toque ou WASD) atrás de nuvens de glicose, lactose e triptofano, cresça e se divida mais rápido que as cepas rivais. Tudo custa ATP, principalmente transcrever e traduzir genes. Por isso, ligar o gene certo na hora certa faz a diferença.

O painel mostra os óperons por dentro, em tempo real: RNA polimerase, repressores LacI e TrpR, CAP-AMPc, alolactose, mRNA e o grampo do atenuador.

| Fase | O que ensina |
|---|---|
| 1. Primeira refeição | Energia, crescimento e fissão binária |
| 2. Liga e desliga | Óperon lac no controle manual: custo e atraso da expressão gênica |
| 3. O repressor | Controle negativo induzível: LacI, operador, alolactose, expressão basal |
| 4. Glicose primeiro | Controle positivo por CAP-AMPc, repressão catabólica, exclusão do indutor e diauxia |
| 5. Triptofano | Vias biossintéticas: importar ou fabricar |
| 6. Repressão e atenuação | Óperon trp reprimível (Trp como correpressor) e atenuação (grampos 2:3 e 3:4) |
| 7. Intestino | Tudo junto, com refeições, jejum e mutações |
| Desafio livre | Recorde de divisões em 4 minutos |

Quando surge uma **mutação** (lacI⁻, lacOᶜ, lacIˢ, lacZ⁻, lacY⁻, crp⁻, cya⁻, trpR⁻, trpL∆, trpE⁻), você abre o laboratório e faz os testes clássicos de Jacob e Monod: indução com lactose ou IPTG, merodiploide F′ lac⁺ (teste cis-trans), adição de AMPc, crescimento com e sem Trp. Cada palpite errado mostra qual teste contradiz a hipótese. Os conceitos ficam guardados num caderno, e o progresso é salvo no navegador.

### ▶️ [Jogar o Operon](https://piergiorge.github.io/Vale-do-Sereno/operon/)

---

# 🏝️ Fundadores

**Uma colônia que começa com uma amostra pequena de um continente enorme.** Em 1790, você escolhe o navio (bote, escuna ou galeão) e a tripulação, vendo só o que aparece por fora. Ninguém sabe quem é portador de alelos recessivos. Durante 150 anos (umas seis gerações), você explora a ilha hexagonal, divide o trabalho entre comida, madeira, ervas e exploração, e define as leis de casamento e o tamanho das famílias. São 15 construções em cinco grupos (comida, materiais, moradia, saúde e sociedade): roça, pesqueiro, pomar, celeiro, serraria, casas, horta de ervas, boticário, poço, enfermaria, drenagem, abrigo na rocha, registro de famílias, escola (com língua de sinais) e cais (mais migrantes, comércio e mais epidemias). Uma tabela de postos de trabalho mostra quem trabalha onde e quanto cada lugar produz. Como o espaço da ilha é limitado, quase todas as construções podem ser melhoradas até o nível 3 (por exemplo, roça → roça com arado → roça irrigada; registro de famílias → livro de genealogias, que permite proibir casamento até entre primos de 2º grau). O nível 3 exige a escola.

Cada colono é simulado individualmente: casa, tem filhos com genes sorteados dos pais (Mendel), adoece e morre. Epidemias, secas, um clima mais frio, a chegada da malária, navios de migrantes, jovens que emigram e um tufão mudam a população e os genes.

| Mecânica | O que ensina |
|---|---|
| Desembarque | **Efeito fundador**: a tabela compara as frequências dos colonos com as do continente; alelos que nem vieram |
| Gráficos ano a ano | **Deriva genética**, perda e fixação de alelos, queda da diversidade em 8 marcadores neutros (tipo STR) |
| Tufão | **Gargalo** (Pingelap e a acromatopsia) |
| Genealogias e coeficiente F | **Endogamia**: coancestria calculada pelo pedigree real de cada pessoa |
| Doenças recessivas (fibrose cística, anemia falciforme, Ellis-van Creveld, Tay-Sachs, surdez GJB2, acromatopsia) | Portadores escondidos, risco de 1/4, exemplos reais (Amish, Martha's Vineyard, Tristão da Cunha) |
| Malária nos pântanos | **Seleção balanceadora**: vantagem do heterozigoto HbA/HbS |
| Navios de migrantes | **Fluxo gênico** |
| Sobrenomes | Sobrenomes também derivam, como um marcador do cromossomo Y |

O modo professor mostra os genótipos escondidos de todos os colonos. O jogo é salvo automaticamente no navegador.

### ▶️ [Jogar o Fundadores](https://piergiorge.github.io/Vale-do-Sereno/fundadores/)

---

# 🖥️ Laudo

**Perícia criminal numa tela de computador de tubo.** É 1997 e você é a perita Lia Moura, do Instituto de Criminalística do Vale do Sereno. O jogo inteiro acontece no SIPEC, um sistema em pixel art de 8 bits: ofícios do delegado, fotos da cena para examinar, requisição de exames com orçamento e prazo, resultados (eletroferogramas de verdade para ler), cálculos de frequência e de paternidade, contatos e o laudo, que vai para o juiz. Afirmar o que não foi examinado derruba o laudo no tribunal.

**Temporada (1997–1998).** Dez casos ligados entre si, que terminam na Mina Velha:

| Caso | O que ensina |
|---|---|
| 001. Arrombamento na Farmácia Sereno | DNA degradado, irmãos com o mesmo perfil parcial, banco de frequências local |
| 002. Carne de boi? | Identificação de espécie pelo DNA (código de barras COI), fauna silvestre |
| 003. A herança dos Rezende | Paternidade post-mortem, mutação de um passo, Y-STR |
| 004. O corpo na trilha | Entomologia forense e intervalo pós-morte |
| 005. Unhas | Misturas de DNA; o Y-STR isola o homem numa mistura com mulher |
| 006. O Mal da Vila Nova | Toxicologia: contaminação por chumbo, não envenenamento |
| 007. A ossada do rio | Pessoa desaparecida: mtDNA, Y-STR e comparação com os pais |
| 008. Feira de domingo | Tráfico de aves: espécie ameaçada e filhotes que não são do casal registrado |
| 009. Chumbinho na festa | Toxicologia e mistura; DNA num objeto mostra contato, não autoria |
| 010. Os ossos da Mina Velha | Antropologia forense, trauma perimortem, linhagens comuns numa população fundadora |

**Plantão.** Casos gerados a cada partida, sorteados entre identificação, misturas, paternidade (inclusive com o tio no lugar do pai), espécie, pessoas desaparecidas, toxicologia e entomologia. Cada plantão tem um código e pode ser repetido.

A reviravolta que atravessa o jogo é a genética forense numa **população fundadora**: no Vale, um perfil de DNA compatível pesa bem menos do que no resto do país, e um Y-STR aponta uma família inteira. Os casos se liberam em sequência; um botão na lista de processos libera todos de uma vez, para uso em aula. O progresso fica salvo no navegador. Perfis, famílias e frequências alélicas são fictícios.

### ▶️ [Jogar o Laudo](https://piergiorge.github.io/Vale-do-Sereno/Laudo/)

---

# 🗼 Torre 3

**Guarda-parque numa torre de vigia, numa tela só.** No estilo de *Do Not Feed the Monkeys*: seis câmeras da Reserva do Sereno, um mapa, sensores de temperatura, umidade, som e movimento, e um rádio que não para. O relógio corre das 18:00 às 06:00 (dá para pausar e acelerar). Quando algo aparece numa câmera, você decide quem sai: brigada de incêndio, patrulha de guarda-parques, polícia ambiental, resgate de fauna, coleta de amostra para o laboratório, Vigilância em Saúde ou ninguém (só registrar). As equipes são poucas e levam tempo para ir e voltar.

| O que aparece | O que ensina |
|---|---|
| Fumaça, neblina, fogueira de quintal | Ler sensores: fogo é quente e seco e sobe em coluna; neblina é fria, com umidade perto de 100%. O fogo cresce e pula de área |
| Luzes azuis no brejo ("Boitatá") | Fogo-fátuo: gases da decomposição em áreas alagadas |
| Pegadas "viradas" ("Curupira") | O rastro do tamanduá-bandeira, que anda com as garras dobradas |
| Bugios mortos | Primatas como sentinelas da febre amarela silvestre; quem transmite é o mosquito |
| Tamanduá atropelado, lobo-guará com arame | Quando resgatar fauna |
| Onça com filhotes, filhote de ave no chão | Quando **não** intervir |
| Caçador armado, laço com ceva, motosserra, balsa de garimpo | Crimes ambientais, segurança da equipe, mercúrio e biomagnificação |

**Temporada.** Cinco turnos roteirizados (Primeira noite, Tiros no escuro, Luzes no brejo, Rio barrento, Noite seca) e **plantão livre**, sorteado a cada partida. No fim de cada turno, um relatório mostra o que aconteceu em cada ocorrência e explica a biologia por trás. As amostras vão para o Laboratório de Perícia do Vale, o mesmo do Laudo: a carne apreendida é identificada pelo gene COI, e a água do garimpo, testada para mercúrio. Barra de espaço pausa; teclas 1 a 6 trocam de câmera.

### ▶️ [Jogar o Torre 3](https://piergiorge.github.io/Vale-do-Sereno/torre-3/)

---

## Detalhes técnicos

Cada jogo é um único arquivo HTML com JavaScript puro, sem bibliotecas nem dependências externas. Os sons e a música são gerados por código (Web Audio API). Os gráficos do Locus Astra são SVG gerados a partir do fenótipo de cada criatura.

```
index.html             menu (mapa do Vale do Sereno)
fita-molde/index.html
genoblocos/index.html
gulp/index.html
locus-astra/index.html
surto/index.html
linhagem/index.html
heranca/index.html
operon/index.html
fundadores/index.html
Laudo/index.html
torre-3/index.html
```

No Fita Molde:
- Renderização em `<canvas>` com física em passo fixo (120 Hz), o que mantém o pulo igual em qualquer taxa de quadros.
- Pulo com tempo de tolerância na borda (*coyote time*), buffer de pulo e altura variável.
- Inimigos com detecção de bordas e paredes para patrulhar sem cair das plataformas.

Para jogar sem internet, baixe o `index.html` do jogo e abra no navegador.

## Uso

Jogar e usar os jogos em sala de aula é livre e gratuito. Para reutilizar ou modificar o código, consulte os termos do repositório ou fale com o autor.

## Autor

Rafael Piergiorge ([@Piergiorge](https://github.com/Piergiorge))
