# blog-api

API para estudo de testes de API.

Passos para executar a API:

1. Execute o comando `npm i` ou `yarn`
2. Execute o comando `yarn start` ou `npm start`

Após executar a API, é possível acessar a documentação por meio da url:

```
http://localhost:3000/docs
```

Obs: Os testes contidos no arquivo a seguir, contenplam apenas um fração mínima das resquisições de testes que a documentação proporciona.


O arquivo `test_api_blog_endpoints.postman_collection.json`, contém os testes reailizados atrvés do Postman.

Para executar o arquivo:

1. Abra o Postman.
2. Em sua workspace, clik em `import`, logo será aberta uma nova janela com a opção `file`, pré-fixada.
3. Click em `choose files`, e selecione o arquivo dentro da pasta em seu diretório. 

A pasta Newman, contém o relátorio html com os dados dos testes realizados.

Para instalar e excutar os testes com o Newmam:

1. Abra o seu `Terminal/Prompt de comando` Power Shell.
2. No terminal, execute o comando, `npm install -g newman`, tecle `enter` e aguarde a instalação
3. Agora execute o comando, ` newman run "caminho do arquivo Json" `, tecle `enter` aguarde a execução dos testes
4. Para rodar os testes mais que 1 vez, execute o camando da linha 3, acrescido de `--iteration-count "n° de vezes que deseja rodar os tests`

Para gerar o relatório HTML, através do Newman:

1. Abra um novo terminal, execute o comando: `npm install -g newman-reporter-htmlextra`, aguarde a instalção
2. Agora execute o comando `newman run collection.json -r htmlextra`, o mesmo, criará um novo relatório no ./newmandiretório, se o diretório não existir, ele será criado como parte da execução do Newman.

