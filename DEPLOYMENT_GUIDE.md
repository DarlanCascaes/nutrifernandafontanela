# Guia Completo de Deployment no GitHub Pages

## 📋 Pré-requisitos

- Conta no GitHub (https://github.com)
- Git instalado no seu computador
- Conhecimento básico de linha de comando

## 🚀 Passo a Passo

### 1️⃣ Criar um Repositório no GitHub

1. Acesse [github.com](https://github.com) e faça login
2. Clique no ícone **+** no canto superior direito
3. Selecione **New repository**
4. **Nome do repositório**: `seu-usuario.github.io`
   - Substitua `seu-usuario` pelo seu nome de usuário do GitHub
   - Este é o padrão obrigatório para GitHub Pages pessoal
5. **Descrição** (opcional): "Site da Nutricionista Fernanda Fontanela"
6. Deixe como **Public** (obrigatório para GitHub Pages)
7. Clique em **Create repository**

### 2️⃣ Clonar o Repositório Localmente

Abra o terminal/prompt de comando e execute:

```bash
git clone https://github.com/seu-usuario/seu-usuario.github.io.git
cd seu-usuario.github.io
```

### 3️⃣ Copiar os Arquivos do Site

Copie todos os arquivos deste projeto para o diretório clonado:

```
seu-usuario.github.io/
├── index.html
├── css/
├── js/
├── images/
├── README.md
├── .gitignore
├── _config.yml
└── .nojekyll
```

### 4️⃣ Fazer Commit e Push

```bash
git add .
git commit -m "Adicionar site Nutri Fernanda Fontanela"
git push origin main
```

Se receber erro sobre a branch, use:
```bash
git branch -M main
git push -u origin main
```

### 5️⃣ Verificar o Deploy

1. Vá para as configurações do repositório no GitHub
2. Procure por **Pages** na barra lateral esquerda
3. Verifique se a source está configurada como "Deploy from a branch"
4. Aguarde alguns minutos (geralmente 1-2 minutos)
5. Seu site estará disponível em: `https://seu-usuario.github.io`

## 🌐 Usar um Domínio Personalizado

Se você tem um domínio próprio (como `nutrifernanda.com.br`):

### Via GitHub Pages:

1. Vá para as configurações do repositório
2. Procure por **Pages**
3. Em **Custom domain**, adicione seu domínio
4. Clique em **Save**

### Configurar DNS:

Você precisará apontar os registros DNS do seu domínio para GitHub Pages. As instruções variam conforme o provedor de domínio, mas geralmente envolve:

**Opção 1 - Registros A (recomendado):**
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

**Opção 2 - CNAME:**
```
seu-usuario.github.io
```

Consulte a [documentação oficial do GitHub Pages](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site) para instruções específicas do seu provedor.

## 📝 Atualizações Futuras

Para fazer atualizações no site:

```bash
# Fazer alterações nos arquivos

# Fazer commit
git add .
git commit -m "Descrição das alterações"

# Fazer push
git push origin main
```

O site será atualizado automaticamente em poucos minutos.

## ❌ Solução de Problemas

### Site não aparece após o push

- Aguarde 2-3 minutos
- Verifique se o repositório está como **Public**
- Verifique se o arquivo `index.html` está na raiz do repositório
- Limpe o cache do navegador (Ctrl+Shift+Del)

### Erro 404 em alguns recursos

- Verifique se os caminhos dos arquivos CSS, JS e imagens estão corretos
- Certifique-se de que todos os arquivos foram feitos push para o GitHub

### Problema com HTTPS

GitHub Pages fornece HTTPS automaticamente. Se não funcionar:
- Aguarde alguns minutos após a primeira publicação
- Verifique se a opção "Enforce HTTPS" está habilitada nas configurações

## 📚 Recursos Úteis

- [Documentação GitHub Pages](https://docs.github.com/en/pages)
- [Guia de Domínios Personalizados](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)
- [Troubleshooting](https://docs.github.com/en/pages/getting-started-with-github-pages/troubleshooting-common-issues-with-github-pages)

---

**Desenvolvido por:** Nutri.ads  
**Data:** Outubro 2025
