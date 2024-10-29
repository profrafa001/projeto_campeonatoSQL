# Banco de Dados
<p align = "justify">Trabalho apresentado à professora Rafaela Pessin, da disciplina Banco de Dados da EEEFM Professor Joaquim Barbosa Quitiba, inclusa no Campeonato de SQL, uma estratégia envolvendo gamificação e protagonismo.
 Os alunos tiveram todos os conceitos de banco de dados, desde conceitos base até a modelagem de dados. Este trabalho tem o objetivo implementar uma banco de dados usando a Linguagem de Consulta Estruturada SQL.

## Turmas Participantes
* 2º IPI 01
* 2º IPI 02
* 2º RDC 01
* 3º MSI 01
 
## Fases do Campeonato
### Fase 1: Competição por turmas
* As turmas serão divididas em grupos de 5 a 6 alunos. 
* Os grupos irão competir entre si.
* Nesta etapa, estarão competindo 22 grupos (somatório dos grupos das 4 turmas).
* Na Fase 1 da competição serão consideradas as seguintes etapas do trabalhos: ETAPA 1 - Criação do Banco de Dados, ETAPA 2 - Documentação do Banco de Dados e ETAPA 3 - Refinamento.
* Essas etapas serão realizadas durante as aulas de Banco de Dados, nas aulas práticas de Laboratório de Informática.
* Serão considerados alguns critérios de avaliação como: cumprimento de todas as etapas completas, qualidade de implementação e documentação e participação dos integrantes.
* Cada turma terá os 1ºs, 2ºs e 3ºs lugares ganhadores, com direito a premiação (medalha) para todos os integrantes dos grupos.
* Os 1ºs lugares de cada turma, vão para a etapa seguinte.

### Fase 2: Competição interclasse
* Nesta etapa, irão participar apenas 4 grupos, ou seja, os 1ºs colocados de cada turma da Fase 1 da competição.
* Na Fase 2 da competição será considerada a seguinte etapa do trabalho: ETAPA 4 - Consulta ao Banco de Dados.
* Essa etapa será em um dia e horário atípico, envolvendo todos os quatro grupos no Laboratório de Informática.
* Nesta fase do campeonato, será dado um tempo e um desafio para que os grupos solucionem.
* Serão considerados alguns critérios de avaliação como: cumprimento da etapa completa, utilização do tempo disponibilizado, qualidade de implementação e participação dos integrantes.
* A competição terá os 1ºs, 2ºs e 3ºs lugeres (com premiação a definir).

# Grupos Participantes 

[Grupos.xlsx](https://github.com/user-attachments/files/17549939/Grupos.xlsx)

# Integrantes do Grupo
1) 
2) 
3) 
4) 
5) 

# Modelo Lógico
* Abaixo você pode visualizar o modelo lógico do trabalho.
  
![modelo logico](https://github.com/user-attachments/assets/a027b355-aa7e-44de-861a-3fad13985b6c)

# ETAPA 1 - Criação das Tabelas do Banco de Dados
* Analise o Modelo Lógico e crie as tabelas do banco de dados (CREATE).
* Crie todas as tabelas do modelo lógico usando os tipos de dados adequados.
* Utilize a ferramenta a seguir para esta tarefa: https://sqliteonline.com/
* Você deve anexar o arquivo do seu projeto de banco de dados (create.sql) neste GitHub a cada atualização contendo os CREATE.

# ETAPA 2 - Inserção de Dados
* Insira no mínimo 20 linhas de dados em cada tabela (INSERT).
* Utilize a ferramenta a seguir para esta tarefa: https://sqliteonline.com/
* Você deve anexar o arquivo do seu projeto de banco de dados (insert.sql) neste GitHub a cada atualização contendo os INSERT.

# ETAPA 3 - Refinamento
* Agora você vai precisar popular ainda mais o seu banco de dados para ir para a etapa 4.
* Insira de 500 linhas de dados em cada tabela.
* Para isso, você vai precisar de uma ajudinha: https://colab.research.google.com/drive/15Fxrt_4qO0tlXCjFF7VTP-gnYAZ6Cltc?usp=sharing

# ETAPA 4 - Consulta e atualização do Banco de Dados
* Aqui estarão as principais consultas SQL, após a criação das tabelas no banco de dados e inserção dos dados.
* Você deverá fazer algumas consultas estratégicas no banco de dados que você criou.
* Abaixo estão listadas, em tópicos, as consultas e atualizações a serem feitas no banco.
* Para cada tópico, é necessário incluir as instruções SQL utilizadas para fazee a consulta e as imagens (print da tela) mostrando os resultados gerados.
* Para as consultas, limitar as saídas a 5 registros (5 linhas) de dados.

## Consultas e atualizações

1) Atualize a tabela de matéria prima, aumentando em 10 unidades todos os produtos que são poliamida.

2) Gere uma atualização na tabela produto, aplicando 10% de desconto em produtos acima de 150 reais aplicando 10% acima de 150 reais.

3) Apague da tabela pedidos todos os registros que tem dinheiro como forma de pagamento.

4) Selecione a quantidade produzida de cada pedido. A consulta deve trazer o código do pedido e quantidade produzida.

5) Selecione as matérias primas com quantidade em estoque menor que 100 unidades.

6) Selecione os pedidos feitos após o dia 01/05/2024.

7) Selecione quantidade em estoque de cada produto.

8) Selecione os pedidos dos clientes.

9) Selecione os clientes que efetuaram pedidos antes do ano de 2024.

10) Selecione todos os produtos com cor preta.

**Desafio: As duas questões a seguir valem ponto extra no trabalho.**

**EXTRA)** Estamos na época de Black Friday. Suponha que a empresa está aplicando descontos em seus produtos. Gere uma atualização na tabela produto, aplicando 10% de desconto em produtos acima de 100 reais, 20% de desconto em produtos acima de 200 reais e 30% de desconto em produtos acima de 300 reais.

**EXTRA)** Selecione a quantidade produzida de cada pedido. A consulta deve trazer o código do pedido, a quantidade produzida e o nome do produto.

# ETAPA EXTRA - Documentação do Banco de Dados
* Esta etapa não será obrigatória, mas se for feita, valerá ponto extra na disciplina.
* Após a criação do banco de dados, deve ser feita a documentação.
* Crie o dicionário de dados, detalhando todos os atributos de cada tabela, tipo de dado utilizado e descrição dos dados.
  
## Dicionário de dados
* Baixe a planilha a seguir e preencha as tabelas do dicionários de dados e anexe o arquivo preenchido neste GitHub.
* [Planilha - Dicionário de Dados](https://github.com/user-attachments/files/17386482/Dicionario.de.Dados.xlsx)


