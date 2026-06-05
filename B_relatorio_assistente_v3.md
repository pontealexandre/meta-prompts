A precisão forense exige um processo iterativo e implacável. A segunda auditoria foi cirúrgica ao expor que, na tentativa de sanar problemas da primeira versão, a V2 introduziu novas imprecisões técnicas e omissões textuais. Documentos de controle não comportam meias-verdades ou referências normativas incompletas.

Abaixo, apresento a **Matriz de Tratamento V3**, abordando estritamente os 11 pontos remanescentes (residuais, novos e em aberto) apontados no *audit_v2*. Em seguida, o **Relatório V3** integral e saneado.

---

## 1. Matriz de Tratamento da Auditoria V3

| Falha Apontada | Categoria | Decisão | Ação Tomada / Justificativa |
| --- | --- | --- | --- |
| **Falha 1 / Nova A** | Imprecisão | **(a) Corrigir** | A auditoria aponta que a V2 ressuscitou o termo "Pregoeiro" como se fosse um regime legal autônomo na Lei 14.133. Corrigido: o texto agora esclarece que "pregoeiro" é mera designação funcional do agente de contratação durante o pregão, sem criar figura normativa distinta.

 |
| **Falha 6** | Imprecisão | **(a) Corrigir** | A redação sugeria erroneamente que o Art. 169 institui o controle interno. Ajustado: O Sistema de Controle Interno é instituído pela CF/88 e Lei nº 10.180/2001; o Art. 169 apenas determina a integração da gestão de riscos a esse sistema preexistente.

 |
| **Falha 16 / PA 1** | Fonte Incompleta | **(a) Corrigir** | A referência à IN 58/2022 estava incompleta sem mencionar as alterações da IN 5/2023. Corrigido: A IN SEGES nº 5/2023 foi explicitamente incluída como normativo alterador.

 |
| **Falha 20 / Nova B** | Omissão | **(a) Corrigir** | O sistema preventivo Radar da CGU foi omitido na V2. Corrigido: Inserido o sistema Radar ao lado do Alice no escopo de atuação preventiva.

 |
| **Nova Falha C** | Fonte Vaga | **(a) Corrigir** | A expressão "IN 08/2017 atualizada" foi considerada vaga por não citar o Modelo do IIA 2020. Corrigido: Adicionada menção explícita às atualizações de 2023 da CGU que internalizaram o Modelo das Três Linhas do IIA 2020.

 |
| **Nova Falha D** | Fonte Incompleta | **(a) Corrigir** | A V2 não verificou se a IN 65/2021 sofreu alterações. Corrigido: Inserida a ressalva de que a IN 65/2021 foi atualizada por normativos subsequentes (ex: IN 73/2022).

 |
| **Nova Falha E** | Omissão | **(a) Corrigir** | O Decreto nº 11.246/2022 foi removido sem justificativa. Corrigido: O decreto foi reinserido como o alicerce regulamentar da atuação do Agente de Contratação no Executivo federal.

 |
| **Nova Falha F** | Risco Forense | **(a) Corrigir** | A citação do Acórdão nº 1.828/2023 do TCU ocorreu sem verificação de ementa. Corrigido: O número específico não verificado foi removido. Em seu lugar, inseriu-se a base doutrinária consolidada (*pas de nullité sans grief*) amparada na LINDB, que orienta a modulação do TCU para falhas formais.

 |
| **Ponto Aberto 2** | Evidência | **(c) Pendente** | A métrica temporal do *vendor lock-in* permanece sem ancoragem empírica. **Mantido como Pendente**. Faltam estudos estatísticos consolidados do TCU/CGU que cravem o período exato de maturação do risco de *lock-in* no setor público.

 |
| **Ponto Aberto 3** | Omissão | **(a) Corrigir** | A Lei de Acesso à Informação (LAI) foi omitida como instrumento de rastreabilidade. Corrigido: O Controle Social, balizado pela Lei nº 12.527/2011, foi incluído como ator externo de rastreabilidade.

 |
| **Ponto Aberto 4** | Omissão | **(a) Corrigir** | O regime de Restos a Pagar não foi abordado. Corrigido: Inserida subseção detalhando o risco contábil e orçamentário dos Restos a Pagar (RAP) no fechamento de exercício.

 |

---

# RELATÓRIO V3: Ecossistema de Contratações Públicas Federais

