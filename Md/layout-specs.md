# Agent Cards — Layout Final (Aprovado pelo JP)

> Posicoes e estilos definitivos para todas as 30 cards
> Template: Front.png (327x538) + Back.png (327x538)
> Card scene: 360x520px

---

## Camadas (z-index)

1. **Art layer** (z-index: auto) — imagem do personagem, atras do frame
2. **Frame layer** (z-index: 2) — Front.png com transparencia
3. **Text layer** (z-index: 3) — todos os textos por cima

---

## Posicoes Finais

### Arte do personagem
- top: 12.1% | left: 13.5% | width: 74% | height: 52.8%
- img: width 100%, height 120%, object-fit: cover, object-position: center 15%

### Nome (ex: "JP")
- top: 4.5% | center | z-index: 3
- Font: Cinzel 900, 22px, #FFD700
- text-shadow: 0 0 12px rgba(255,215,0,0.6), 0 2px 4px rgba(0,0,0,0.8)

### Titulo (ex: "The Boss")
- top: 66% | center | z-index: 3
- Font: Cinzel 700, 14px, #FFFFFF, uppercase
- text-shadow: 0 0 8px rgba(0,212,255,0.4), 0 1px 3px rgba(0,0,0,0.9)

### Tagline (ex: "Every agent answers to someone...")
- Dentro da area de habilidades, italic, 9px, #9999CC, text-align: left

### Habilidades
- top: 73% | bottom: 7% | padding-left: 52px | padding-right: 14px | z-index: 3
- Sem pontos/dots antes das frases
- ability-name: 700, 10px, #00D4FF
- ability-desc: 9.5px, #9999BB

### Numero (ex: "#001 / 030")
- bottom: 5% | right: 8% | z-index: 3
- Font: 13px, 700, #8899BB

### Time Betinho
- bottom: 4% | left: 26% | z-index: 3
- Font: 10px, #8899BB

---

## Imagens DALL-E

### Prompt base para arte dos personagens
```
Digital character portrait illustration, square format, NO TEXT, NO FRAME, NO BORDER, NO CARD ELEMENTS. Just the character on a dark background. [DESCRICAO DO PERSONAGEM]. Dramatic cinematic lighting from below with orange rim light. Background: dark tech environment with holographic data visualizations. Style: semi-realistic digital painting, detailed, moody cyberpunk. Facing camera. Isolated on very dark navy (#0A0E1A) background.
```

### Parametros DALL-E
- model: dall-e-3
- size: 1024x1024
- quality: hd

---

## Card scene e efeitos

- Card: 360x520px, border-radius: 14px
- Glow Mythic: conic-gradient rotativo (FFD700, FF3900, 00D4FF)
- Hover: rotateY(-3deg) rotateX(3deg) scale(1.02)
- Shine sweep: rgba(255,255,255,0.06) da esquerda pra direita
- Flip: rotateY(180deg), 0.8s cubic-bezier
- Particulas: 25, cores #FF3900 e #00D4FF
