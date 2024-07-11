SQL

DDL

```sql
USE `Candidatura`;

DROP TABLE IF EXISTS `Curso`;
DROP TABLE IF EXISTS `Estudante`;
DROP TABLE IF EXISTS `Disciplina`;
DROP TABLE IF EXISTS `RequisitosDeAdmissão`;

CREATE TABLE IF NOT EXISTS `Curso` (
  `nome` varchar,
  `duração` int (3),
  `numerodevagas` int(9) ,
  `disciplina` FK
  `estudante` FK
  PRIMARY KEY (`nome`),
)


CREATE TABLE IF NOT EXISTS `disciplina` (
  `nome` varchar,
 PRIMARY KEY ( `BI`)
)

CREATE TABLE IF NOT EXISTS `RequisitosDeAdmissão` (
  `historico` Array,
  `valor` Decimal,
  `comprovativo` String ,
  `estudante` FK
 PRIMARY KEY ( `comprovativo`)
)
