• Criar uma pasta chamada "src" e dentro dela criar o "index.ts"

• Comando para iniciar um projeto node: npm init

• Instalar o TypeScript no projeto: npm install -g typescript

• Criar arquivo de configuração do TypeScript: tsc --init (será criado um arquivo tsconfig.json, um arquivo de configuração do TypeScript)

• Abrir o arquivo tsconfig.json

• Deixar ("moduleResolution": "node" e "rootDir": "./src") descomentados

• Atribuir "src" dentro de "./":
"rootDir": "./src"

• Descomentar "outDir": "./" e escrever o diretorio "dist" dentro de "./":
"outDir": "./dist"

• Em seguida vamos instalar a biblioteca: 
npm install --save-dev @types/node

• Instalar o nodemon:
npm install nodemon

• Em seguida: 
npm install -D ts-node

• Acessar o package.json, abaixo de "test"(linha 8), criar o "start-dev":
"test": "echo \"Error: no test specified\" && exit 1",
    "start-dev": "nodemon src/index.ts"

• Depois, o comando:
npm run start-dev

Lembrando que para usar o comando "npm run start-dev", o arquivo "index.ts" deverá possuir algum comando a ser executado, exemplo:

var name: string = "Vinicius"
var age: number = 17

console.log(`My name is ${name} and i'm ${age} years old`);

