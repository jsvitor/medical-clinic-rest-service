# Sistema Web Clínica Médica

> Este sistema foi desenvolvido para posterior submissão avaliativa da disciplina de Introdução ao Armazenamento e Análise de Dados (IAAD) da Universidade Federal Rural de Pernambuco (UFRPE).
> O processo de desenvolvimento foi composto lançou mão de ferramentas de organização de projetos, teorias de arquitetura de software e conhecimentos de sistemas de banco de dados.

## Sobre o projeto
> Este repositório conta com o script SQL para criação e população do esquema relacional do banco de dados Clínica Médica, assim como o código fonte da API para interação com o banco de dados

### Ferramentas usadas
* VSCODE
* 

### Arquitetura
> Colocar um diagrama da arquitetura: MySQl → Web-Service→ Interface Web → Dispositivos do Usuário

## Como usar esse projeto

### Pré-requisitos

#### Para a execução do MySQL
* MySQL version xxx

#### Para execução do web service com NodeJS

* Node xx ou mais recente
* Yarn
* ...

#### Para execução da interface Web
* 

Se for usar o Docker Compose:
* Docker Engine XXX
* 



### Instalação

1. Clone o repositório
	`git clone https://github.com/jsvitor/medical-clinic`

	Você terá a seguinte estrutura de diretórios:


```
      .
      ├── data-base-scripts
      │   ├── clinica-medica-creation.sql
      │   └── clinica-medica-populate.sql
      ├── rest-service
      │   ├── src
      │   │    ├── config
      │   │    ├── controllers
      │   │    ├── doctorControllers
      │   │    |   ├── ...
      │   │    |   └── index.ts
      │   │    ├── routes          # rotas da aplicação
      │   │    │   ├── doctor.routes.ts
      │   │    │   ├── ...
      │   │    │   └── index.ts
      |   │    └── server.ts
      │   ├── .editorconfig
      │   ├── .eslintignore
      │   ├── .eslintrc.json
      │   ├── .gitattributes
      │   ├── .gitignore
      │   ├── README.md
      │   ├── .package.json
      │   ├── tsconfig.json
      │   └── yarn.lock
      │
      ├── web-interface             # SPA interface
      │   ├── index.ts
      │   ├── README.MD             # Getting started guide
      │   ├── src             
      │   └── ...                 
      └── ...
```


2. Execute o script para criação e população do banco de dados Clinica Médica. Cujo diagrama está representado abaixo:
	
	![esquema clínica médica](https://raw.githubusercontent.com/jsvitor/iaad-bsi-ufrpe/main/semana%2005-06/clinica_medica_diagram.png)

3. Após a criação e população do banco de dados clinica médica, é hora de executar a API.
	* Dentro do diretório 'web-service', execute:
		`yarn install`
	* Com as dependências instaladas, execute:
		`yarn dev`
	Agora você tem a API Rest funcionando no endereço `http://localhost:3333`

4. Agora chegou a hora de inicializar a interface web, para tal execute o comando: 
	* xxxxxxxxxxxx
		``
	* xxxxxxxxxxxx
		``

5. Agora basta acessar no seu navegador o endereço `http://localhost:port`



















OLD VERSION
***



# Clínica Médica

## Estrutura dos diretórios

      .
      ├── rest-service
      │   ├── src
      │   │    ├── config
      │   │    ├── controllers
      │   │    ├── doctorControllers
      │   │    |   ├── ...
      │   │    |   └── index.ts
      │   │    ├── routes          # rotas da aplicação
      │   │    │   ├── doctor.routes.ts
      │   │    │   ├── ...
      │   │    │   └── index.ts
      |   │    └── server.ts
      │   ├── .editorconfig
      │   ├── .eslintignore
      │   ├── .eslintrc.json
      │   ├── .gitattributes
      │   ├── .gitignore
      │   ├── README.md
      │   ├── .package.json
      │   ├── tsconfig.json
      │   └── yarn.lock
      │
      ├── web-interface             # SPA interface
      │   ├── index.ts
      │   ├── README.MD             # Getting started guide
      │   ├── src             
      │   └── ...                 
      └── ...


### Modelo Entidade Relacionamento Estendido | MySQL
![esquema clínica médica](https://raw.githubusercontent.com/jsvitor/iaad-bsi-ufrpe/main/semana%2005-06/clinica_medica_diagram.png)


## Funcionalidades da aplicação
- [ ] A escolha da linguagem de programação é livre (python, dart, java, php, javascript, entre outras), mas o BD deve ser o MySQL.

- [ ] O sistema deve contemplar as quatro operações básicas de CRUD (Create, Read, Update e Delete).

- [ ] Incluir no sistema pelo menos um trigger e um stored procedure. 

- [ ] Incluir no sistema no mínimo duas consultas, envolvendo junções, funções de agregação e agrupamentos. 

- [ ] O banco de dados deve estar populado.

- [ ] O sistema deve dispor de interface gráfica, seja web, mobile ou desktop.


## Tarefas

### Gravar o vídeo mostrando o funcionamento da aplicação

### Interface
- [ ] Protótipo no Figma

### Web service
- [ ] CRUD de medico
- [ ] CRUD de clinica
- [ ] CRUD de paciente
- [ ] CRUD de agendaConsulta
- [ ] CRUD clinicamedico

- [ ] Configuração do ambiente de desenvolvimento
- [ ] Criar as rotas para médico
- [ ] Fazer a conexão com o banco de dados mysql
- [ ] Documentar


## Medico

### Listar os 10 primeiros registros médicos

````GET```` ``/medico``


### Criar um registro de médico

```POST``` ``/medico``

``BODY``

````json
{
      "name": "Arlindo",
      "gender": "M",
      "phone": "81995374530",
      "email": "arlindo@hr.com",
      "codEspec": 3001
}
````


### Alterar um registro de médico usando o CodMed

```PUT``` ``/medico/:codmed``

#### Body

```json
{
      "name": "José"
}
```


### Deletar um registro de Médico

```DELETE``` ```/medico/:codmed```

## Clinica




## Paciente

## AgendaConsulta

## ClinicaMedico


