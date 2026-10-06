# Publicar deck MV no GitHub Pages

Arquivo: `index.html` (deck "Cadastro de novo produto no Salesforce", HTML único, offline, sem dependências).

## Prompt para o Claude Code

Cole isto no Claude Code, dentro desta pasta:

```
Publique esta pasta no GitHub Pages:
1. git init, commit do index.html e deste README
2. Crie o repositório público "projeto-mv" na minha conta (gh repo create projeto-mv --public --source=. --push)
3. Ative o GitHub Pages na branch main, pasta raiz (gh api -X POST repos/{owner}/projeto-mv/pages -f "source[branch]=main" -f "source[path]=/")
4. Aguarde o deploy e me devolva a URL final (https://<usuario>.github.io/projeto-mv/)
```

Requisitos: `git` e GitHub CLI (`gh`) logado (`gh auth login`).

## Atualizar depois
Substitua o `index.html` pela nova versão e rode: `git commit -am "atualiza deck" && git push`.
