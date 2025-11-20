projeto java + sql server
========================

estrutura:
- src/app/Models.java        (entidades do dominio)
- src/app/Daos.java          (connection factory e daos)
- src/app/CadastroService.java
- src/app/CadastroController.java
- src/app/TelaCadastro.java
- src/app/Main.java
- database_sqlserver.sql     (script para criar o banco no sql server)
- diagrama: /mnt/data/diagrama_sequencia_cadastro.pdf.png

instrucoes:
1) coloque o driver jdbc do sql server no classpath (microsoft jdbc driver).
   exemplo: mssql-jdbc.jar
2) ajuste usuario e senha no arquivo Daos.java (constantes USER e PASS).
3) crie o banco usando o script database_sqlserver.sql (veja abaixo).
4) compile: javac -d out src/app/*.java
5) execute: java -cp out;path/to/mssql-jdbc.jar app.Main   (windows)
   ou: java -cp out:path/to/mssql-jdbc.jar app.Main        (linux/mac)

obs: o caminho do diagrama respondido pelo usuario esta em:
/mnt/data/diagrama_sequencia_cadastro.pdf.png
