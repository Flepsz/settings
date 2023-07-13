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
## prettierrc.json
```
{
    "semi": true,
    "trailingComma": "es5",
    "singleQuote": false,
    "tabWidth": 4,
    "useTabs": true
}
```
