# 📖 Antes Que o Dia Termine — Página de Download

Página para baixar o livro gratuitamente (obra de coração). Hospedagem **gratuita** na Vercel.

---

## 🚀 Deploy na Vercel (grátis)

O projeto é 100% HTML estático (`index.html` + `capa.jpg`), então a Vercel publica sozinha. Você tem **2 formas** de subir:

---

### Opção 1 — Pelo site (sem terminal, mais fácil) ✅

1. Acesse [vercel.com](https://vercel.com) e faça login com sua conta **GitHub** (ou Google).
2. No dashboard, clique em **Add New… → Project**.
3. Clique em **Deploy without Git** (ou arraste a pasta direto).
4. Arraste a pasta `projeto-livro` (com `index.html` e `capa.jpg` dentro).
5. Clique em **Deploy**.
6. Pronto! URL: `https://projeto-livro-xxxxx.vercel.app`

---

### Opção 2 — Pela CLI (terminal) 🚀

#### 1. Instale a CLI da Vercel (só uma vez)

```bash
npm i -g vercel
```

#### 2. Faça o deploy

```bash
cd "C:\Users\pedro\Desktop\FISCHER\project\projeto-livro"
vercel
```

- Na primeira vez ele pede **login** (email ou GitHub) — abre uma página no navegador para autorizar.
- Depois é só dar **Enter** em tudo — a Vercel detecta que é HTML estático e sobe sozinha.
- Ele vai dar uma URL de **preview**. Quando estiver satisfeito, rode:

```bash
vercel --prod
```

Seu site estará em: `https://projeto-livro-xxxxx.vercel.app`

> 💡 **Dica:** depois de pronto, vá nas configurações do projeto na Vercel e cadastre um **domínio personalizado** se quiser (ex: `seulivro.com.br`).

---

## 📝 O que editar depois de subir

O site já sobe e fica no ar. O **download do livro já está configurado** (Google Drive, obra de coração — 100% gratuito), o **Instagram** e o **contato** (email + WhatsApp com mensagem pronta) já estão com os dados corretos.

Quando editar o `index.html` (no seu computador), **suba de novo** com:

```bash
vercel --prod
```

> 🔗 **Download do livro:** o botão "📥 Baixar o livro grátis" usa o link direto do Google Drive. Se um dia quiser trocar o arquivo, substitua o `href` (formato `https://drive.google.com/uc?export=download&id=SEU_ID`).

> 🔓 **Importante:** no Google Drive, deixe o arquivo com permissão **"Qualquer pessoa com o link"** para leitura — senão o download pede login.
