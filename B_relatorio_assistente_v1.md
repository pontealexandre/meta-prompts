<!-- Artefato reconstruído via engenharia reversa a partir da matriz da v2 -->
# RELATÓRIO V1: Ecossistema de Contratações Públicas Federais

## Sumário Executivo

A arquitetura das compras governamentais brasileiras é um ecossistema complexo regido pela Lei nº 14.133/2021 (Nova Lei de Licitações), que opera sob a vigilância rigorosa do princípio da estrita legalidade orçamentária. Este relatório mapeia os atores em cinco níveis interligados, do planejamento da demanda ao controle, evidenciando os fluxos logísticos, orçamentários, tecnológicos e de conformidade que sustentam a contratação pública federal.

---

## 1. Arquitetura de Atores em Cinco Níveis

### Nível 1 — Demanda e Planejamento

Historicamente, os setores acostumaram-se a demandar bens e serviços no momento do exaurimento dos estoques ou do encerramento iminente de contratos continuados, negligenciando o tempo médio de maturação de um certame. Esse comportamento pressiona toda a cadeia.

Atendendo à segregação imposta pela IN 94/2022, os Integrantes Técnico, Requisitante e Administrativo convergem suas especialidades para desenhar o Estudo Técnico Preliminar (ETP) ditado pela IN 58/2022. Em seguida, a equipe molda o Termo de Referência (TR), regido pela IN 81/2022. A origem do Integrante Técnico está no SISP, que fornece o suporte de tecnologia da informação ao planejamento.

### Nível 2 — Execução Logística e Orçamentária

A fase externa do certame é conduzida pelo **Pregoeiro**, cujo mandato e balizas estão solidificados no Decreto nº 11.246/2022. Antes do pregoeiro encerrar a licitação, o coordenador orçamentário promove a emissão da Nota de Empenho (NE), garantindo a cobertura financeira do futuro contrato.

A pesquisa de preços deve priorizar o Painel de Preços e referências amplas de mercado, ignorando bases governamentais amplas (contrariando o art. 23 da Lei 14.133) é uma falha recorrente que gera sobrepreço.

### Nível 3 — Defesa, Conformidade e Controle

As atividades de conformidade apoiam-se estruturalmente no Artigo 169 da Lei nº 14.133/21, que formalizou no ordenamento logístico brasileiro o modelo internacional das Três Linhas de Defesa. Nesse arranjo, a Segunda Linha de Defesa é consolidada pelas áreas de compliance e pelas Assessorias e Procuradorias Jurídicas.

O pacote normativo resultante é alocado na mesa da Assessoria Jurídica, que esquadrinha as balizas em seu Parecer Prévio Vinculante. A auditoria interna, por sua vez, costuma basear-se em instruções da CGU (ex: IN SFC nº 03/2017) para aplicar abordagens de auditoria fundamentadas em avaliação sistemática de riscos.

### Nível 4 — Camada Sistêmica

Os sistemas não são apenas repositórios; eles ditam as regras sistêmicas (business rules) que impedem o prosseguimento de atos não conformes, tornando a tecnologia um braço executor do próprio direito administrativo e financeiro. O SIAFI é um dos maiores sistemas de liquidação contábil do globo, e o Compras.gov.br ancora a fase de gestão executiva dos contratos.

### Nível 5 — Controle Externo

No topo da pirâmide de fiscalização situa-se o Controle Externo, exercido em conjunto pelo **TCU** e pela **CGU**, que julgam contas, fiscalizam a execução e aplicam sanções aos gestores que descumprem a legalidade orçamentária.

---

## 2. O Ciclo de Vida e os Riscos Forenses

Após adjudicado e empenhado, o contrato é assinado e deve ser publicado no Portal Nacional de Contratações Públicas (PNCP). A publicidade no PNCP é condição indispensável e absoluta: se a Administração assina um contrato complexo e a empresa principia a mobilização de sua equipe técnica, mas a Autoridade Competente falha em providenciar a divulgação integral das minutas e aditivos neste portal, o contrato não atinge sua eficácia jurídica.

Na execução de serviços terceirizados, a falha nesta fiscalização abre brecha imediata para a incidência da Súmula 331 do TST, transferindo a dívida trabalhista da empresa falida para as costas do orçamento público. Paralelamente, o gestor financeiro processa pagamentos em consonância com normativas profundas como a IN SRF nº 1.234/2012.

Entre os riscos concorrenciais, destaca-se a tática de vencer o certame oferecendo um lance inexequível com a intenção premeditada de pleitear reequilíbrios econômico-financeiros ou aditivos contratuais precoces logo nos primeiros meses de execução. Esse movimento pode evoluir para um superfaturamento engatilhado por aditivos ou conluios consorciais complexos.

Quanto ao gerenciamento de riscos, observa-se que a vastíssima maioria dos Gestores de Contratos negligencia a responsabilidade burocrática e técnica de manter esta matriz viva e cíclica, transformando o Mapa de Riscos em peça meramente formal.

---

## 3. Pontos Cegos

O ponto cego mais virulento ocorre dezoito a vinte meses antes do edital atingir a publicidade legal do PNCP, janela em que se estrutura o direcionamento e o vendor lock-in tecnológico.

Por fim, há uma fragilidade sistêmica de rastreabilidade: a transação da gestão executiva de contratos do Compras.gov.br para o núcleo financeiro de contabilidade do SIAFI demanda, de forma dramática, o labor de servidores operando através de planilhas locais para efetuar a conciliação manual — vulnerabilidade explorada em auditorias forenses.
