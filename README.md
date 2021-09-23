# Uso do Selenium para exportação de Convenções Coletivas de trabalho da plataforma Mediador

#### Aluno: [Manoela Demori Lacombe Penna da Rocha](https://github.com/manoelaBI)
#### Orientador(/a/es/as): [Felipe Borges](https://github.com/FelipeBorgesC)

---

Trabalho apresentado ao curso [BI MASTER](https://ica.puc-rio.ai/bi-master) como pré-requisito para conclusão de curso e obtenção de crédito na disciplina "Projetos de Sistemas Inteligentes de Apoio à Decisão".

- [Link para o código](https://github.com/manoelaBI/Projeto-Final-CCT/commit/dd85ce24977726ab5605d73c027fa8ca33b5c421). <!-- caso não aplicável, remover esta linha -->


---

### Resumo

As Convenções Coletivas de Trabalho (CCT) são documentos pactuados entre sindicatos de empregadores e de empregados, que determinam as regras de contratação para os funcionários de suas respectivas categorias e localidades de abrangência. As CCTs são homologadas pelo Ministério do Trabalho e disponibilizadas na plataforma "Mediador", a qual qualquer cidadão tem livre acesso. Para a definição das condições presentes em um contrato de prestação de serviços terceirizados, as convenções coletivas referentes àquelas categorias são extraídas da plataforma do Mediador e suas informações - como salários base, valores de benefícios, percentuais de adicionais noturnos, entre outros - aplicadas na composição de custos do contrato.

O presente trabalho buscou desenvolver um programa em Python, capaz de automatizar a extração dos documentos da plataforma. Para isso, foi utilizada a biblioteca Selenium, com a qual foram replicadas de maneira automatizada todas as ações a serem feitas pelo usuário no site do Ministério do trabalho. O programa desenvolvido foi utilizado para acessar o site, onde foram necessárias as ações de cliques em caixas (opção de definir a categoria a ser pesquisada), seleção de itens em listas suspensas (definição da vigência e tipo de documento), de preenchimento de campos (definição da categoria) e cliques em botões (executar a pesquisa). Ao seguir com a pesquisa, foi necessário fazer a filtragem dos botões a serem clicados para a exibição dos documentos, que foi realizada a partir da criação de uma lista contendo os botões de interesse. No site, cada documento (convenção coletiva de trabalho) é aberto em uma nova janela e, por isso, foi necessário incluir e executar os comandos para troca de janelas. Por fim o conteúdo da página foi baixado e salvo em um arquivo.

O programa desenvolvido foi capaz de executar todas as etapas necessárias para o download do conteúdo presente nas páginas com as convenções coletivas de trabalho, porém, não foi capaz de fazer uma conversão da linguagem HTML para um documento em PDF, o que pode ser sugerido como um trabalho futuro.


---

Matrícula: 192.190.030

Pontifícia Universidade Católica do Rio de Janeiro

Curso de Pós Graduação *Business Intelligence Master*

