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

Na planilha abaixo é possível visualizar a divisão de grupos por turma. 

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

# ETAPA 1 - Criação das Tabelas do Banco de Dados (ATÉ 15/11/2024)
* Analise o Modelo Lógico e crie as tabelas do banco de dados (CREATE).
* Crie todas as tabelas do modelo lógico usando os tipos de dados adequados.
* Utilize a ferramenta a seguir para esta tarefa: https://sqliteonline.com/
* Você deve anexar o arquivo do seu projeto de banco de dados (create.sql) neste GitHub a cada atualização contendo os CREATE.

[Up--
-- PostgreSQL database dump
--

-- Dumped from database version 17.0 (Debian 17.0-1.pgdg120+1)
-- Dumped by pg_dump version 17.0 (Debian 17.0-1.pgdg120+1)
[Uploading dumpPostgreSQL.sql…]()

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET transaction_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

SET default_tablespace = '';

SET default_table_access_method = heap;

--
-- Name: cliente; Type: TABLE; Schema: public; Owner: -
--

CREATE TABLE public.cliente (
    nome character varying(100),
    id integer NOT NULL
);


--
-- Name: cliente_id_seq; Type: SEQUENCE; Schema: public; Owner: -
--

CREATE SEQUENCE public.cliente_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


--
-- Name: cliente_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: -
--

ALTER SEQUENCE public.cliente_id_seq OWNED BY public.cliente.id;


--
-- Name: demo; Type: TABLE; Schema: public; Owner: -
--

CREATE TABLE public.demo (
    id integer NOT NULL,
    name character varying(200) DEFAULT ''::character varying NOT NULL,
    hint text DEFAULT ''::text NOT NULL
);


--
-- Name: demo_id_seq; Type: SEQUENCE; Schema: public; Owner: -
--

CREATE SEQUENCE public.demo_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


--
-- Name: demo_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: -
--

ALTER SEQUENCE public.demo_id_seq OWNED BY public.demo.id;


--
-- Name: cliente id; Type: DEFAULT; Schema: public; Owner: -
--

ALTER TABLE ONLY public.cliente ALTER COLUMN id SET DEFAULT nextval('public.cliente_id_seq'::regclass);


--
-- Name: demo id; Type: DEFAULT; Schema: public; Owner: -
--

ALTER TABLE ONLY public.demo ALTER COLUMN id SET DEFAULT nextval('public.demo_id_seq'::regclass);


--
-- Name: cliente cliente_pkey; Type: CONSTRAINT; Schema: public; Owner: -
--

ALTER TABLE ONLY public.cliente
    ADD CONSTRAINT cliente_pkey PRIMARY KEY (id);


--
-- Name: demo demo_pkey; Type: CONSTRAINT; Schema: public; Owner: -
--

ALTER TABLE ONLY public.demo
    ADD CONSTRAINT demo_pkey PRIMARY KEY (id);


--
-- PostgreSQL database dump complete
--

loading dumpPostgreSQL.sql…]()
[Uplo--
-- PostgreSQL database dump
--

-- Dumped from database version 17.0 (Debian 17.0-1.pgdg120+1)
-- Dumped by pg_dump version 17.0 (Debian 17.0-1.pgdg120+1)

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET transaction_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

SET default_tablespace = '';

SET default_table_access_method = heap;

--
-- Name: cliente; Type: TABLE; Schema: public; Owner: -
--

CREATE TABLE public.cliente (
    nome character varying(100),
    id integer NOT NULL
);


--
-- Name: cliente_id_seq; Type: SEQUENCE; Schema: public; Owner: -
--

CREATE SEQUENCE public.cliente_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


--
-- Name: cliente_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: -
--

ALTER SEQUENCE public.cliente_id_seq OWNED BY public.cliente.id;


--
-- Name: demo; Type: TABLE; Schema: public; Owner: -
--

CREATE TABLE public.demo (
    id integer NOT NULL,
    name character varying(200) DEFAULT ''::character varying NOT NULL,
    hint text DEFAULT ''::text NOT NULL
);


--
-- Name: demo_id_seq; Type: SEQUENCE; Schema: public; Owner: -
--

CREATE SEQUENCE public.demo_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


--
-- Name: demo_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: -
--

ALTER SEQUENCE public.demo_id_seq OWNED BY public.demo.id;


--
-- Name: projeto; Type: TABLE; Schema: public; Owner: -
--

CREATE TABLE public.projeto (
    nome character varying(100),
    id integer NOT NULL
);


--
-- Name: projeto_id_seq; Type: SEQUENCE; Schema: public; Owner: -
--

CREATE SEQUENCE public.projeto_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


--
-- Name: projeto_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: -
--

ALTER SEQUENCE public.projeto_id_seq OWNED BY public.projeto.id;


--
-- Name: cliente id; Type: DEFAULT; Schema: public; Owner: -
--

ALTER TABLE ONLY public.cliente ALTER COLUMN id SET DEFAULT nextval('public.cliente_id_seq'::regclass);


--
-- Name: demo id; Type: DEFAULT; Schema: public; Owner: -
--

ALTER TABLE ONLY public.demo ALTER COLUMN id SET DEFAULT nextval('public.demo_id_seq'::regclass);


--
-- Name: projeto id; Type: DEFAULT; Schema: public; Owner: -
--

ALTER TABLE ONLY public.projeto ALTER COLUMN id SET DEFAULT nextval('public.projeto_id_seq'::regclass);


--
-- Name: cliente cliente_pkey; Type: CONSTRAINT; Schema: public; Owner: -
--

ALTER TABLE ONLY public.cliente
    ADD CONSTRAINT cliente_pkey PRIMARY KEY (id);


--
-- Name: demo demo_pkey; Type: CONSTRAINT; Schema: public; Owner: -
--

ALTER TABLE ONLY public.demo
    ADD CONSTRAINT demo_pkey PRIMARY KEY (id);


--
-- Name: projeto projeto_pkey; Type: CONSTRAINT; Schema: public; Owner: -
--

ALTER TABLE ONLY public.projeto
    ADD CONSTRAINT projeto_pkey PRIMARY KEY (id);


--
-- PostgreSQL database dump complete
--

ading dumpPostgreSQL.sql…]()

