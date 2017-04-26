## Repositorio para Atividades

**Disciplina**

Programação para Web 2017-1

**Link para repositorio**

https://github.com/THYERESNAHUM/PW2017-calculaimc.git

**Procedimento para clonar o repositorio**
```
git clone https://github.com/THYERESNAHUM/PW2017-calculaimc.git
```
**Comando para executar o servidor Tomcat**

* Se possuir maven instalado
```
mvn org.apache.tomcat.maven:tomcat7-maven-plugin:run
```

* Se não possuir maven instalado

```
mvnw org.apache.tomcat.maven:tomcat7-maven-plugin:run
```

**Para Acessar Calculadora**

http://localhost:9090/calculaimc em qualquer navegador.

Caso esteja clonando o repositorio no Linux, use ./mvnw ao invés de apenas mvnw, como no Windows. Além disso, pelo menos uma vez, é preciso dar permissão de execução ao arquivo de script mvnw com o comando chmod +x mvnw.


**Para "empacotar" a aplicação**

* Se possuir maven instalado
```
mvn package
```

* Se não possuir maven instalado
```
mvnw package
```
**Obs:**

O arquivo .gitignore contem as exceções(dir target) que não são enviadas para esse repositorio.

**Caso queira compactar o pacote para executar em maquinas sem maven instalado.**
```
mvn io.takari:maven:0.3.3:wrapper -Dmaven=3.3.9
```
