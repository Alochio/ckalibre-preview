# Ckalibri — Landing Page (Demonstração)

Recriação do front-end de demonstração da Ckalibri, mantendo a direção visual e a estrutura da proposta de 29/10/2026.

## Arquivos

- `index.html` — toda a página com HTML, CSS e JavaScript.
- `assets/favicon.svg` — ícone da aba.
- `.nojekyll` — impede processamento desnecessário pelo Jekyll no GitHub Pages.

**Não há dependências, Node.js, React, Vite ou etapa de build.** O site é estático, responsivo e pode ser publicado no GitHub Pages gratuitamente.

## Testar no computador

Abra `index.html` em um navegador ou, para um servidor local:

```bash
python -m http.server 8080
```

Depois abra `http://localhost:8080`.

## Publicar no GitHub Pages (sem GitHub Actions)

1. Crie um repositório no GitHub, por exemplo `ckalibri-demo`.
2. Extraia o ZIP e envie o **conteúdo da pasta** para a raiz do repositório (`index.html`, `assets/`, `.nojekyll`, `README.md`). Não envie somente o ZIP.
3. Faça commit na branch `main`.
4. Entre em **Settings → Pages**.
5. Em **Build and deployment → Source**, escolha **Deploy from a branch**.
6. Em **Branch**, selecione `main` e `/ (root)`. Clique em **Save**.
7. O endereço será `https://SEU-USUARIO.github.io/ckalibri-demo/` (ajuste usuário e repositório).

**Importante:** Não precisa criar `gh-pages`, não precisa de `.github/workflows` e não deve escolher GitHub Actions para esta versão. Isso evita o erro de `actions/configure-pages` quando Pages não está configurado para Actions.

## Funcionalidades

- Identidade industrial verde, verde-lima e tons claros.
- Navegação com menu mobile, links âncora e cabeçalho fixo.
- Ilustrações SVG embutidas (sem dependência de arquivos externos).
- Filtros interativos de serviços.
- Detalhes dos serviços em modal acessível, com preenchimento automático da especialidade no orçamento.
- Formulário que prepara uma mensagem e abre o WhatsApp do visitante (não salva nem envia dados por servidor).
- Acesso ao portal real de certificados.
- Metadados para SEO, favicon e animações respeitando preferência por movimento reduzido.

## Antes de divulgar como site oficial

Esta é uma **proposta visual**, não um site institucional oficialmente aprovado. Confirme com a Ckalibri logotipo/marca, textos, especialidades, escopo e acreditações, contatos e endereço, e autorização de publicação. O símbolo e a palavra-marca aqui são estilizações demonstrativas. O telefone do WhatsApp usado na demonstração é `+55 31 99508-7713` e o portal é `https://certificados.ckalibri.com.br/`.

## Personalização rápida

- **Cores:** variáveis CSS em `:root` no começo de `index.html`.
- **Telefone e link do WhatsApp:** procure por `5531995087713`.
- **Serviços:** edite os seis cards em `#service-grid` e o objeto `services` no JavaScript.
- **Textos e endereços:** procure no próprio HTML.

