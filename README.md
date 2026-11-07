# Suporte Inteligente — Já Deu Certo

Chat de suporte automático para bancas (Acertos Club, Feiticeira, Super Acertos, Banca Brasileira, SuperBancas, Tiger Club).

**Domínio:** https://www.jadeucerto.net

## Arquivos

- `index.html` — aplicação completa do chat
- `ads.txt` — autorização AdSense (obrigatório na raiz do domínio)

## Publicar no domínio

1. Faça upload de **todos** os arquivos para a **raiz** do site (ou pasta pública do hosting).
2. Confirme que o `ads.txt` fica acessível em:
   ```
   https://www.jadeucerto.net/ads.txt
   ```
3. No Google AdSense, adicione o site `jadeucerto.net` / `www.jadeucerto.net` e aguarde aprovação.

## AdSense já configurado

- Publisher: `ca-pub-5066020163837493`
- Meta tag + script no `<head>`
- Anúncio exibido na **fila de atendimento** (quando o cliente clica em “Chamar Atendente”)

### Melhorar o anúncio (opcional)

1. No painel AdSense → Anúncios → Por unidade de anúncio → criar um bloco **Display**.
2. Copie o `data-ad-slot` (número) gerado.
3. No `index.html`, na função `getAdSenseHTML()`, troque:
   ```html
   data-ad-slot="auto"
   ```
   pelo número do seu bloco, por exemplo:
   ```html
   data-ad-slot="1234567890"
   ```

## GitHub Pages (alternativa)

Se usar GitHub Pages, o site precisa ser o domínio customizado `www.jadeucerto.net` apontando para o repositório, e o `ads.txt` deve estar na raiz do repositório publicado.