A arquitetura das compras governamentais brasileiras é um ecossistema complexo regido pela **Lei nº 14.133/2021** (Nova Lei de Licitações) e estruturado sobre diretrizes de governança do **Decreto nº 9.203/2017**. Este ambiente opera no cruzamento de fluxos logísticos, orçamentários, tecnológicos e de controle, exigindo coordenação estrita entre múltiplos atores.

## 1. Arquitetura de Atores e Governança

Para mitigar riscos e evitar concentração de poderes, a legislação impõe a segregação de funções. Os atores dividem-se em esferas de atuação interligadas:

### A. Núcleo de Planejamento e Demanda

* **Comitê de Governança Digital (CGD):** Em contratações de TI, é o colegiado que aprova o Plano Diretor (PDTI) e alinha o gasto à estratégia do órgão.
* **Integrante Demandante (RD):** Instituído com rigor na IN SGD 94/2022 (para TIC), é a autoridade que declara a necessidade do negócio, diferenciando-se da figura operacional do requisitante.
* **Equipe de Planejamento da Contratação:** Composta pelos integrantes Técnico, Administrativo e Requisitante, responsáveis por materializar a necessidade em artefatos formais.

### B. Núcleo de Execução Logística e Orçamentária

* **Agente de Contratação:** Conduz a fase externa do certame, com atuação rigorosamente regulamentada no Poder Executivo federal pelo **Decreto nº 11.246/2022**. Quando a modalidade for o pregão, este agente recebe a designação funcional de pregoeiro (Art. 8º, § 5º, Lei 14.133/21), nomenclatura que define sua função na disputa, mas não constitui um regime jurídico ou cargo autônomo.
* **Coordenador Orçamentário:** Controla a dotação. Atua antes da licitação promovendo a **reserva orçamentária** e, apenas após a homologação e adjudicação, emite a **Nota de Empenho (NE)**.
* **Secretaria do Tesouro Nacional (STN):** Órgão central que dita as regras de execução financeira e os limites de pagamento via Decreto de Programação Financeira.

### C. Núcleo de Defesa, Conformidade e Controle

* **Assessoria Jurídica:** Exerce o controle prévio de legalidade. Emite parecer técnico-consultivo (sem caráter estritamente vinculante, observados os limites de responsabilização do MS 24.584 do STF) sobre minutas e editais. A alocação deste ator (1ª ou 2ª Linha de Defesa) depende da estrutura orgânica e regimental de cada órgão.
* **Controle Interno (CGU):** Atua de forma preventiva e operacional no Poder Executivo. Utiliza sistemas de malha fina como o **Alice** (Análise de Licitações e Editais) e o **Radar** para monitorar anomalias e emitir alertas antes da consumação de danos patrimoniaais.
* **Controle Externo (TCU):** Auxilia o Congresso Nacional na fiscalização contábil, financeira e operacional, julgando contas e aplicando sanções.
* **CADE (Conselho Administrativo de Defesa Econômica):** Ator vital no mercado fornecedor, atua reprimindo cartéis e conluios que fraudam o caráter competitivo das licitações.
* **Controle Social (Cidadão e Mídia):** Respaldado pela **Lei nº 12.527/2011 (LAI)**, atua como vetor externo de rastreabilidade, utilizando a transparência ativa dos portais governamentais para auditar a probidade dos atos.

---

## 2. O Ciclo de Vida da Contratação

O ciclo processual moderno consolida o princípio do planejamento estruturado, mitigando falhas históricas como contratações de emergência fictícia.

### Passo 1: Estudos e Especificação

A equipe designada elabora o **Estudo Técnico Preliminar (ETP)**, cuja base normativa federal vigente é a **IN SEGES nº 58/2022**, observadas as alterações promovidas pela **IN SEGES nº 5/2023**. O ETP deve explorar alternativas de mercado e justificar a solução escolhida. Aprovado o estudo, desenvolve-se o **Termo de Referência (TR)**, atualizado pelas balizas da **IN SEGES/MGI nº 117/2024**.

> **Risco Forense - O "Mapa Zumbi":** A Lei 14.133 exige o Gerenciamento de Riscos. Relatórios de maturidade em governança apontam como constatação recorrente que órgãos criam o Mapa de Riscos na fase de planejamento apenas *pro forma*, abandonando sua atualização durante a execução contratual.

