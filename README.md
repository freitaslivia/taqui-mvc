
![Logo](https://i.ibb.co/28CdGFY/BANNER-TAQUI.png)

# Documentação TAQUI USUÁRIOS

Primeiro deve ter instalado na sua maquina java 17 e o gradle(tutorial de como instalar o gradle: https://www.youtube.com/watch?v=R5MwoMsnh2E )

1 - Adicionamos no arquivo build.gradle o plugin do azure:
```
plugins {
    id "com.microsoft.azure.azurewebapp" version "1.1.0"
}     
```
vai ficar assim:

```
plugins {
	id 'java'
	id 'org.springframework.boot' version '3.3.3'
	id 'io.spring.dependency-management' version '1.1.6'
	id "com.microsoft.azure.azurewebapp" version "1.10.0"


}
```
2 - Adicionamos  no arquivo build.gradle a configuração do  plugin do azure:
```
azurewebapp {
	subscription = '77473478-7b1d-4345-95f9-5d7f456d8c84'
	resourceGroup = 'rgsprint3'
	appName = 'sprint3java'
	pricingTier = 'F1'
	region = 'brazilsouth'
	runtime {
		os = 'Windows'
		webContainer = 'Java SE'
		javaVersion = 'Java 17'
	}
}

```

3 - No cmd navegue até o projeto e rode esse comando:
```
gradle azureWebAppDeploy
```
fonte: https://devblogs.microsoft.com/java/gradle-deploy-java-web-apps-to-azure-in-one-step/



---------------------------------------
 ## Instruções de testes:



 No sistema temos essas url:

  - Home : https://sprint3java.azurewebsites.net/template
  - Lista de Usuarios : https://sprint3java.azurewebsites.net/listaUsuariosTemplate
  - Lista de Produtos: https://sprint3java.azurewebsites.net/listaProdutosTemplate
  - Cadastrar Usuarios: https://sprint3java.azurewebsites.net/cadastroUsuario
  - Cadastrar Produtos: https://sprint3java.azurewebsites.net/cadastroProduto

 No sistema podemos deletar, cadastrar, editar e ver a lista de produtos e Usuarios

Campos obrigatórios: *

Cadastro e Edição de usúario:

Nome* - O campo não pode estar vazio e deve ter no máximo 50 carácteres.

Senha*- Não pode estar vazio, deve ter no minimo 12 e maximo de 15 caracteres e conter pelo menos um caractere especial e uma letra maiúscula.

Email* - O campo não pode estar vazio, deve ter no máximo 50 carácteres e deve ser um email com @.

<a href="https://ibb.co/zHctKNL"><img src="https://i.ibb.co/2Y2pX5L/cadastro-usuario.png" alt="cadastro-usuario"/></a>

Cadastro e Edição de produto: 

Deve ter um usúario cadastro para poder cadastrar um produto.

Nome* - O campo não pode estar vazio e deve ter no máximo 50 carácteres.

Descrição* - O campo não pode estar vazio e deve ter no máximo 50 carácteres.

Preço* - O campo não pode estar nulo.

Id do úsuario* - Deve ser o mesmo id que já tem cadastrado na lista de usuários

<a href="https://ibb.co/qppjWT8"><img src="https://i.ibb.co/qppjWT8/cadastro-produto.jpg" alt="cadastro-produto" border="0" /></a>

Ao deletar um usuário, os produtos vinculados a ele são excluídos automaticamente.

Ao editar um usuário não deve deixar nenhum campo vazio.

Lista de Produto:

<a href="https://ibb.co/f4WmtkZ"><img src="https://i.ibb.co/f4WmtkZ/lista-produto.png" alt="lista-produto" border="0" /></a>


Lista de Usuários:
<a href="https://ibb.co/CwsZx5J"><img src="https://i.ibb.co/CwsZx5J/lista-usuario.png" alt="lista-usuario" border="0" /></a>
------------------------------------------------------------------------
Aquitetura de JAVA:

<a href="https://ibb.co/bsLjGDX"><img src="https://i.ibb.co/bsLjGDX/arquitetura-do-projeto.png" alt="arquitetura-do-projeto" border="0" /></a>

---------------------------------------

Rodando o projeto na própria maquina

 No sistema temos essas url:

  - Home : http://localhost:8080/template
  - Lista de Usuarios : http://localhost:8080/listaUsuariosTemplate
  - Lista de Produtos: http://localhost:8080/listaProdutosTemplate
  - Cadastrar Usuarios: http://localhost:8080/cadastroUsuario
  - Cadastrar Produtos: http://localhost:8080/cadastroProduto

---------------------------------------------------


## Integrantes
:small_blue_diamond:Gabriel Sampaio
IOT, C#
RM 552342		
<a href="https://www.linkedin.com/in/gabrielsampaiogianini/">Linkedin</a>
<a href="https://github.com/gabrielsampaiog">Github</a>

:small_blue_diamond:Gabriel Neves
Mobile, IOT
RM 552244
<a href="https://www.linkedin.com/in/-gabriel-neves/">Linkedin</a>
<a href="https://github.com/Neveszera">Github</a>

:small_blue_diamond:Livia Freitas
Java, QA, IOT
RM 99892
<a href="https://www.linkedin.com/in/l%C3%ADvia-freitas-ferreira/">Linkedin</a>
<a href="https://github.com/freitaslivia">Github</a>

:small_blue_diamond:Rafael Mendonça
Database, IOT
RM 552422
<a href="https://www.linkedin.com/in/rafael-henrique-de-mendon%C3%A7a-51263326b/">Linkedin</a>
<a href="https://github.com/rhmendonca">Github</a>

:small_blue_diamond:Renato Romeu
DevOps, Mobile, QA, IOT
RM 551325
<a href="https://www.linkedin.com/in/renato-russano-706423a3/">Linkedin</a>
<a href="https://github.com/RenatoRussano">Github</a>
