## 1 - Explique qual é a definição de MVC, MVVM e MVP

MVC (Model View Controller): Model fornece todos os dados, Controller gerencia qual View vai carregar e para onde vão os dados, View é a parte onde mostra os dados para usuário.

MVVM (Model View ViewModel): Model fornece os dados, View é a camada onde mostra os dados, ViewModel é a camada onde gerencia as regras de dados apresentados na View.

MVP (Model View Presenter): Model fornece os dados, View é a camada onde mostra os dados, Presenter é responsável por atualizar View quando Model é atualizado.

## 2 - Crie uma aplicação com um nome e um form onde os dados colocados neles sejam mostrados logo abaixo, formatados.

```html
<html ng-app="beMean">
<head>
    <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.5.5/angular.min.js"></script>
</head>

<body>
<form action="">
    <div>
        <label for="">Nome: <input type="text" ng-model="nome"></label>
    </div>
    <div>
        <label for="">E-mail: <input type="text" ng-model="email"></label>
    </div>
    <div>
        <label for="">Telefone: <input type="text" ng-model="telefone"></label>
    </div>

    <div>
        Nome: {{ nome }} <br>
        E-mail: {{ email }} <br>
        Telefone: {{ telefone }}
    </div>
</form>

<script>
    angular.module('beMean', [])
</script>
</body>
</html>
```