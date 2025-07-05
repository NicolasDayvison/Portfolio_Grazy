# 🚀 Como fazer o Deploy no GitHub Pages

Este guia vai te ajudar a hospedar o site da Grazy Batista no GitHub Pages.

## 📋 Pré-requisitos

1. Ter uma conta no GitHub
2. Ter o Git instalado no seu computador
3. Ter o projeto pronto (que já está!)

## 🔧 Passo a Passo

### 1. Criar um repositório no GitHub

1. Acesse [github.com](https://github.com) e faça login
2. Clique no botão "+" no canto superior direito
3. Selecione "New repository"
4. Configure o repositório:
   - **Repository name**: `grazy-web` (ou o nome que preferir)
   - **Description**: `Site pessoal da Grazy Batista - UGC Creator`
   - **Visibility**: Public (recomendado para GitHub Pages)
   - **Initialize this repository with**: Deixe desmarcado
5. Clique em "Create repository"

### 2. Fazer upload dos arquivos

#### Opção A: Pelo navegador (mais fácil)
1. No repositório criado, clique em "uploading an existing file"
2. Arraste todos os arquivos do projeto para a área de upload
3. Adicione uma mensagem de commit: "Initial commit - Site da Grazy Batista"
4. Clique em "Commit changes"

#### Opção B: Pelo terminal (para quem conhece Git)
```bash
# Navegue até a pasta do projeto
cd "caminho/para/grazy-web"

# Inicialize o Git
git init

# Adicione todos os arquivos
git add .

# Faça o primeiro commit
git commit -m "Initial commit - Site da Grazy Batista"

# Adicione o repositório remoto
git remote add origin https://github.com/NicolasDayvison/grazy-web.git

# Envie para o GitHub
git branch -M main
git push -u origin main
```

### 3. Configurar o GitHub Pages

1. No repositório, vá em **Settings** (aba superior)
2. No menu lateral esquerdo, clique em **Pages**
3. Em **Source**, selecione **Deploy from a branch**
4. Em **Branch**, selecione **main** e **/(root)**
5. Clique em **Save**

### 4. Aguardar o deploy

- O GitHub vai começar a fazer o build do site
- Pode levar alguns minutos
- Você verá uma mensagem verde "Your site is published at [URL]"
- A URL será algo como: `https://seu-usuario.github.io/grazy-web`

## 🔄 Atualizações futuras

Para fazer atualizações no site:

### Pelo navegador:
1. Vá no arquivo que quer editar
2. Clique no ícone de lápis (Edit)
3. Faça as alterações
4. Clique em "Commit changes"

### Pelo terminal:
```bash
# Faça as alterações nos arquivos
# Depois execute:
git add .
git commit -m "Descrição das alterações"
git push
```

## ⚙️ Configurações importantes

### Atualizar URLs nos arquivos
Depois do deploy, você precisa atualizar as URLs nos seguintes arquivos:

1. **README.md**: Substitua `seu-usuario` pelo seu nome de usuário do GitHub
2. **_config.yml**: Atualize a URL base
3. **sitemap.xml**: Atualize as URLs
4. **robots.txt**: Atualize a URL do sitemap

### Domínio personalizado (opcional)
Se você tiver um domínio próprio:
1. Vá em Settings > Pages
2. Em **Custom domain**, digite seu domínio
3. Clique em **Save**
4. Configure o DNS do seu domínio para apontar para o GitHub Pages

## 🐛 Solução de problemas

### Site não carrega
- Verifique se o repositório é público
- Aguarde alguns minutos para o build
- Verifique se não há erros no código

### Imagens não aparecem
- Verifique se os caminhos estão corretos (relativos)
- Certifique-se de que as imagens foram enviadas

### Vídeos não carregam
- Verifique se os arquivos de vídeo foram enviados
- GitHub Pages tem limite de tamanho de arquivo (100MB)

## 📞 Suporte

Se tiver problemas:
1. Verifique a aba **Actions** no repositório para ver logs de erro
2. Consulte a [documentação do GitHub Pages](https://docs.github.com/en/pages)
3. Verifique se todos os arquivos estão no repositório

## 🎉 Pronto!

Seu site estará disponível em: `https://nicolasdayvison.github.io/grazy-web`

✅ URLs já atualizadas com o nome de usuário NicolasDayvison! 