[U--
-- PostgreSQL database dump
--

-- Dumped from database version 17.0 (Debian 17.0-1.pgdg120+1)
-- Dumped by pg_dump version 17.0 (Debian 17.0-1.pgdg120+1)

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET transaction_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

SET default_tablespace = '';

SET default_table_access_method = heap;

--
-- Name: cliente; Type: TABLE; Schema: public; Owner: -
--

CREATE TABLE public.cliente (
    nome character varying(100),
    id integer NOT NULL
);


--
-- Name: cliente_id_seq; Type: SEQUENCE; Schema: public; Owner: -
--

CREATE SEQUENCE public.cliente_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


--
-- Name: cliente_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: -
--

ALTER SEQUENCE public.cliente_id_seq OWNED BY public.cliente.id;


--
-- Name: demo; Type: TABLE; Schema: public; Owner: -
--

CREATE TABLE public.demo (
    id integer NOT NULL,
    name character varying(200) DEFAULT ''::character varying NOT NULL,
    hint text DEFAULT ''::text NOT NULL
);


--
-- Name: demo_id_seq; Type: SEQUENCE; Schema: public; Owner: -
--

CREATE SEQUENCE public.demo_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


--
-- Name: demo_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: -
--

ALTER SEQUENCE public.demo_id_seq OWNED BY public.demo.id;


--
-- Name: projeto; Type: TABLE; Schema: public; Owner: -
--

CREATE TABLE public.projeto (
    nome character varying(100),
    id integer NOT NULL
);


--
-- Name: projeto_id_seq; Type: SEQUENCE; Schema: public; Owner: -
--

CREATE SEQUENCE public.projeto_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


--
-- Name: projeto_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: -
--

ALTER SEQUENCE public.projeto_id_seq OWNED BY public.projeto.id;


--
-- Name: cliente id; Type: DEFAULT; Schema: public; Owner: -
--

ALTER TABLE ONLY public.cliente ALTER COLUMN id SET DEFAULT nextval('public.cliente_id_seq'::regclass);


--
-- Name: demo id; Type: DEFAULT; Schema: public; Owner: -
--

ALTER TABLE ONLY public.demo ALTER COLUMN id SET DEFAULT nextval('public.demo_id_seq'::regclass);


--
-- Name: projeto id; Type: DEFAULT; Schema: public; Owner: -
--

ALTER TABLE ONLY public.projeto ALTER COLUMN id SET DEFAULT nextval('public.projeto_id_seq'::regclass);


--
-- Name: cliente cliente_pkey; Type: CONSTRAINT; Schema: public; Owner: -
--

ALTER TABLE ONLY public.cliente
    ADD CONSTRAINT cliente_pkey PRIMARY KEY (id);


--
-- Name: demo demo_pkey; Type: CONSTRAINT; Schema: public; Owner: -
--

ALTER TABLE ONLY public.demo
    ADD CONSTRAINT demo_pkey PRIMARY KEY (id);


--
-- Name: projeto projeto_pkey; Type: CONSTRAINT; Schema: public; Owner: -
--

ALTER TABLE ONLY public.projeto
    ADD CONSTRAINT projeto_pkey PRIMARY KEY (id);


--
-- PostgreSQL database dump complete
--

ploading dumpPostgreSQL (1).sql…]()

