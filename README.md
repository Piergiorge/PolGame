# PolGame — Fita Molde

**Um platformer 2D sobre replicação do DNA.** Você é a DNA polimerase: atravesse a célula coletando nucleotídeos complementares para copiar a fita molde, corrija seus erros com a revisão 3'→5' e chegue ao telômero.

### ▶️ [Jogar agora](https://piergiorge.github.io/PolGame/)

Roda direto no navegador, no computador ou no celular. Não precisa instalar nada.

---

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

## Detalhes técnicos

- Um único arquivo `index.html` com HTML, CSS e JavaScript puro, sem bibliotecas nem dependências externas.
- Renderização em `<canvas>` com física em passo fixo (120 Hz), o que mantém o pulo igual em qualquer taxa de quadros.
- Pulo com tempo de tolerância na borda (*coyote time*), buffer de pulo e altura variável.
- Inimigos com detecção de bordas e paredes para patrulhar sem cair das plataformas.

Para jogar sem internet, baixe o `index.html` e abra no navegador.

## Próximas fases (ideias)

- Fita descontínua: fragmentos de Okazaki, primase e DNA ligase
- Transcrição: RNA polimerase, uracila no lugar de timina
- Tradução: ribossomo, tRNAs e anticódons

## Licença

Veja o arquivo [LICENSE](LICENSE).

## Autor

Rafael Piergiorge ([@Piergiorge](https://github.com/Piergiorge))
