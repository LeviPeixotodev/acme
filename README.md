# 📝 Anotações de Configuração:

Este repositório armazena as configurações fundamentais e boas práticas para o desenvolvimento do projeto.

## ⚙️ Arquivos de Configuração

### 📂 `.gitignore`
Utilizado para listar arquivos e diretórios que **não devem** ser rastreados pelo Git. Isso evita o envio de informações sensíveis ou arquivos desnecessários para o repositório remoto.
* **Conteúdos restritos:** Arquivos de variáveis de ambiente (ex: `.env`).
* **Pastas pesadas:** Dependências do projeto (ex: `node_modules/`).
* **Builds:** Pastas geradas automaticamente (ex: `.next/`).

### 🟢 `.nvmrc`
esta definindo a versão específica do **Node.js** exigida para o projeto. 
* **Uso:** Permite que desenvolvedores sincronizem o ambiente utilizando o comando `nvm use`.
* **Exemplo de conteúdo:** `20` (ou a versão LTS atual).

### 🛠️ `next.config.js` & Linting
Configurações globais do framework Next.js e padrões de qualidade de código:
* **ESLint:** No arquivo `.eslintrc.json`, utilizamos a extensão `next/core-web-vitals` para garantir que o código siga as melhores práticas de performance e melhorar tambem o **SEO**.

* **Prettier:** Atua como formatador de código, padronizando o estilo de escrita entre todos os colaboradores para manter a consistência do projeto.

---
### 📦 Gerenciamento de Dependências

No desenvolvimento deste projeto, utilizamos a separação entre dependências de produção e dependências de desenvolvimento.

#### `npm install -D` (ou `--save-dev`)
Este comando é utilizado para instalar pacotes que são necessários **apenas durante a fase de desenvolvimento**. 