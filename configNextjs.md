# Eslint
## eslintrc.json
```
{
  "plugins": [
    "@typescript-eslint"
  ],
  "extends": [
    "next/core-web-vitals",
    "plugin:@typescript-eslint/recommended",
    "prettier"
  ],
  "rules": {
    "@typescript-eslint/no-unused-vars": "error",
    "@typescript-eslint/no-explicit-any": "error"
  }
}
```
# Prettier
Installing:
```
yarn add --dev --exact prettier
```
Creating prettier config:
```
echo {}> .prettierrc.json
```
Creating prettierignore:
```
echo {}> .prettierignore
```
Add on prettierignore:
```
build
coverage
```
Format all files:
```
yarn prettier . --write
```
## prettierrc.json
```
{
    "semi": true,
    "trailingComma": "es5",
    "singleQuote": false,
    "tabWidth": 2,
    "useTabs": true
}
```
