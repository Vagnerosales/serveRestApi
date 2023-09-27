# Teste de API
teste de API Rest do manual ao CI/CD

## O que é
Este repositórioi foi criado para estudos de teste de API Rest.

## Tecnologias utilizadas
Postman
node version v18.17.0
Newman version v6.0.0
Newman-reporter-html

## Documentações 
- Analise Técnica: 
- Doc da API: [Consulte Swagger](https://serverest.dev/#/Usu%C3%A1rios/put_usuarios___id_)
  
## Como instalar o ambiente 

- Primeiro: instale o node em seu computador [baixe aqui](https://nodejs.org/en/download)
- Segundo: realize a instalação do newman de forma global [baixe aqui a dependencia](https://www.npmjs.com/package/newman)
```
npm install -g newman
```
- Terceiro: realize a instalação da dependencia dos relatórios (opcional) [newman-reporter-html](https://www.npmjs.com/package/newman-reporter-html)

## Como rodar os testes

### Pelo Postman web ou desktop
-Import a collection e o environment
-Execute os teste de forma manual ou automatizada

### Pelo newman
-Abra o console e execute a seguinte linha de comando para rodar os testes
```
newman run ServeRest.postman_collection.json -e ServeRestEnvi.postman_environment.json -r cli
```
- Execute os testes com relatório
```
newman run ServeRest.postman_collection.json -e ServeRestEnvi.postman_environment.json -r cli,htmlextra
```
### Report 

Se você optou por rodar os testes com o report htmlextra, você gerou um arquivo html com o resultado dos testes e para verificar as validações você pode abrir a pasta **newman** que foi criada no local em que os arquivos de collection e environment se encontram.

## Entre em contato

vagnerosales@gmail.com


