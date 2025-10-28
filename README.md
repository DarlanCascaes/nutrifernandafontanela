# Nutri Fernanda Fontanela - Site Migrado para GitHub Pages

Este é o site da Nutricionista Fernanda Fontanela, migrado de WordPress para uma versão estática compatível com GitHub Pages.

## Estrutura do Projeto

```
.
├── index.html          # Página principal
├── css/               # Folhas de estilo
├── js/                # Arquivos JavaScript
├── images/            # Imagens do site
├── README.md          # Este arquivo
└── .gitignore         # Arquivos a ignorar no Git
```

## Características Preservadas

- ✅ Layout responsivo
- ✅ Elementos interativos (toggles, carrosséis)
- ✅ Formulários funcionais
- ✅ Imagens otimizadas
- ✅ Navegação completa

## Como Fazer Deploy no GitHub Pages

### 1. Criar um repositório no GitHub

1. Acesse [github.com](https://github.com) e faça login
2. Clique em "New" para criar um novo repositório
3. Nomeie como `seu-usuario.github.io` (substitua `seu-usuario` pelo seu username)
4. Deixe como público
5. Clique em "Create repository"

### 2. Clonar o repositório localmente

```bash
git clone https://github.com/seu-usuario/seu-usuario.github.io.git
cd seu-usuario.github.io
```

### 3. Copiar os arquivos do site

Copie todos os arquivos deste projeto (index.html, css/, js/, images/) para o diretório do repositório.

### 4. Fazer commit e push

```bash
git add .
git commit -m "Adicionar site Nutri Fernanda Fontanela"
git push origin main
```

### 5. Acessar o site

Seu site estará disponível em: `https://seu-usuario.github.io`

## Configuração Alternativa (Subdomínio)

Se preferir usar um domínio personalizado:

1. Vá para as configurações do repositório no GitHub
2. Procure por "Pages"
3. Em "Custom domain", adicione seu domínio
4. Configure os registros DNS do seu domínio apontando para GitHub Pages

## Elementos Interativos

O site inclui:

- **Toggles/Acordeões**: Clique para expandir/recolher respostas
- **Carrosséis**: Navegue entre imagens
- **Links de Navegação**: Funcionam normalmente
- **Formulários**: Podem ser integrados com serviços como Formspree

## Otimizações Realizadas

- Remoção de scripts do WordPress que causavam erros
- Correção de caminhos de arquivos (CSS, JS, imagens)
- Limpeza de metadados desnecessários
- Mantém toda a funcionalidade Elementor Pro em HTML/CSS/JS puro

## Suporte

Para dúvidas sobre o deployment, consulte a [documentação oficial do GitHub Pages](https://docs.github.com/en/pages).

---

**Desenvolvido por:** Nutri.ads  
**Data de Migração:** Outubro 2025
