# Site Dra. Fernanda Melo | Nutricionista Clínica

Landing page estática (HTML, CSS e JS num único `index.html`), sem etapa de build.

## Estrutura
- `index.html`: página completa (CSS e JS embutidos)
- `img/`: fotos em webp (versões grande e pequena para celular)
- `vendor/`: GSAP 3.12.5, ScrollTrigger e Lenis 1.1.13 (servidos pelo próprio site, sem depender de CDN)
- `favicon.svg`, `apple-touch-icon.png`, `og-image.jpg`
- `vercel.json`: URLs limpas e cache longo para imagens

## Rodar localmente
```
python3 -m http.server 8000
```
Abra http://localhost:8000

## Publicar na Vercel
1. Suba esta pasta para um repositório no GitHub.
2. Na Vercel: Add New > Project > importe o repositório.
3. Framework Preset: Other. Build Command: vazio. Output Directory: `./`.
4. Cada push na branch principal publica de novo automaticamente.

Depois de ter o domínio final, troque a URL em `<link rel="canonical">` no `index.html`.

## Pendências de conteúdo
- CRN da Fernanda (obrigatório pelo Conselho de Nutrição): adicionar no rodapé e na seção Sobre.
- Confirmar se atende online.
