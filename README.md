ï»¿# lead-comenta

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


[![lead-comenta: comentêÂ¡rio vira guia](guia/assets/banner.jpg)](https://inematds.github.io/lead-comenta/guia/)

**ê°Å¸â¡Â§ê°Å¸â¡Â· [PortuguêÂªs](README.md) êÂ· ê°Å¸â¡Âºê°Å¸â¡Â¸ [English](README.en.md) êÂ· ê°Å¸â¡Âªê°Å¸â¡Â¸ [EspaêÂ±ol](README.es.md)**

## O que êÂ©

O lead-comenta cria a pêÂ¡gina do "guia grêÂ¡tis" que vocêÂª promete quando diz "comenta PALAVRA que eu te mando". Serve para quem posta carrossel ou reel com esse convite e precisa ter o material pronto antes de publicar. VocêÂª dêÂ¡ a palavra, o tema e uma fonte (uma pêÂ¡gina ou um arquivo de texto); ele escreve um guia curto de 4 a 7 passos sêÂ³ com o que estêÂ¡ na fonte, gera uma pêÂ¡gina no padrêÂ£o INEMA e os textos prontos para responder o comentêÂ¡rio, a mensagem direta e o story. Precisa de Python 3 e do Claude Code; a publicaêÂ§êÂ£o êÂ© pelo GitHub Pages.

## ê°Å¸ââ Guia de uso

Guia completo (landing + passo a passo): **https://inematds.github.io/lead-comenta/guia/**

## Usar

```bash
cd ~/projetos/lead-comenta
python3 lead.py nova AGENTE --tema "6 tarefas chatas que um agente faz" --fonte https://inematds.github.io/empresa-de-ia/guia/
python3 lead.py lista              # palavras e links
python3 lead.py resposta AGENTE    # textos prontos para responder
git add -A && git commit -m "guia AGENTE" && git push   # a pêÂ¡gina vai ao ar
```

PêÂ¡gina: `https://inematds.github.io/lead-comenta/paginas/<palavra>/` êÂ· exemplo: [AGENTE](https://inematds.github.io/lead-comenta/paginas/agente/).

## O processo, do inêÂ­cio ao fim

ê°Å¸Â§Â  sessêÂ£o com o Nei êÂ· ê¢Å¡â¢ê¯Â¸Â script êÂ· ê°Å¸Â¤â `claude -p` (assinatura)

| # | Passo | Comando / o que acontece | Quem |
|---|---|---|---|
| 1 | Palavra + tema | vem do carrossel-inema, do r7ex ou do Nei | ê°Å¸Â§Â  |
| 2 | Fonte | pêÂ¡gina do inema.club/guia do projeto ou arquivo .md com o conteêÂºdo | ê°Å¸Â§Â  |
| 3 | Guia | `lead.py nova PALAVRA --tema ê¢â¬Â¦ --fonte ê¢â¬Â¦` ê¢â â texto sêÂ³ da fonte | ê°Å¸Â¤â |
| 4 | PêÂ¡gina + respostas | `paginas/<palavra>/index.html` e `respostas.md`; registro em `palavras.json` | ê¢Å¡â¢ê¯Â¸Â |
| 5 | Publicar | `git push` ê¢â â GitHub Pages | ê¢Å¡â¢ê¯Â¸Â |
| 6 | Responder quem comentou | êÂ  mêÂ£o com `respostas.md` (envio automêÂ¡tico: ver `DECISAO-DM.md`) | ê°Å¸Â§Â  |

## Limites

- NêÂ£o envia mensagens: ver `DECISAO-DM.md`.
- O guia sai sêÂ³ do que estêÂ¡ na fonte; fonte pobre = guia curto.
- Resposta pêÂºblica no comentêÂ¡rio vai sem link (o Instagram tende a esconder comentêÂ¡rio com link).

LicenêÂ§a: MIT.

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>