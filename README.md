Se o VS Code não está autocompletando seu código ao usar styled.div (ou outros componentes do styled-components), aqui estão os passos para fazer o autocomplete funcionar corretamente:

✅ 1. Instale as dependências corretas
Se estiver usando styled-components, certifique-se de que ele e os tipos estão instalados:


npm install styled-components
npm install --save-dev @types/styled-components

⚠️ Importante: Mesmo que esteja usando TypeScript, o auto-complete no JavaScript também pode melhorar com essas tipagens instaladas.

✅ 2. Configure o TypeScript corretamente (mesmo em JS)
Se estiver usando JavaScript, crie um arquivo jsconfig.json na raiz do seu projeto com:



{
  "compilerOptions": {
    "target": "es6",
    "module": "commonjs",
    "checkJs": true,
    "jsx": "react"
  },
  "include": ["src"]
}

Se for TypeScript, o tsconfig.json já deve cuidar disso.

✅ 3. Extensão recomendada:
Instale a extensão:

💡 vscode-styled-components

Link: https://marketplace.visualstudio.com/items?itemName=styled-components.vscode-styled-components

Essa extensão habilita:

Syntax Highlighting

AutoComplete

Linting

Jump to Definition

IntelliSense para CSS
