# React + TypeScript + Vite 学习项目


## 一些依赖版本/环境参考

> - react 19.2
> - typescript 6.0
> - vite 8.3

> - node 24.15.0
> - npm 管理依赖
> - windows 11

## 补充说明

### 补充1
`eslint-plugin-prettier` 依赖。
可以把 `Prettier` 的格式化能力包装成标准 `ESLint` 规则，并且 `--fix` 命令可以集成自动格式化的能力。效果类似 `eslint ./src --fix && prettier ./src --write`。
```js
'prettier/prettier': 'warn', // 不能是 'off'，才能生效
```

PS: 若检查时不想打印可能存在的 `Prettier` 规则信息(太多，影响查看别的)。可以使用命令行参数，临时覆盖对应规则，生成本次的打印结果。不影响 `--fix` 命令的自动格式化。
```bash
# 例如 npm run lint2
"lint2": "eslint ./src --rule {\\\"prettier/prettier\\\":off}"
```
