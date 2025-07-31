## Descrição

Aplicação back-end com NestJS, TypeORM e Typescript.

## Instalação e execução

### Com Docker

```bash
$ docker-compose up -d --build
```

### Sem Docker

```bash
# Instalar dependencias
$ npm install

# Desenvolvimento
$ npm run start

# Desenvolvimento (Watch Mode)
$ npm run start:dev

# Produção
$ npm run start:prod
```

## Criando e executando migrações

```bash
# Executar migrações pendentes
$ npm run migration:run

# Criar novas migrações com base nas mudanças nas entidades
$ npm run migration:generate -name=NOME_DA_MIGRATION

# Criar novas migrações sem nenhum conteúdo
$ npm run migration:generate:clear -name=NOME_DA_MIGRATION

# Revertar última migração executada
$ npm run migration:revert
```

## Criando e executando seeds

```bash
# Executar seeds pendentes
$ npm run seed:run

# Criar novas seeds
$ npm run seed:create -name=NOME_DA_SEED
```

## Configurações de VSCode recomendadas:

```json

"editor.formatOnSave": true,
"prettier.requireConfig": true,
"editor.codeActionsOnSave": {
  "source.fixAll.eslint": true
}

```
