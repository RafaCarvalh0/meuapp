# [Meuapp]

![Licença](https://img.shields.io/badge/licença-MIT-blue.svg)
![Status](https://img.shields.io/badge/status-em%20desenvolvimento-yellow.svg)

> projeto base com Laravel


## 🛠️ Tecnologias Utilizadas

* **Backend:**
    * [PHP 8.2](https://www.php.net/)
    * [Laravel 10](https://laravel.com/)
    * [MySQL](https://www.mysql.com/)
* **Frontend:**
    * [Blade](https://laravel.com/docs/10.x/blade)
    * [Tailwind CSS](https://tailwindcss.com/)
    * [JavaScript](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript)
* **Ambiente de Desenvolvimento:**
    * [Docker](https://www.docker.com/)
    * [VS Code](https://code.visualstudio.com/)

---

## 🚀 Como Começar

Siga estas instruções para obter uma cópia do projeto em funcionamento na sua máquina local para desenvolvimento e testes.

### Instalação

Siga o passo a passo abaixo para instalar o projeto:

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/RafaCarvalh0/meuapp.git
    ```

2.  **Acesse a pasta do projeto:**
    ```bash
    cd meuapp
    ```

3.  **Instale as dependências do PHP:**
    ```bash
    composer install
    ```

4.  **Instale as dependências do JavaScript:**
    ```bash
    npm install
    ```

5.  **Configure o arquivo de ambiente:**
    * Copie o arquivo de exemplo `.env.example` para `.env`.
    ```bash
    cp .env.example .env
    ```
    * Abra o arquivo `.env` e configure suas variáveis de ambiente, especialmente a conexão com o banco de dados (`DB_DATABASE`, `DB_USERNAME`, `DB_PASSWORD`).

6.  **Gere a chave da aplicação:**
    ```bash
    php artisan key:generate
    ```

7.  **Execute as migrações do banco de dados:**
    * Isso criará todas as tabelas necessárias no seu banco de dados.
    ```bash
    php artisan migrate
    ```

8.  **(Opcional) Popule o banco de dados com dados de teste:**
    ```bash
    php artisan db:seed
    ```

---

## 💻 Uso

Após a instalação, você pode iniciar o servidor de desenvolvimento.

1.  **Inicie o servidor local:**
    ```bash
    php artisan serve
    ```

2.  **Compile os assets do frontend (se necessário):**
    ```bash
    npm run dev
    ```

3.  Abra seu navegador e acesse [http://127.0.0.1:8000](http://127.0.0.1:8000) para ver a aplicação.

**Exemplo de login:**
    ```bash
    php artisan tinker
    ```
    ```bash
    App\Models\User::create(['name' => 'Seu Nome', 'email' => 'email@exemplo.com', 'password' => bcrypt('senha')])
    ```
* **Usuário:** `email@exemplo.com`
* **Senha:** `senha`

