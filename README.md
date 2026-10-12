# Edição de Vídeos — HyperFrames

Projeto de vídeo baseado no [HyperFrames](https://github.com/heygen-com/hyperframes):
vídeos escritos em HTML/CSS + animações (GSAP) e renderizados em MP4.

## Como usar com o Claude

As skills do HyperFrames já estão em `.claude/skills/`, então qualquer sessão do
Claude Code neste repositório já as carrega. Basta pedir, por exemplo:

> Usando /hyperframes, crie uma intro de 15 segundos sobre [seu tema]

> Usando /embedded-captions, adicione legendas neste vídeo (envie o .mp4)

## Comandos

```bash
npm run dev      # pré-visualização no navegador (Studio)
npm run check    # valida a composição
npm run render   # renderiza para MP4 (saída em renders/)
```

Requisitos: Node.js 22+ e FFmpeg.

## Estrutura

- `index.html` — composição principal (o vídeo)
- `assets/` — imagens, vídeos, áudios e scripts usados no vídeo
- `assets/vendor/gsap.min.js` — GSAP 3.14.2 local (não depende de CDN)
- `renders/` — vídeos renderizados (ignorado pelo git)
