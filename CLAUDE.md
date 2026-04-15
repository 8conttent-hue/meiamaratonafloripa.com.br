# CLAUDE.md — MEIAMARATONAFLORIPA

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** MEIAMARATONAFLORIPA
**Nicho:** Esportes e Fitness
**Keywords:** A mais ou menos 3 anos decidir criar o site e isso
**Paleta de cores:** forest | **Fonte:** outfit

A mais ou menos 3 anos decidir criar o site e isso tem renovado minha energia com a corrida. Amo compartilhar todo o meu conhecimento através da internet. Meu objetivo é passar todo os meus aprendizados de forma simples para que o máximo de pessoas sejam beneficiadas com ele. Olá! Seja muito bem vindo ao meu site, me chamo Felipe Nobre, tenho 31 anos e sou corredor de maratona profissional a mais de 7 anos. Criei este portal para dividir um pouco da minha experiência que adquiri ao longo dos anos nas ruas. Muitos conhecido sempre falam para eu criar um site e compartilhar minhas experiências.



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-D |
| Hero | Hero-C |
| Features | Features-A |
| About Section | About-I |
| Posts | Posts-D |
| Footer | Footer-D |
| Página Sobre | Sobre-A |
| Página Contato | Contato-F |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
