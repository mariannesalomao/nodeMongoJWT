# SCRIPTS SHELL - Ir devagar e ensinar POSTMAN!

```shell
npm install bcrypt dotenv express jsonwebtoken mongoose

npm install --save-dev nodemon
```

### Package.json

```json
{
  "scripts": {
    "start": "nodemon app.js"
  }
}
```

> Bcrypt pega a senha que vc digita cru ali e transforma num hash.

> Dotenv pra gente ter um arquivo de configuração na máquina, a ideia é não versionar esse arquivo

> Jsonweb token é pra manusear o token, verificar se o token do usuário é válido

- Criar arquivo `.gitignore` e `.env`


# POSTMAN

> Seta a URL e mais tarde o TOKEN gerado como variáveis (URL - TOKEN)

- Rota POST REGISTRO: {{URL}}/auth/register

- Body do Post:

```json
{
    "name": "Marianne",
    "email": "marianne@gmail.com",
    "password": "123456",
    "confirmPassword": "123456"
}
```

----------------------------

- Rota POST LOGIN: {{URL}}/auth/login

- Body do Post:

```json
{
  "email": "marianne@gmail.com",
  "password": "123456"
}
```

-------------------------------------

- Rota GET PRIVADA: {{URL}}/user/62a38ffc2b6a6573ce5f0e9d

- Authorization coloca Bearer Token
