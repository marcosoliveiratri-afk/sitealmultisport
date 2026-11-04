# AL MULTISPORT — site (pacote de produção)

Site estático (sem build). Publicar pela Vercel a partir do GitHub.

## Arquivos
- `index.html`: o site (HTML, CSS e JS). As imagens ficam em `img/`.
- `404.html`, `politica-de-privacidade.html`, `termos-de-uso.html`
- `favicon.ico`, `favicon-32.png`, `apple-touch-icon.png`, `icon-192.png`, `icon-512.png`, `site.webmanifest`
- `og-image.png` (imagem de compartilhamento 1200×630)
- `robots.txt`, `sitemap.xml`
- `vercel.json` (cabeçalhos de segurança, URLs limpas e cache das imagens)

## Publicar (GitHub + Vercel)
1. Suba todos os arquivos (mantendo a pasta `img/`) na branch `main` do repositório.
2. Na Vercel: **Add New → Project**, importe o repositório. Framework: **Other**. Sem comando de build e sem pasta de saída.
3. Em **Settings → Domains**, ligue o domínio. O HTTPS (SSL) é automático.

## Antes de publicar: preencher
1. **Domínio**: troque `SEU-DOMINIO.com.br` pelo endereço real em `index.html`, `robots.txt`, `sitemap.xml` (no VS Code: Ctrl+Shift+H, "substituir em todos os arquivos").
2. **Google Analytics**: em `index.html`, procure `const GA_ID=''` e coloque o ID (ex.: `G-XXXXXXXXXX`). Enquanto estiver vazio, nenhum cookie é usado e o aviso de cookies não aparece. Com o ID, o aviso aparece e o GA só carrega se o visitante aceitar. Eventos enviados: `click_whatsapp`, `click_area_aluno` e `erro_js`.
3. **WhatsApp e preços**: `const WA` e `const PRECO` ficam no final do `index.html`.

## Depois de publicar
- **Google Search Console**: adicione o site como propriedade (domínio ou prefixo de URL), confirme a propriedade e envie `https://SEU-DOMINIO.com.br/sitemap.xml`.
- **PageSpeed**: teste em https://pagespeed.web.dev
- **Prévia no WhatsApp**: teste o link em https://developers.facebook.com/tools/debug/ (limpa o cache da prévia).