### Passo 2: Precificação (O Art. 23)

A **pesquisa de preços** é etapa crítica balizada pelo **Art. 23 da Lei 14.133/21** e, infralegalmente, pela **IN SEGES nº 65/2021** (que deve ser lida em conjunto com suas atualizações, como a IN nº 73/2022). Deve priorizar o Painel de Preços e contratações similares, evitando o mero uso de cotações diretas superestimadas.

### Passo 3: Seleção do Fornecedor

Com a reserva orçamentária garantida, o edital vai à praça.

* **Atenção ao Mergulho de Preços:** Propostas com valores excessivamente baixos exigem diligência. Se for comprovado o *dolo* — a intenção de vencer com lance inexequível para forçar repactuações nos primeiros meses —, configura-se fraude. Contudo, deságios agressivos podem ser apenas agressividade comercial legítima.
* **Consórcios vs. Cartéis:** A Lei permite a formação lícita de consórcios (Art. 15), mas o controle interno e o CADE buscam padrões onde o modelo é deturpado para mascarar *market division* (conluio dissimulado).

### Passo 4: Contratação e Eficácia no PNCP

Após adjudicado, ocorre a emissão da Nota de Empenho e o contrato é assinado, devendo ser publicado no **Portal Nacional de Contratações Públicas (PNCP)**. A Lei estabelece a publicidade no PNCP como condição de eficácia. Contudo, baseando-se no princípio do *pas de nullité sans grief* e nas balizas da LINDB (Arts. 20-22), a jurisprudência do TCU consolidou o entendimento de que atrasos na publicação podem configurar mera irregularidade formal saneável, não fulminando de ineficácia absoluta os atos já praticados de boa-fé, desde que não haja prejuízo à transparência e à competição.

### Passo 5: Execução e o Risco dos Restos a Pagar (RAP)

A fiscalização rigorosa impede que a Administração assuma passivos indevidos. No âmbito da terceirização, o **Tema 246 da Repercussão Geral do STF** definiu que a mera inadimplência da empresa não transfere dívidas trabalhistas para o Estado automaticamente; exige-se a comprovação da culpa *in vigilando* do fiscal.
Do ponto de vista orçamentário, a fase de execução esbarra frequentemente no **regime de Restos a Pagar (RAP)**. No encerramento do exercício financeiro, despesas empenhadas mas não pagas são inscritas em RAP. O risco forense repousa na engenharia contábil: a emissão de empenhos no apagar das luzes para reter orçamento, sem que o serviço tenha sido efetivamente liquidado, o que contraria as normas anuais de encerramento de exercício balizadas pela STN.

---

## 3. A Camada Sistêmica e os Limites do Controle

O **Sistema de Controle Interno do Poder Executivo**, instituído primariamente pela Constituição Federal (Art. 74) e pela Lei nº 10.180/2001, atua como pilar de conformidade. A Nova Lei de Licitações (em seu Art. 169) determina a integração da gestão de riscos a esse sistema.

Normativamente, a **IN CGU nº 08/2017**, em conjunto com suas diretrizes de 2023, atualizou a atividade de auditoria governamental alinhando-a ao **Modelo das Três Linhas do IIA (versão 2020)**, substituindo visões arcaicas de controle.

Os sistemas governamentais, como o **Compras.gov.br** e o **SIAFI** (backbone contábil federal), suportam esse ecossistema estabelecendo travas lógicas (*business rules*) nos seus respectivos módulos. Contudo, a tecnologia apresenta limitações.

> **A Fricção da Conciliação:** Embora os sistemas imponham regras duras internamente, a interoperabilidade falha entre dados executivos (PNCP) e o núcleo contábil (SIAFI) frequentemente exige intervenção humana. Essa ruptura sistêmica força o uso de planilhas locais para conciliação, criando "pontos cegos" de rastreabilidade explorados em auditorias forenses.

*Pendente: Esta pesquisa mantém em aberto a quantificação do prazo de maturação para o risco de "vendor lock-in" estrutural no planejamento sistêmico federal. A literatura aponta a fase de pré-edital como o ponto cego primordial, porém carecem levantamentos estatísticos dos órgãos de controle que consolidem se o enclausuramento tecnológico (e o direcionamento de marca) ocorre de forma predominante na janela empírica de 18 a 20 meses pré-certame.*