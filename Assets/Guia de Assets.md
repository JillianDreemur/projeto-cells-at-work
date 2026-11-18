---
tags: [cells-at-work, assets]
---
# Guia de Assets

## Estrutura

```
Assets/
├── aseprite/      ← arquivos-fonte editáveis (.aseprite)
├── sprites/       ← PNGs exportados, prontos para usar no jogo
└── sons/          ← músicas e efeitos sonoros (.mp3)
```

`aseprite/` e `sprites/` têm a **mesma estrutura interna e os mesmos nomes**. Por exemplo,
`aseprite/personagens/globulo_branco/globulo_branco_andar_direita.aseprite` é exportado para
`sprites/personagens/globulo_branco/globulo_branco_andar_direita.png`.

| Pasta | Conteúdo | Nota |
|---|---|---|
| `personagens/` | glóbulo branco e glóbulo vermelho | [[Glóbulo Branco]], [[Glóbulo Vermelho]] |
| `inimigos/` | vírus | [[Vírus]] |
| `cenarios/` | as 4 telas da veia | [[Cenários]] |
| `interface/` | telas, menu de pausa, diálogos, HUD | [[Interface]] |
| `sons/` | músicas, jingles, efeitos | [[Sons]] |

## Convenção de nomes
- Tudo em minúsculas, `snake_case`, sem acentos nem espaços (evita problemas em engines e no Git).
- Padrão: `<entidade>_<ação>_<direção>`, ex.: `virus_andar_direita`.
- Sons têm prefixo por tipo: `musica_`, `jingle_`, `sfx_`.
- Ao exportar do Aseprite, salve o PNG na pasta espelhada dentro de `sprites/`, com o mesmo nome.

---
Veja também: [[Especificações Técnicas]] · [[Cells at Work]]
