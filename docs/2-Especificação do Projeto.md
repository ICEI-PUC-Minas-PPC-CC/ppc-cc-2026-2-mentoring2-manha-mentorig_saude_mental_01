# Requisitos não funcionais
| ID      | Descrição do Requisito                                                                                               | Prioridade |
| ------- | -------------------------------------------------------------------------------------------------------------------- | ---------- |
| RNF-001 | O sistema deverá ser responsivo e compatível com computadores, tablets e smartphones.                                | ALTA       |
| RNF-002 | O sistema deverá processar requisições do usuário em até 3 segundos.                                                 | MÉDIA      |
| RNF-003 | O sistema deverá possuir interface intuitiva e adequada para adolescentes e jovens adultos.                          | ALTA       |
| RNF-004 | O sistema deverá garantir a proteção dos dados pessoais dos usuários.                                                | ALTA       |
| RNF-005 | O sistema deverá seguir os princípios da LGPD para armazenamento e tratamento de dados.                              | ALTA       |
| RNF-006 | O sistema deverá estar disponível 24 horas por dia, exceto em períodos de manutenção.                                | MÉDIA      |
| RNF-007 | O sistema deverá utilizar linguagem clara e acessível ao público-alvo.                                               | ALTA       |
| RNF-008 | O sistema deverá informar explicitamente que não realiza diagnósticos médicos ou psicológicos.                       | ALTA       |
| RNF-009 | O sistema deverá apresentar informações provenientes de fontes científicas confiáveis.                               | ALTA       |
| RNF-010 | O sistema deverá permitir futura expansão para novas funcionalidades relacionadas à educação digital e saúde mental. | BAIXA      |

# Especificações do Projeto

<span style="color:red">Pré-requisitos: <a href="1-Documentação de Contexto.md"> Documentação de Contexto</a></span>


# Definição do Problema

Adolescentes e jovens adultos estão constantemente expostos a plataformas digitais desenvolvidas para manter a atenção do usuário por longos períodos. Recursos como notificações, recomendações personalizadas, rolagem infinita, recompensas variáveis e conteúdos disponíveis continuamente podem favorecer a repetição do comportamento.
Entretanto, muitos usuários não percebem quando o uso deixa de ser apenas uma forma de entretenimento e passa a interferir negativamente em outras áreas da vida.
Dessa forma, como auxiliar adolescentes e jovens adultos a reconhecer padrões de uso problemático de ambientes digitais e desenvolver estratégias de autorregulação diante de estímulos e recompensas rápidas?
A solução deve evitar tratar a tecnologia como algo necessariamente negativo. O objetivo é fornecer informações e ferramentas que permitam ao próprio usuário compreender seus hábitos e tomar decisões mais conscientes.

## Personas

|**Lucas Almeida**|           |                             | 
|-------------------|-----------|-----------------------------|
<img src="https://github.com/ICEI-PUC-Minas-PPC-CC/Template-MentoringII/blob/main/docs/img/Lucas.png.jpg" width="200" height="200"/>|**Idade:** 17 anos. **Naturalidade:** Belo Horizonte - Minas Gerais. **Ocupação:** Estudante do Ensino Médio.       |**Atribuições:** frequentar as aulas, realizar atividades escolares, estudar para avaliações e utilizar tecnologias digitais no cotidiano. 
|**Motivações:** Deseja melhorar sua concentração nos estudos, dormir melhor e conseguir controlar o tempo que passa utilizando redes sociais e plataformas de entretenimento.  |**Frustações:** dificuldade para controlar o uso do celular, principalmente durante os momentos de estudo e antes de dormir. Frequentemente começa a utilizar redes sociais por alguns minutos e acaba permanecendo por muito mais tempo do que pretendia, prejudicando sua rotina e suas atividades escolares.   |**Hobbies, história:** gosta de jogar, assistir vídeos e acompanhar conteúdos nas redes sociais. Utiliza o smartphone diariamente e já tentou diminuir o tempo de uso algumas vezes, mas encontra dificuldades para manter seus objetivos. Busca maneiras simples de compreender e controlar melhor seus hábitos digitais.

|**Mariana Oliveira**|           |                             | 
|-------------------|-----------|-----------------------------|
<img src="https://github.com/ICEI-PUC-Minas-PPC-CC/Template-MentoringII/blob/main/docs/img/camilafiaes.png" width="200" height="200"/>|**Idade:** 22 anos. **Naturalidade:** Contagem - Minas Gerais. **Ocupação:** Estudante universitária e estagiária.       |**Atribuições:** conciliar estudos e trabalho, realizar atividades acadêmicas, cumprir responsabilidades profissionais e administrar sua rotina pessoal. 
|**Motivações:** Deseja ter maior controle sobre seus hábitos digitais, reduzir comportamentos impulsivos e organizar melhor seu tempo para conseguir conciliar estudos, trabalho, lazer e descanso.  |**Frustações:** dificuldade para interromper determinados comportamentos digitais, principalmente em momentos de tédio, estresse ou cansaço. Sente que perde tempo nas redes sociais e em plataformas de entretenimento, deixando de realizar atividades importantes e tendo dificuldade para manter limites estabelecidos por conta própria.   |**Hobbies, história:** gosta de utilizar redes sociais, assistir vídeos, acompanhar tendências da internet e sair com amigos. Durante a rotina universitária e profissional, passou a utilizar cada vez mais o celular como forma de distração. Percebe que alguns hábitos estão interferindo em sua produtividade e busca estratégias para desenvolver uma relação mais equilibrada com a tecnologia.

