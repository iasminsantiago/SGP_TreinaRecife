# SGP_TreinaRecife
Projeto full stack de gerenciador de projetos por usuário, usando Java + React e JS + React.






# SGP - NOTAS

## Termos

Spring - framework para produtividade

Maven - gerencia as **dependências**, informo-as no arquivo e o Maven entende

# Criando o projeto

- Usando o spring initializr (cntl shift P - spring initialzr: Create a Maven project), escolheremos as configurações
    - versão do spring boot
    - nome do pacote (ex.: br.com.sitedoprojeto)
    - nome do projeto (ex.: demo-springboot)
    - jar
    - versão do Java
    - **dependências** base [1]
    - 


Informaçoes úteis:
http://localhost:8080/h2-console
Porta - 
JDBC URL: 
Login: sa
Senha: sa

#### [1] Dependências

Spring web - permite criarmos uma app web

Spring data - permite interagirmos com banco de dados, podemos usar JDBC ou JPA

H2 - Se comunica com o banco de dados, é o driver do banco, H@ é um banco simples de utilizar

DevTools - dependência que permite termos rápidos restarts no projeto

#### Execução do código
-- O que acontece se clicar direto em Run, sem extensão Maven no VS CODE
Não clicar em Run no VS Code pois isso roda pelo javac puro, que não conhece as dependências do Spring. 
Projeto Spring Boot precisa ser rodado pelo Maven ou pela própria IDE, não diretamente pelo terminal assim.
Por isso, usamos mvnw spring-boot:run

-- Porque o comando mvnw.. não deu certo mas mvn deu certo:
mvnw — é o Maven "embutido" no projeto (Maven Wrapper). Às vezes não funciona no Windows por causa de permissão ou porque o arquivo não foi gerado corretamente.
mvn — é o Maven instalado na minha  máquina. Como funcionou, significa que tenho o Maven instalado globalmente, o que é ótimo.
