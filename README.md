# MiProyecto

Proyecto ESM con ESLint y Prettier configurados.

## Scripts

- `start`: inicia la app (`node src/index.js`).
- `lint`: corre ESLint sobre el repo.
- `format`: formatea el código con Prettier (modo write).

## Uso

1. Instalar dependencias:
   - npm: `npm install`
   - pnpm: `pnpm install`
   - yarn: `yarn`

2. Lint:
   - `npm run lint`

3. Formateo:
   - `npm run format`

## Configuración

- `.eslintrc.json`:
  - `env` para Node y ES2022.
  - `sourceType: "module"` para ESM.
  - `extends: ["eslint:recommended", "plugin:prettier/recommended"]` integra Prettier para evitar reglas en conflicto.
  - Reglas suaves: `no-unused-vars` como warning e ignora argumentos/vars con prefijo `_`.

- `.prettierrc`:
  - Comillas simples, `semi: true`, `trailingComma: "es5"`, ancho 100, `tabWidth: 2`, `arrowParens: "always"`.

Si faltara algún paquete (por ejemplo `eslint`, `prettier` o `eslint-plugin-prettier`/`eslint-config-prettier`), instalalos según tu gestor.