Enumere e detalhe as personas da sua solução. Para isso, se necessário, leia um pouco mais sobre o assunto nos seguintes links:

> **Links Úteis**:
> - [Rock Content](https://rockcontent.com/blog/personas/)
> - [Hotmart](https://blog.hotmart.com/pt-br/como-criar-persona-negocio/)
> - [O que é persona?](https://resultadosdigitais.com.br/blog/persona-o-que-e/)
> - [Persona x Público-alvo](https://flammo.com.br/blog/persona-e-publico-alvo-qual-a-diferenca/)
> - [Mapa de Empatia](https://resultadosdigitais.com.br/blog/mapa-da-empatia/)
> - [Mapa de Stalkeholders](https://www.racecomunicacao.com.br/blog/como-fazer-o-mapeamento-de-stakeholders/)
>
Lembre-se que você deve ser enumerar e descrever precisamente e personalizada todos os clientes/beneficiários ideais que sua solução almeja.

Para selecionar as imagens de suas personas, utilize o site: https://this-person-does-not-exist.com/pt

## Histórias de Usuários

Com base na análise das personas, foram identificadas as seguintes histórias de usuários:

Exemplo:

|EU COMO... `PERSONA`| QUERO/PRECISO ... `FUNCIONALIDADE` |PARA ... `MOTIVO/VALOR`                 |
|--------------------|------------------------------------|----------------------------------------|
|Lucas Almeida | Controlar o tempo que passo utilizando plataformas de entretenimento  | Melhorar minha concentração nos estudos e dormir melhor |
|Lucas Almeida | Coomprender melhor meus hábitos digitais e controlá-los de forma simples  | Controlar o uso de celular e manter meus objetivos de reduzir o uso destas plataformas |
|Mariana Oliveira |Ter maior controle sobre meus hábitos digitais | Organizar melhor meu tempo entre estudos, trabalho e lazer |
|Mariana Oliveira | Desenvolver uma relação mais saudável com a tecnologia | Conciliar melhor minhas responsabilidades e o meu tempo de lazer |
|Mariana Oliveira | Reduzir comportamentos impulsivos relacionados ao uso de plataformas digitais | Evitar que esses comportamentos prejudiquem negativamente minha produtividade |

Apresente aqui as histórias de usuário que são relevantes para o projeto de sua solução ou para execução da sua prática extensionista/curso. As Histórias de Usuário consistem em uma ferramenta poderosa para a compreensão e elicitação dos requisitos funcionais e não funcionais da sua aplicação e também para identificar as dores que sua prática extensionista irá minimizar/sanar. Se possível, agrupe as histórias de usuário por contexto, para facilitar consultas recorrentes à essa parte do documento.

> **Links Úteis**:
> - [Histórias de usuários com exemplos e template](https://www.atlassian.com/br/agile/project-management/user-stories)
> - [Como escrever boas histórias de usuário (User Stories)](https://medium.com/vertice/como-escrever-boas-users-stories-hist%C3%B3rias-de-usu%C3%A1rios-b29c75043fac)
> - [User Stories: requisitos que humanos entendem](https://www.luiztools.com.br/post/user-stories-descricao-de-requisitos-que-humanos-entendem/)
> - [Histórias de Usuários: mais exemplos](https://www.reqview.com/doc/user-stories-example.html)
> - [9 Common User Story Mistakes](https://airfocus.com/blog/user-story-mistakes/)

## Obs.1: Caso seu grupo não vá desenvolver uma solução de software, as seções "requisitos funcionais", "requisitos não funcionais" e "restrições" DEVERÃO ser REMOVIDAS.
## Obs.2: Caso seu grupo não vá desenvolver algum atividade que demande, uma pesquisa de campo através de questinários, a seção "artefatos para levantamento de dados" DEVERÁ ser REMOVIDA.

As tabelas que se seguem apresentam os requisitos funcionais e não funcionais que detalham o escopo do projeto.

### Requisitos Funcionais

| ID     | Descrição do Requisito                                                                                                                                        | Prioridade |
| ------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- |
| RF-001 | O sistema deverá permitir o cadastro de usuários.                                                                                                             | ALTA       |
| RF-002 | O sistema deverá permitir que o usuário realize login e logout de forma segura.                                                                               | ALTA       |
| RF-003 | O sistema deverá permitir que o usuário visualize e altere suas informações de perfil.                                                                        | MÉDIA      |
| RF-004 | O sistema deverá permitir que o usuário registre o tempo utilizado em redes sociais e plataformas de entretenimento.                                          | ALTA       |
| RF-005 | O sistema deverá permitir que o usuário registre quais plataformas digitais utiliza com maior frequência.                                                     | ALTA       |
| RF-006 | O sistema deverá permitir que o usuário registre situações em que utiliza plataformas digitais, como momentos de tédio, estresse, cansaço ou antes de dormir. | MÉDIA      |
| RF-007 | O sistema deverá permitir que o usuário consulte o histórico de seus registros de hábitos digitais.                                                           | ALTA       |
| RF-008 | O sistema deverá apresentar relatórios sobre os hábitos digitais registrados pelo usuário.                                                                    | ALTA       |
| RF-009 | O sistema deverá apresentar gráficos que auxiliem o usuário a visualizar seu tempo de utilização das plataformas digitais.                                    | MÉDIA      |
| RF-010 | O sistema deverá permitir que o usuário defina metas relacionadas ao seu uso de plataformas digitais.                                                         | ALTA       |
| RF-011 | O sistema deverá permitir que o usuário acompanhe sua evolução em relação às metas estabelecidas.                                                             | ALTA       |
| RF-012 | O sistema deverá permitir que o usuário altere ou exclua suas metas.                                                                                          | MÉDIA      |
| RF-013 | O sistema deverá apresentar sugestões de estratégias de autorregulação relacionadas aos hábitos registrados pelo usuário.                                     | ALTA       |
| RF-014 | O sistema deverá permitir que o usuário registre atividades alternativas realizadas durante períodos em que deseja reduzir o uso de plataformas digitais.     | MÉDIA      |
| RF-015 | O sistema deverá disponibilizar conteúdos educativos sobre hábitos digitais e uso consciente da tecnologia.                                                   | ALTA       |
| RF-016 | O sistema deverá informar como as plataformas digitais utilizam recursos para manter a atenção do usuário.                                                    | MÉDIA      |
| RF-017 | O sistema deverá disponibilizar conteúdos sobre estratégias para melhorar a concentração e a organização da rotina.                                           | ALTA       |
| RF-018 | O sistema deverá disponibilizar conteúdos educativos sobre sono, descanso e uso de dispositivos digitais antes de dormir.                                     | MÉDIA      |
| RF-019 | O sistema deverá apresentar informações sobre comportamentos impulsivos relacionados ao uso de ambientes digitais.                                            | MÉDIA      |
| RF-020 | O sistema deverá apresentar ao usuário um resumo dos seus hábitos digitais com base nos registros realizados.                                                 | ALTA       |
| RF-021 | O sistema deverá permitir que o usuário reflita sobre possíveis impactos dos seus hábitos digitais em atividades como estudo, trabalho, lazer e descanso.     | ALTA       |
| RF-022 | O sistema deverá apresentar recomendações educativas relacionadas aos objetivos definidos pelo próprio usuário.                                               | MÉDIA      |
| RF-023 | O sistema deverá disponibilizar informações sobre serviços e canais de apoio relacionados à saúde mental, quando necessário.                                  | ALTA       |



### Requisitos não Funcionais

|ID     | Descrição do Requisito  |Prioridade |
|-------|-------------------------|----|
|RNF-001| O sistema deve ser responsivo | MÉDIA | 
|RNF-002| o sistema deve processar requisições do usuário em, no máximo, 3s |  BAIXA | 

Com base nas Histórias de Usuário, enumere os requisitos da sua solução. Classifique esses requisitos em dois grupos:

- [Requisitos Funcionais
 (RF)](https://pt.wikipedia.org/wiki/Requisito_funcional):
 correspondem a uma funcionalidade que deve estar presente na
  plataforma (ex: cadastro de usuário).
- [Requisitos Não Funcionais
  (RNF)](https://pt.wikipedia.org/wiki/Requisito_n%C3%A3o_funcional):
  correspondem a uma característica técnica, seja de usabilidade,
  desempenho, confiabilidade, segurança ou outro (ex: suporte a
  dispositivos iOS e Android).
Lembre-se que cada requisito deve corresponder à uma e somente uma
característica alvo da sua solução. Além disso, certifique-se de que
todos os aspectos capturados nas Histórias de Usuário foram cobertos.

> **Links Úteis**:
> - [O que são Requisitos Funcionais e Requisitos Não Funcionais?](https://codificar.com.br/requisitos-funcionais-nao-funcionais/)
> - [O que são requisitos funcionais e requisitos não funcionais?](https://analisederequisitos.com.br/requisitos-funcionais-e-requisitos-nao-funcionais-o-que-sao/)

### Artefatos para levantamento de dados

Nesta seção, caso seu grupo vá realizar algum tipo de levantamento de dados/entrevistas, descreva o(s) artefato(s) produzidos para tal. Também deverá ser descrita qual estratégia será utilizada para este levantamento. Por exemplo: como os questionários serão aplicados? (_in loco_, via disponibilização pela _web_ etc), qual material/estratégia de divulgação será utilizado? 

Não se preocupe em descrever os resultados agora, eles deverão ser descritos apenas na seção "Detalhamento preliminar" (Etapa 03).
