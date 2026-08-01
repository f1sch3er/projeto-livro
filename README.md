# 📖 Antes Que o Dia Termine — Página de Download

Página para baixar o livro gratuitamente (obra de coração). Hospedagem **gratuita** na Vercel.

---

## 🚀 Deploy automático na Vercel (grátis)

O projeto está no GitHub (`f1sch3er/projeto-livro`). O ideal é **conectar o Vercel ao GitHub**: aí **toda vez que você der `git push`, o deploy acontece sozinho**. Sem terminal, sem comandos.

### Opção 1 — Conectar ao GitHub (deploy automático) ✅ RECOMENDADO

1. Acesse [vercel.com](https://vercel.com) e faça login com a conta que já está conectada.
2. No dashboard, clique em **Add New… → Project**.
3. Selecione o repositório **`projeto-livro`** (na aba de importação do GitHub).
4. A Vercel detecta que é HTML estático automaticamente. Só clique em **Deploy**.
5. Pronto! URL: `https://projeto-livro-xxxxx.vercel.app`

**A partir daí, cada `git push` no GitHub publica automaticamente.** Para atualizar o site, é só:

```bash
git add -A
git commit -m "ajustes"
git push
```

---

### Opção 2 — Pelo site (sem terminal, sem GitHub)

1. Acesse [vercel.com](https://vercel.com) e faça login.
2. No dashboard, clique em **Add New… → Project**.
3. Clique em **Deploy without Git** (ou arraste a pasta direto).
4. Arraste a pasta `projeto-livro` (com `index.html` e `capa.jpg` dentro).
5. Clique em **Deploy**.
6. Pronto! URL: `https://projeto-livro-xxxxx.vercel.app`

> ⚠️ Essa opção **não** tem deploy automático — precisa repetir o upload a cada alteração.

---

### Opção 3 — Pela CLI (terminal)

```bash
npm i -g vercel
cd "C:\Users\pedro\Desktop\FISCHER\project\projeto-livro"
vercel --prod
```

Na primeira vez pede **login** (email ou GitHub) — abre uma página no navegador para autorizar. Também **não** tem deploy automático.

> 💡 **Dica:** depois de pronto, vá nas configurações do projeto na Vercel e cadastre um **domínio personalizado** se quiser (ex: `seulivro.com.br`).

---

## 📝 Como atualizar o site depois de subir

O site já sobe e fica no ar. O **download do livro já está configurado** (Google Drive, obra de coração — 100% gratuito), o **Instagram** e o **contato** (email + WhatsApp com mensagem pronta) já estão com os dados corretos.

Para mudar algo no `index.html` (no seu computador) e publicar **automaticamente** (se conectou ao GitHub):

```bash
git add -A
git commit -m "ajustes"
git push
```

> 🔗 **Download do livro:** o botão "📥 Baixar o livro grátis" abre um **modal de apoio opcional** (doar ou baixar grátis). O download usa o link direto do Google Drive. Se um dia quiser trocar o arquivo, substitua o `href` (formato `https://drive.google.com/uc?export=download&id=SEU_ID`).

> 💛 **Doação opcional (no modal):** o botão "Doar este valor" aponta para `https://buy.stripe.com/SEU_LINK_AQUI` (placeholder). Para ativar, crie um **Payment Link** no Stripe ("o cliente escolhe o valor", mínimo R$ 1) e troque o `href` do botão `#donateModalBtn` no `index.html`.

> 🔓 **Importante:** no Google Drive, deixe o arquivo com permissão **"Qualquer pessoa com o link"** para leitura — senão o download pede login.
