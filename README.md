## a simple comment-api worker on cloudflare

- install tools, 也许后续新版不需要单独安装 beta 版 wrangler 

```
    npm install wrangler@d1
```

- create a empty project 

```
    npx wrangler@d1 init -y
```

- Make sure you've logged in

```
    npx wrangler login
```

- Create the D1 Database

```
    npx wrangler d1 create database-name
```

- Fill the DB with seed data from an SQL file

```
    wrangler d1 execute d1-example --file schema/schema.sql
```

- Install some dependencies

```
    npm install --save-dev @cloudflare/d1
```

- Deploy the worker

```
    wrangler publich
```