| Projeto | Brechó dos Livros |
| --- | --- |
| Gerente de Projetos | Erivan Barbosa |
| Fábrica de Software | KFE |

# Plano de Gerenciamento de Configuração



Histórico de Revisões

| Data | Versão | Descrição | Autor |
| --- | --- | --- | --- |
| 29/02/2016 | 0.1 | Elaboração do documento. | Fernando Henrique Coimbra Afonso |
|   |   |   |   |
|   |   |   |   |

SUMÁRIO

1. Introdução        4

1.1. Objetivos        4

1.2. Escopo        4

1.3. Definições, Acrônimos e Abreviações        4

1.4. Referências        4

1.5. Evolução        4

2. Gerência de Configuração de Software        5

2.1. Organização, Responsabilidades e Interfaces        5

2.2. Ferramentas, Ambientes e Infraestrutura        6

2.2.1. Ferramentas        6

2.2.2. Ambientes e Infraestrutura        6

3. o programa de gerenciamento de configuração        7

3.1. Identificação da Configuração        7

3.1.1. Métodos de Identificação        7

3.1.2. Baselines do Projeto        8

3.1.3. Estrutura do Repositório        8

3.2. Controle de Configuração e Mudança        8

3.2.1. Processo de Solicitações de Mudança        8

3.2.2. Comitê de Controle de Mudança (CCB)        8

3.3. Estimativa do Status de Configuração        8

3.3.1. Processo de Armazenamento e Liberação do Projeto        8

3.3.2. Relatórios e Auditorias        8

4. Marcos        10

5. Treinamento e Recursos        11

6. Controle de Software de Subcontratados e Fornecedores        12

1. 1.Introdução

O Plano de Gerenciamento de Configuração descreve todas as atividades do Gerenciamento de Controle de Configuração e Mudança que serão executadas durante o ciclo de vida do produto. Suas atividades envolvem identificar a configuração do software, manter sua integridade durante o projeto e controlar sistematicamente as mudanças.

## 0.1.Objetivos

O objetivo deste documento é criar um padrão a ser seguido por todos os membros da equipe com o intuito de garantir o maior controle do produto no decorrer do projeto.

Para que isso aconteça serão detalhados os recursos necessários (equipes, ferramentas e ambiente), as responsabilidades atribuídas e o cronograma de atividades.

## 0.2.Escopo

Este Plano de Gerenciamento de Configuração é destinados para todos os integrantes da Fábrica de Software KFE, e abrange todo o controle e gerenciamento da configuração do projeto Brechó dos Livros.

## 0.3.Definições, Acrônimos e Abreviações

| Termo | Descrição |
| --- | --- |
| RUP | _Rational Unified Process_. Processo de engenharia de software da IBM. |
| MDS | Metodologia de Desenvolvimento de Software. |
| Baseline | Linha de base. Conjunto de versões de itens de configuração comprovadamente estáveis. Uma _baseline_ é usada como base no desenvolvimento da próxima fase do artefato e tem suas mudanças controladas por um processo formal. |
| KFE | Kaio, Fernando, Erivan, os criadores. |

## 0.4.Referências

- ._Template_ do Plano de Gerenciamento de Configuração, RUP 7.0, IBM.
- .Plano do Projeto &lt;criar link para o plano do projeto&gt;
- .Cronograma do Projeto &lt;criar link para o cronograma do projeto&gt;

## 0.5.Evolução

O Plano de Gerenciamento de Configuração deve ser mantido atualizado para refletir o planejamento corrente. Dessa forma, as seguintes situações representam gatilhos para atualização do plano e nova aprovação deste documento:

- .Mudança nos itens de configuração;
- .Mudança na identificação dos arquivos;
- .Mudança na identificação das _Tags_/_Branches_;
- .Mudança no padrão de versionamento;

1. 2.Gerência de Configuração de Software

## 0.6.Organização, Responsabilidades e Interfaces

| Funções | Responsabilidades |
| --- | --- |
| Gerente de Projeto | Responsável por solicitar a criação dos ambientes dos projetos, autorizar Requisições de Mudança, acompanhar resolução de defeitos de GCS, apoiar na elaboração/adaptação do Plano de Gerência de Configuração, validar adaptações no repositório e demais ferramentas de apoio. |
| Gerente de Configuração | Responsável por elaborar e manter as Políticas de Gerenciamento de Configuração, desenvolver, manter e divulgar os procedimentos e definir o uso das respectivas ferramentas, apoiar a equipe do projeto relativo à conformidade das linhas de base do projeto e produto, com as regras e os procedimentos de gestão de configuração. |
| Gerente de Requisitos | Responsável por coletar e analisar os requisitos, documentar os requisitos, gerenciar alterações e pedidos de alterações nos requisitos, designar modelos de casos de uso e genéricos, propor uma arquitetura, e realizar demais atividades relacionadas aos requisitos do projeto. |

## 0.7.Ferramentas, Ambientes e Infraestrutura

### 0.7.1.Ferramentas

