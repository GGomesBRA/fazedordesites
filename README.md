# Fazedor de Sites

Landing page estática para venda do agente de IA que cria e publica sites em minutos (deploy Netlify + checkout Hotmart).

## Arquivos
- `index.html`: variação A (azul/verde, foco em velocidade e prova social)
- `index-b.html`: variação B (âmbar/escuro, foco em escassez e ancoragem)
- `netlify.toml`: redireciona `/` para A e `/b` para B em produção Netlify

## Como rodar localmente
```bash
# usando npm serve
npx serve .
# ou python
python -m http.server 4173
```
Acesse http://localhost:3000 ou a porta exibida. Use `/b` para ver a variação B.

## Deploy na Netlify
1. Crie um novo site na Netlify apontando para este diretório.
2. Defina build command vazio e publish dir `.`.
3. Deploy manual (arraste o zip) ou conecte ao repositório.
4. Redirecionamentos já configurados em `netlify.toml` (raiz -> index, `/b` -> index-b).

## Hotmart
Atualize os links de CTA (`https://hotmart.com`) para a URL do seu checkout/checkout split.

## Personalização rápida
- Cores: ajuste variáveis `:root` em cada HTML.
- Textos: edite hero, provas sociais, FAQ e CTAs.
- Imagens: substitua URLs do Unsplash por imagens do produto/cliente e salve em formatos `.webp`/`.avif`.
