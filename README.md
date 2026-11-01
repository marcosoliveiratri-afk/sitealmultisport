# AL MULTISPORT — site

Site institucional da AL MULTISPORT (assessoria esportiva de corrida, ciclismo e triathlon).
É uma página única (`index.html`), sem build: basta abrir no navegador ou publicar como está.

## Antes de publicar (editar no `index.html`)

1. **WhatsApp**: já configurado com `5511971502554`. Para trocar, procure `const WA=` no final do arquivo (formato: DDI + DDD + número, sem espaços ou traços).
2. **Preços**: procure `const PRECO=` e ajuste os valores dos planos.
3. **Modalidades e botão "Sou Aluno"**: os cards (na primeira tela e na seção de modalidades) abrem o WhatsApp com uma mensagem pronta (procure `data-msg=` no `index.html`). O botão "Sou Aluno" abre a área de treinos em https://treinosalmultisport.lovable.app/.

## Publicar no GitHub Pages

1. Suba estes arquivos para a branch `main` do repositório.
2. No GitHub: **Settings → Pages → Build and deployment**.
3. Em **Source**, escolha **Deploy from a branch**, branch `main`, pasta `/ (root)`, e salve.
4. Em alguns minutos o site fica em `https://marcosoliveiratri-afk.github.io/sitealmultisport/`.

Para usar domínio próprio, configure em **Settings → Pages → Custom domain**.

## Estrutura

- `index.html`: o site inteiro (HTML, CSS e JS; as imagens estão embutidas).
- `.nojekyll`: faz o GitHub Pages servir o arquivo exatamente como está.
