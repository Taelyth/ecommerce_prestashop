# Testes — Appium
Projeto criado para acompanhar as aulas do curso [Formação em Teste de Software][Iterasys] em **Java** utilizando **Junit, Selenium e Cucumber**.
A organização dos testes foi feita em **Page Object**, e também foi utilizado um CSV como massa de testes em um dos exemplo.

Para o teste foi utilizado um link de demonstração de um e-commerce simples.

---

### Pré-Requisitos
- Nesse projeto utilizamos o **Pom — Maven** com as seguintes versões das bibliotecas:

```java
<junit.version>5.7.2</junit.version>
<hamcrest.version>2.2</hamcrest.version>
<selenium.version>3.141.59</selenium.version>
<cucumber.version>6.10.4</cucumber.version>
```

- A URL utilizada para os testes é um e-commerce de demonstração: [Link][Prestashop]
- Para rodar os testes web é necessário adicionar o `chromedriver` no seguinte local: `C:\\webdrivers\chromedriver\{versão}\chromedriver.exe`
- Colocar a `{versão}` desejada e alterar no código [BaseTests.java](src/test/java/base/BaseTests.java).

---

### Glossário

`pages` Pacote contendo as classes de cada uma das páginas testadas, seus elementos e ações realizadas.

`util` Pacote contendo métodos reutilizados nos testes.

`BaseTests.java` Classe com o Setup e Teardown dos testes e código de tirar screenshot.

`HomePageTests.java` Código com os testes realizados.

`Runner.java` Código de exemplo de um Runner em Cucumber.

`steps` Pacote contendo os passos implementados do arquivo [comprar_produto.feature](src/test/resources/features/comprar_produto.feature)

`massaTeste_Login.csv` Massa de testes usada no arquivo [HomePageTests.java](src/test/java/homepage/HomePageTests.java)

---

### Créditos
[<img src="assets\Iterasys-Logo.png" width="20%"/>][Iterasys]


<!-- links -->
[Iterasys]: https://iterasys.com.br/
[Prestashop]: https://marcelodebittencourt.com/demoprestashop/

<!-- imagens -->
[Iterasys-Logo]: assets/Iterasys-Logo.png (Iterasys-logo)