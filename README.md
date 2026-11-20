# lead-comenta

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


[![lead-comenta: comentÃ¡rio vira guia](guia/assets/banner.jpg)](https://inematds.github.io/lead-comenta/guia/)

**ðŸ‡§ðŸ‡· [PortuguÃªs](README.md) Â· ðŸ‡ºðŸ‡¸ [English](README.en.md) Â· ðŸ‡ªðŸ‡¸ [EspaÃ±ol](README.es.md)**

## O que Ã©

O lead-comenta cria a pÃ¡gina do "guia grÃ¡tis" que vocÃª promete quando diz "comenta PALAVRA que eu te mando". Serve para quem posta carrossel ou reel com esse convite e precisa ter o material pronto antes de publicar. VocÃª dÃ¡ a palavra, o tema e uma fonte (uma pÃ¡gina ou um arquivo de texto); ele escreve um guia curto de 4 a 7 passos sÃ³ com o que estÃ¡ na fonte, gera uma pÃ¡gina no padrÃ£o INEMA e os textos prontos para responder o comentÃ¡rio, a mensagem direta e o story. Precisa de Python 3 e do Claude Code; a publicaÃ§Ã£o Ã© pelo GitHub Pages.

## ðŸ“– Guia de uso

Guia completo (landing + passo a passo): **https://inematds.github.io/lead-comenta/guia/**

## Usar

```bash
cd ~/projetos/lead-comenta
python3 lead.py nova AGENTE --tema "6 tarefas chatas que um agente faz" --fonte https://inematds.github.io/empresa-de-ia/guia/
python3 lead.py lista              # palavras e links
python3 lead.py resposta AGENTE    # textos prontos para responder
git add -A && git commit -m "guia AGENTE" && git push   # a pÃ¡gina vai ao ar
```

PÃ¡gina: `https://inematds.github.io/lead-comenta/paginas/<palavra>/` Â· exemplo: [AGENTE](https://inematds.github.io/lead-comenta/paginas/agente/).

## O processo, do inÃ­cio ao fim

ðŸ§  sessÃ£o com o Nei Â· âš™ï¸ script Â· ðŸ¤– `claude -p` (assinatura)

| # | Passo | Comando / o que acontece | Quem |
|---|---|---|---|
| 1 | Palavra + tema | vem do carrossel-inema, do r7ex ou do Nei | ðŸ§  |
| 2 | Fonte | pÃ¡gina do inema.club/guia do projeto ou arquivo .md com o conteÃºdo | ðŸ§  |
| 3 | Guia | `lead.py nova PALAVRA --tema â€¦ --fonte â€¦` â†’ texto sÃ³ da fonte | ðŸ¤– |
| 4 | PÃ¡gina + respostas | `paginas/<palavra>/index.html` e `respostas.md`; registro em `palavras.json` | âš™ï¸ |
| 5 | Publicar | `git push` â†’ GitHub Pages | âš™ï¸ |
| 6 | Responder quem comentou | Ã  mÃ£o com `respostas.md` (envio automÃ¡tico: ver `DECISAO-DM.md`) | ðŸ§  |

## Limites

- NÃ£o envia mensagens: ver `DECISAO-DM.md`.
- O guia sai sÃ³ do que estÃ¡ na fonte; fonte pobre = guia curto.
- Resposta pÃºblica no comentÃ¡rio vai sem link (o Instagram tende a esconder comentÃ¡rio com link).

LicenÃ§a: MIT.

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>