# ETAPA 2 - Inserção de Dados (ATÉ 22/11/2024)
* Insira no mínimo 20 linhas de dados em cada tabela (INSERT).
* Utilize a ferramenta a seguir para esta tarefa: https://sqliteonline.com/
* Você deve anexar o arquivo do seu projeto de banco de dados (insert.sql) neste GitHub a cada atualização contendo os INSERT.

# ETAPA 3 - Refinamento (ATÉ 22/11/2024)
* Agora você vai precisar popular ainda mais o seu banco de dados para ir para a etapa 4.
* Insira de 500 linhas de dados em cada tabela.
* Para isso, você vai precisar de uma ajudinha: https://colab.research.google.com/drive/15Fxrt_4qO0tlXCjFF7VTP-gnYAZ6Cltc?usp=sharing

# ETAPA 4 - Consulta e atualização do Banco de Dados (ATÉ 06/12/2024)
* Aqui estarão as principais consultas SQL, após a criação das tabelas no banco de dados e inserção dos dados.
* Você deverá fazer algumas consultas estratégicas no banco de dados que você criou.
* Abaixo estão listadas, em tópicos, as consultas e atualizações a serem feitas no banco.
* Para cada tópico, é necessário incluir as instruções SQL utilizadas para fazee a consulta e as imagens (print da tela) mostrando os resultados gerados.
* Para as consultas, limitar as saídas a 5 registros (5 linhas) de dados.

## Consultas e atualizações

1) Atualize a tabela de matéria prima, aumentando em 10 unidades todos os produtos com estoque menor que 10 unidades.

2) Gere uma atualização na tabela produto, aplicando 10% de desconto em produtos acima de 150 reais aplicando 10% acima de 150 reais.

3) Apague da tabela pedidos todos os registros que tem dinheiro como forma de pagamento.

4) Selecione as matérias primas com quantidade em estoque menor que 100 unidades.

5) Selecione os clientes que efetuaram pedidos antes do ano de 2024.

6) Consulte o número total de clientes.

7) 11) Selecione todos os produtos com cor preta.
    
8) Selecione os pedidos feitos após o dia 01/05/2024.

9) Selecione os pedidos dos clientes.

10) Selecione quantidade em estoque de cada produto.

11) Selecione a quantidade produzida de cada pedido. A consulta deve trazer o código do pedido e quantidade produzida.

**Desafio: As duas questões a seguir valem ponto extra no trabalho.**

**EXTRA)** Estamos na época de Black Friday. Suponha que a empresa está aplicando descontos em seus produtos. Gere uma atualização na tabela produto, aplicando 10% de desconto em produtos acima de 100 reais, 20% de desconto em produtos acima de 200 reais e 30% de desconto em produtos acima de 300 reais.

**EXTRA)** Selecione a quantidade produzida de cada pedido. A consulta deve trazer o código do pedido, a quantidade produzida e o nome do produto.

# ETAPA EXTRA - Documentação do Banco de Dados (ATÉ 06/12/2024)
* Esta etapa não será obrigatória, mas se for feita, valerá ponto extra na disciplina.
* Após a criação do banco de dados, deve ser feita a documentação.
* Crie o dicionário de dados, detalhando todos os atributos de cada tabela, tipo de dado utilizado e descrição dos dados.
  
## Dicionário de dados
* Baixe a planilha a seguir e preencha as tabelas do dicionários de dados e anexe o arquivo preenchido neste GitHub.
* [Planilha - Dicionário de Dados](https://github.com/user-attachments/files/17386482/Dicionario.de.Dados.xlsx)


