# Meu primeiro projeto em AngularJS

Esse é um exemplo de um input que utilizamos AngularJS para mostrar o quanto é simples utilizar esse framework.

Esse projeto contém uma pasta chamada projeto1, dentro da mesma nós temos uma outra pasta chamada lib, onde colocamos o nosso framework AngularJS.

Temos também dois arquivos, o index.html que é o da tela inicial do nosso projeto que contém o seguinte código:

~~~html
<!doctype html>
<html ng-app="Projeto1">
	<head>
		<title>Título da sua página</title>
	</head>
	<body ng-controller="PrimeiraController">
		<input type="text" ng-model="mensagem" /> <br />
		{{mensagem}}

		<script src="lib/angular.min.js"></script>
		<script src="main.js"></script>
	</body>
</html>
~~~

E também tem a configuração desse pequeno exemplo que é o main.js que tem o seguinte código:

~~~javascript
//projeto1/main.js
var app = angular.module('Projeto1',[]);
app.controller('PrimeiraController', function($scope) {
	$scope.mensagem = "Olá, esse é o meu primeiro projeto em AngularJS";
});
~~~

Continue acompanhando a apostila e respondendo os excercícios para que objtenha o melhor aprendizado possível.