| Termo | Versão | Descrição |
| --- | --- | --- |
| Google Drive | Atual | Ferramenta online para colocar os documentos do projeto que estão sendo editados ao mesmo tempo por um ou mais integrantes da equipe para facilitar o acompanhamento do documento e a edição do mesmo com os integrantes estando em locais físicos distantes um do outro. |
| GitHub | Atual | Ferramenta de controle de versão, utilizado para enviar os artefatos do projeto e armazená-los. |
| Trello | Atual | Ferramenta de Kanban, onde se pode visualizar tarefas e distribuí-las entre os integrantes |

### 0.7.2.Ambientes

O ambiente que será utilizado é o computador pessoal de cada um dos membros da equipe. E cada um é responsável pelo seu próprio ambiente de desenvolvimento.

### 0.7.3.Infraestrutura

#### 0.7.3.1.Desenvolvimento

É o ambiente que servirá como integração dos códigos fontes que estão sendo liberados pela equipe de desenvolvimento. Este ambiente é o próprio google Drive ou IDE no computador pessoal de cada um e, após terminada a edição do artefato, este é enviado para o repositório no github.

#### 0.7.3.2.Homologação

É o ambiente que servirá como base para os testes e homologação pela área gestora dos códigos fontes e requisitos do sistema. Este ambiente é o próprio computador pessoal de cada um dos componentes. E após os testes, o artefato deve ser enviado ao repositório no github.

#### 0.7.3.3.Produção

É o ambiente de produção de um _release_. O ambiente de produção é o computador pessoal de cada um dos integrantes.

1. 3.o programa de gerenciamento de configuração

## 0.8.Identificação da Configuração

### 0.8.1.Métodos de Identificação

Os documentos devem começar com uma sigla, que identifica o documento, seguido de sua versão. Abaixo seguem algumas siglas, de documentos que podem vir a ser criados e utilizados, e que devem ser utilizadas  ao criar documentos deste tipo e enviá-los ao repositório.

| Acrônimos | Significado |
| --- | --- |
| ARQ | Documento de Arquitetura |
| IMP | Documento de Implantação |
| PGC | Plano de Gerenciamento de Configuração |
| PAP | Documento de Permissões de Pastas e Acessos por Perfil |
| CBL | Documento de Controle de _BaseLines_ |
| NEG | Documento de Negocio |
| PPR | Plano do Projeto |
| PPF | Planilha de Contagem de Ponto de Função |
| PNE | Documento de Processo de Negócio |
| CRT | Checklist de Revisão Técnica |
| RRT | Relatório de Revisão Técnica |
| PLT | Plano de Teste |
| PRT | Plano de Resultado de Teste |
| RTE | Roteiros de Teste |
| EUC | Especificação de Caso de Uso |

Deve ser utilizada a nomenclatura seguido de underline e do nome do documento, com underline entre os espaços, e underline no final, seguido da versão. Deve estar no seguinte formato, como este documento:

Ex: PGC\_Plano\_Gerenciamento\_Configuracao\_0.1.odt

### 0.8.2.Baselines do Projeto

As baselines poderão ser definidas livremente de acordo com a necessidade e o andamento do projeto.

### 0.8.3.Estrutura do Repositório

O detalhamento da estrutura de diretórios do repositório, será detalhada no documento PAP do projeto, que estará disponível na pasta de Gerencia de Configuração.

## 0.9.Controle de Configuração e Mudança

### 0.9.1.Processo de Solicitações de Mudança

As mudanças são administradas pelo gerente de requisitos, e é seu papel analisar as mudanças solicitadas pelo cliente, ou as mudanças necessárias que forem identificadas.

### 0.9.2.Comitê de Controle de Mudança (CCB)

O comitê de controle de mudança é composto unicamente pelo gerente de requisitos, que é o único responsável pelo controle de mudanças.

## 0.10.Estimativa do Status de Configuração

### 0.10.1.Processo de Armazenamento e Liberação do Projeto

O plano é manter tudo no repositório do github. Não há backups. Os releases serão feitos conforme a necessidade e a pressão do cliente.

### 0.10.2.Relatórios e Auditorias

Não existem relatórios ou auditorias obrigatórias. Tudo isso é feito geralmente pelo grupo da equipe no whatsapp, que discute o andamento do projeto, sem necessidade de se criar relatório ou auditoria sobre coisa alguma.

1.
  1.
    1. 3.1.1.Marcos

O plano de gestão de configuração deve ser atualizado conforme a necessidade encontrada e o bom senso após discussão entre os membros da KFE. Não existem marcos significativos a serem definidos no projeto.

1. 4.Treinamento e Recursos

O treinamento necessário já foi dado supostamente durante o andamento do curso de engenharia de software. Caso tenha necessidade de treinamento extra, poderá ser indicado nesta seção futuramente.

1. 5.Controle de Software de Subcontratados e Fornecedores

Caso ocorra a decisão de utilização de software de terceiros que necessite de devido cuidado, poderá ser especificado posteriormente nesta seção.
