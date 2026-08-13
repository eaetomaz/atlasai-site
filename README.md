# atlasai-site

Site estático com as 3 páginas exigidas pelo cadastro de app no TikTok for Developers:

- `index.html` — área de trabalho/web do app
- `termos.html` — Termos de Serviço
- `privacidade.html` — Política de Privacidade

## Publicar no GitHub Pages

```bash
cd atlasai-site
git init
git add .
git commit -m "Site inicial do AtlasAI"
git branch -M main
git remote add origin https://github.com/eaetomaz/atlasai-site.git
git push -u origin main
```

Depois, em https://github.com/eaetomaz/atlasai-site/settings/pages, em "Build and deployment",
selecione "Deploy from a branch" → branch `main` → pasta `/ (root)`.

URLs finais (podem levar alguns minutos para ficar no ar após o primeiro deploy):

- Área de trabalho: `https://eaetomaz.github.io/atlasai-site/`
- Termos de Serviço: `https://eaetomaz.github.io/atlasai-site/termos.html`
- Política de Privacidade: `https://eaetomaz.github.io/atlasai-site/privacidade.html`

## Verificação de domínio do TikTok

Quando o TikTok for Developers gerar o arquivo de verificação (algo como
`tiktok-developers-site-verification-XXXXXXXX.txt` ou um arquivo HTML), salve ele direto nesta
pasta (raiz, ao lado do `index.html`) e rode de novo:

```bash
git add .
git commit -m "Verificação de domínio TikTok"
git push
```

Ele precisa ficar acessível em `https://eaetomaz.github.io/atlasai-site/<nome-do-arquivo>`.
