# 🌱 AgroCitro

Sistema web para gerenciamento agrícola com foco em **plantio, irrigação e colheita**.  
O projeto foi desenvolvido utilizando **Node.js**, **JavaScript**, **HTML/CSS** e **SQL** para banco de dados.  

---

## 📋 Pré-requisitos

Antes de iniciar, você precisará ter instalado em sua máquina:

- [Node.js](https://nodejs.org/) (versão LTS recomendada)
- [npm](https://www.npmjs.com/) (já incluso no Node.js)
- Banco de dados MySQL ou MariaDB
- Git (opcional, para versionamento)

---

## ⚙️ Configuração do Projeto

1. **Clonar o repositório**
   ```bash
   git clone https://github.com/seu-repositorio/AgroCitro.git
   cd AgroCitro
   ```

2. **Instalar dependências**
   Existem dependências em duas pastas (`/js` e `/database`).  
   Execute o comando dentro de cada uma delas:
   ```bash
   cd js
   npm install

   cd ../database
   npm install
   ```

3. **Configuração do Banco de Dados**
   - Crie um banco de dados MySQL.
   - Importe os scripts SQL localizados em:
     - `database/AgroCitro_Banco (2).sql`
     - `database/database_login.sql`

   ```sql
   SOURCE database/AgroCitro_Banco (2).sql;
   SOURCE database/database_login.sql;
   ```

4. **Variáveis de Ambiente**
   Crie um arquivo `.env` na raiz do projeto com as seguintes informações:

   ```env
   DB_HOST=localhost
   DB_USER=seu_usuario
   DB_PASSWORD=sua_senha
   DB_NAME=agrocitro
   PORT=3000
   ```

---

## 🚀 Execução do Projeto

1. Entre na pasta `js`:
   ```bash
   cd js
   ```

2. Inicie o servidor:
   ```bash
   node index.js
   ```
   ou, se preferir, use o nodemon (caso instalado globalmente):
   ```bash
   nodemon index.js
   ```

3. Acesse no navegador:
   ```
   http://localhost:3000
   ```

---

## 🧪 Testes e Validação

Atualmente, o projeto não possui testes automatizados configurados.  
A validação do funcionamento pode ser feita da seguinte forma:

1. Subir o servidor com `node index.js`.
2. Acessar as páginas do frontend:
   - `public/index.html` → Tela inicial
   - `public/cadastrar.html` → Cadastro
   - `public/plantio.html` → Gestão do plantio
   - `public/irrigacao.html` → Gestão da irrigação
   - `public/colheita.html` → Gestão da colheita

3. Confirmar se as interações estão salvando corretamente no banco de dados.

---

## 👥 Integrantes do Grupo

- Guilherme  
- Tiago  
- Ana Julia  
- Lucas  

---

