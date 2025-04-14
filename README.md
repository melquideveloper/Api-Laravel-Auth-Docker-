
<p align="center">
  <img src="https://github.com/user-attachments/assets/bde9e4c8-70a1-46a3-ac5f-d05d3ed93477" alt="Codificando..." />
</p>

# 👋 Hello, let's connect this technical repository to new opportunities!

   ## Este repositório apresenta uma API moderna, robustas, segura e escalável desenvolvida com Laravel.
   
   ## By software engineer Melquisedeque Bispo de Jesus
   
     Principais recursos:

    🔐 Autenticação com JWT

    🗄️ Banco de dados PostgreSQL

    🐳 Up do servidor sendo pelo Docker ou execução via Artisan

    📊 Exportação de dados em Excel (disponível após login)

    🌱 Migrations + Seeders configurados para facilitar testes e replicação do ambiente

📍 Documentação.pdf, Localizada na raiz do projeto nela contém:

    🧭 Mapa dos Endpoints

    🔐 Instruções de como realizar testes das rotas com JWT (como gerar e utilizar o token)

    🧱 Diagrama do Banco de Dados   

    ⚙️ Organização e estrutura da aplicação

🚀 Como rodar o projeto localmente
## 1️⃣ Clone o projeto

    -git clone https://github.com/melquideveloper/Api-Laravel-Auth-Docker-.git
    -cd Api-Laravel-Auth-Docker-\

## 2️⃣ Instale as dependências Laravel

    -cp .env.example .env
    -composer install
    -php artisan key:generate
    -php artisan jwt:secret

## 3️⃣ Configure o banco de dados (PostgreSQL)

    -No arquivo .env, configure com os dados do seu PostgreSQL
      Certifique que você criou o banco no seu SGBD

    -Se precisar testar na sua aplicação a conexão com banco de dados foi bem sucedida, siga esse passo no terminal:
      php artisan tinker
      DB::connection()->getPdo();
      exit

    -Rode as migrações:
      php artisan migrate:refresh

    -Popular o banco:
      php artisan db:seed

    -Resumo e linguagem menos verbosa
      php artisan migrate:fresh --seed

## 4️⃣ Deseja Subir o Servidor com Docker?

   - Certifique-se de que a porta 5432 esteja livre (PostgreSQL)

    Arquivos Docker já prontos e configurados: 📁
    ├──docker-compose.yml 
    ├──/dockerfiles 
    
    Execute 🧑‍💻 
     -docker compose up -d

## 5️⃣ Deseja Subir o Servidor com Laravel Artisan?
    
    -php artisan serve 
    -php artisan serve --host=seu_ip --port=9090 (Ser preferir Acesso Em toda Rede Local)

## 6️⃣ Teste os endpoints via Insomnia / Postman

   - 📍 Veja todos os endpoints no PDF da Documentação.pdf.
   - ✅ Com exemplos de requisições e headers.

## 7️⃣ Interface bônus! Simples para Login e carga de dados Excel 🎁

   - Acesse após subir o servidor no navegador:
   - http://127.0.0.1:8000
   
   - Você verá a seguinte interface
     
  
<p align="center">
  <img src="https://github.com/user-attachments/assets/b4c8adb5-74e2-4f2c-83b0-bc636156fe7f" alt="Codificando..." style="border-radius: 30px;"/>
</p>

## 🧠 Principais Tecnologias

    -Laravel Framework 8.83.27

    -PHP 8.0.13

    -PostgreSQL

    -JWT (tymon/jwt-auth)

    -Docker / Docker Compose

    -Insomnia para testes

- ✅ Maiores dúvidas consulte o arquivo Documentação.pdf além do passo a passo orientados aqui.

## 📄 Licença

- Codificação do projeto: UTF-8
 
- Este projeto utiliza a licença MIT.
