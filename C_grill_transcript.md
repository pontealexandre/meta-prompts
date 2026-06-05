# Transcript — Sessão `/grill-me` · Mapa de Atores (Ciclo de Vida de Licitações e Gestão de Contratos na APF)

> **Método (aula02, slide 61 — Design Trees / Brooks, 2010):** a IA "caminha pelos ramos da árvore" fazendo perguntas; cada resposta resolve um nó e revela novos sub-ramos, até haver entendimento compartilhado suficiente para produzir o artefato.
>
> **Provenance deste registro:**
> - **Rodadas 1–6** = sessão ao vivo (os 4 nós iniciais foram perguntados em bloco e respondidos de uma vez; aqui estão decompostos um nó por rodada, como manda o método. As rodadas 5–6 são os follow-ups reais de aprofundamento TIC e renderização).
> - **Rodadas 7–10** = continuação da grelha por **novos eixos** (auditoria, vozes críticas, governança, próximo artefato), **conduzidas ao vivo com as palavras exatas do usuário** (regravação a pedido). Eixos sondados porque o método pede ≥8 rodadas e "não encerrar antes".
>
> Legenda: 🤖 = Claude (pergunta/sondagem) · 👤 = Usuário (resposta que resolve o nó).

---

## Rodada 1 — Nó-raiz: Propósito (Passo 0)

🤖 **Claude:**
Antes de listar um único ator, a aula crava o nó-raiz no Passo 0: *"sem propósito explícito, o mapa vira lista — não direciona ação."* O `B_relatorio_assistente_v3` oferece vários riscos forenses candidatos a ancorar o mapa. Qual é a *dor* que você quer iluminar?
- Direcionamento / *vendor lock-in* na fase pré-edital (o próprio V3 chama de "ponto cego primordial");
- Falha de fiscalização/ateste na execução (Mapa Zumbi, culpa *in vigilando*/Tema 246, ateste de serviço não prestado);
- Engenharia orçamentária e rastreabilidade (RAP "no apagar das luzes", ruptura PNCP↔SIAFI);
- Ou um propósito panorâmico — ciente de que a aula adverte que isso enfraquece o direcionamento.

👤 **Usuário:**
Nó 1: **Falha de fiscalização/ateste na execução.**

🤖 *Nó resolvido → abre sub-ramos:* centro de gravidade do mapa migra para a Camada 1 (operadores) e para o nó-ponte do ateste. Próximo nó: recorte do objeto.

---

## Rodada 2 — Recorte do objeto contratado

🤖 **Claude:**
O `A_meta_prompt` puxa forte para TIC (PDTI, Comitê de Governança Digital, Integrante Demandante/RD, IN SGD 94/2022), mas o relatório descreve o ciclo geral da Lei 14.133. O mapa é para contratações **de TIC** especificamente, **em geral**, ou **geral com TIC destacado** onde ele adiciona atores próprios?

👤 **Usuário:**
Nó 2: **geral com TIC destacado.**

🤖 *Nó resolvido:* CGD e Integrante Requisitante (RD) entram marcados na Camada 2; reservo gancho para uma eventual camada TIC própria.

---

## Rodada 3 — Visualização das relações (Passo 4)

🤖 **Claude:**
A matriz de Mendelow (Poder × Interesse, Passo 2) entra de qualquer forma. A questão é como tornar visíveis as *relações* (Passo 4): **Cebola/Onion** (camadas concêntricas a partir do núcleo da demanda), **Rede** (nós e arestas, para achar atores-ponte), **Mapa de Influência** (setas de fluxo normativo/financeiro e conflitos), ou combinação?

👤 **Usuário:**
Nó 3: **Onion + Mendelow.**

🤖 *Nó resolvido:* diagrama de cebola como visual principal + matriz de Mendelow; um mapa de influência complementar pode entrar para mostrar o fluxo ateste→pagamento.

---

## Rodada 4 — Profundidade do entregável

🤖 **Claude:**
Entregável **completo** (Passos 0→5 inteiros: níveis concêntricos destrinchados, Mendelow, incentivos/resistências, relações, 5–8 atores-chave, hipóteses e análise de lacunas) ou **enxuto** (5–8 atores-chave + Mendelow + hipóteses)?

👤 **Usuário:**
Nó 4: **completo.**

🤖 *Árvore inicial resolvida.* Produzi o artefato `C_mapa_de_atores_v1.md` (Passos 0→5 + armadilhas + lacunas + governança + pontos cegos).

---

## Rodada 5 — Novo sub-ramo: camada de TIC própria

🤖 **Claude:**
No v1, CGD e Integrante Demandante (RD) ficaram apenas *marcados*. Mas a fiscalização de serviços continuados de TIC tem instrumentos próprios — **Níveis Mínimos de Serviço (NMS/SLA)** e **Instrumento de Medição de Resultado (IMR)** — e modos de falha próprios. Quer uma **camada de TIC dedicada**, destrinchando a fiscalização de SLA via IMR (IN SGD nº 94/2022)?

👤 **Usuário:**
Sim — camada TIC própria, com a fiscalização de SLAs (níveis de serviço, IN SGD 94/2022).

🤖 *Nó resolvido:* criada a seção "Camada TIC", com atores (CGD, SGD/SISP, RD, Integrantes Técnico/Administrativo, EPC, Gestor e Fiscais de TIC, Preposto), instrumentos (NMS, IMR, Modelo de Gestão) e 6 modos de falha (IMR fantasma, captura por assimetria técnica, *uptime* como álibi, posto-de-trabalho vs. resultado, NMS irreal, Mapa de Riscos Zumbi de TIC). Propósito reajustado para incluir o vetor "ateste de SLA sem aferição do IMR" → gerado `C_mapa_de_atores_v2.md`.

---

## Rodada 6 — Formato renderizável

🤖 **Claude:**
O onion está em ASCII. Posso gerar imagem real: **Graphviz/DOT** (clusters aninhados = camadas concêntricas, ideal para o onion) e **Mermaid** (flowchart para o mapa de influência; quadrantChart para Mendelow). Renderizo as imagens aqui na pasta?

👤 **Usuário:**
Sim — renderize os diagramas em imagem (pode instalar/usar Graphviz e gerar os PNGs na pasta).

🤖 *Nó resolvido:* instalado Graphviz (winget) e mermaid-cli (npx). Contornadas duas barreiras: SSL interceptado (Avast) → `NODE_OPTIONS=--use-system-ca`; Chrome 148 incompleto → `puppeteer.json` apontando para o Chrome 149. Gerados `diagramas/onion.png`, `influencia.png`, `mendelow.png` e incorporados ao v2.

---

## Rodada 7 — Novo eixo: camada de auditoria (Modelo das Três Linhas) · *ao vivo*

🤖 **Claude:**
No mapa, a **CGU** está como controle interno e o **TCU** como externo. Mas a **AUDIN** é a **3ª linha** do Modelo das Três Linhas do IIA (2020), internalizado pela IN CGU nº 08/2017 — distinta da 1ª linha (gestão/fiscais que executam o controle) e da 2ª linha (jurídico/conformidade/riscos que supervisionam). Três perguntas:
(1) Quer a AUDIN posicionada explicitamente como 3ª linha, separada da Procuradoria/Jurídico — sabendo que o V3 diz que a alocação do Jurídico entre 1ª/2ª linha "depende da estrutura de cada órgão"?
(2) De quem é a responsabilidade de testar se o ateste tem lastro — da AUDIN (avaliação independente *a posteriori*) ou embutida na 1ª/2ª linha antes do pagamento?
(3) O controle externo (TCU/CGU) deve ser uma 4ª camada sobreposta de avaliação independente, ou fundido com a 3ª linha?

👤 **Usuário:**
1. Sobre a posição da AUDIN e da Procuradoria/Jurídico:
Sim, quero a AUDIN posicionada explicitamente como a 3ª linha do modelo. Ela deve estar totalmente separada da Procuradoria/Jurídico. O Jurídico, no contexto deste mapeamento (especialmente em contratações de TI e serviços de URA), atua predominantemente como 2ª linha (prestando consultoria, avaliando conformidade legal prévia e gerenciando riscos jurídicos) ou até como 1ª linha caso esteja executando atos de gestão específicos. A AUDIN é a única com o papel de avaliação (assurance) independente e objetiva.

2. Sobre a responsabilidade de testar o lastro do ateste:
A responsabilidade primária e intransferível de testar e garantir que o ateste tem lastro físico/lógico é da 1ª linha (especificamente dos Fiscais e Gestores do Contrato), e isso deve ocorrer antes de o pagamento sair. A 2ª linha fornece as ferramentas, as diretrizes de conformidade e a supervisão do processo de ateste. Se a organização depende da AUDIN (3ª linha) para validar atestes antes do pagamento, o modelo de governança está quebrado. A AUDIN avalia o ateste apenas a posteriori, por amostragem e baseada em riscos, para verificar se os controles da 1ª e 2ª linhas estão funcionando adequadamente.

3. Sobre o papel do TCU e da CGU:
Eles não devem ser fundidos com a 3ª linha. O controle externo (TCU) e o órgão central de controle interno do Executivo (CGU - que na visão do órgão auditado atua como um controle de sobreposição) devem aparecer como uma camada externa (external assurance). O Modelo das Três Linhas as posiciona fora da estrutura de gestão da própria organização. Mapeie-os como uma camada superior/sobreposta de avaliação independente de caráter fiscalizatório e sancionatório.

🤖 *Nó resolvido:* o mapa passa a rotular explicitamente **1ª linha** (Fiscais/Gestor — dono intransferível do lastro do ateste, *ex ante*), **2ª linha** (Jurídico/conformidade/riscos — ferramentas e supervisão), **3ª linha** (AUDIN — *assurance* independente, *a posteriori*, por amostragem baseada em risco) e **camada externa de *external assurance*** (TCU + CGU como sobreposição fiscalizatória/sancionatória, fora da estrutura de gestão). Implicação forense: "depender da AUDIN para validar ateste antes do pagamento = governança quebrada".

---

## Rodada 8 — Novo eixo: vozes críticas e controle social · *ao vivo*

🤖 **Claude:**
A aula02 é enfática (slide 37): *"mapas incompletos ignoram quem questiona o serviço — sem essas vozes, o diagnóstico vira confirmation bias, espelho da gestão."* Candidatos: controle social via LAI (12.527/2011), conselhos de usuários (13.460/2017), ouvidorias, jornalismo de dados (Agência Pública, Fiquem Sabendo) e os intermediários paradoxais (que lucram com a complexidade). Três perguntas:
(1) Essas vozes externas entram como atores ativos de rastreabilidade, ou são contexto periférico?
(2) Quer o próprio usuário/área requisitante mapeado como voz crítica (e não só beneficiário passivo)?
(3) Os intermediários paradoxais de TI (consultorias de compliance, fábricas de medição/IMR) são voz crítica, captura, ou os dois?

👤 **Usuário:**
1. Sobre as vozes externas (Controle Social, LAI, Jornalismo de Dados):
Elas devem entrar no mapa como atores ativos de rastreabilidade, e não apenas como contexto periférico. Na administração pública, esses atores funcionam como uma rede descentralizada de auditoria contínua. Ao cruzar dados abertos, investigar históricos de contratos e usar a LAI, eles frequentemente identificam padrões de atestes indevidos ou sobrepreço que as linhas de defesa internas não capturaram. Eles geram a pressão externa que frequentemente se materializa em denúncias e representações formais, forçando o sistema a se corrigir.

2. Sobre a "voz crítica" interna (Área Requisitante / Usuário do Serviço):
Faço questão de que a área requisitante seja mapeada estritamente como voz crítica e validadora, não como beneficiária passiva. Esse é um dos maiores pontos cegos na gestão de contratos, especialmente em iniciativas complexas de tecnologia (como as previstas em um PDTI). É muito comum o fiscal de TI atestar tecnicamente a entrega de uma solução (como painéis gerenciais integrados ou uma nova arquitetura de dados), mas a área de negócio receber um produto disfuncional para a rotina diária. Se não existe um canal formal ou a obrigatoriedade de o requisitante validar o recebimento antes do ateste e da liquidação da despesa, o processo vira um "espelho da gestão" e uma mera formalidade burocrática.

3. Sobre os intermediários paradoxais em TI (Fábricas de Medição e Consultorias de IMR):
Classifique-os primariamente no espectro da captura, atuando sob a fachada de voz crítica. A terceirização da medição de resultados (IMR) ou do "compliance" cria uma falsa sensação de segurança. Na prática, a complexidade excessiva dessas métricas cria uma assimetria de informação que blinda a execução contra questionamentos. Eles geram "falsos positivos de conformidade": o serviço bate todas as métricas artificiais para garantir o faturamento integral, mas não entrega o valor público real. A complexidade, nesse caso, é o próprio mecanismo de captura do orçamento.

🤖 *Nó resolvido:* (a) vozes externas (LAI/controle social/jornalismo de dados) entram como **rede descentralizada de auditoria contínua** — atores ativos que geram denúncias/representações formais; (b) **área requisitante reclassificada de núcleo passivo para voz crítica validadora**, com a tese de um **gate obrigatório: validação do requisitante antes do ateste e da liquidação** (ataca o "ateste técnico OK / negócio disfuncional"); (c) **fábricas de IMR/compliance movidas para o quadrante de captura** ("falsos positivos de conformidade" — a complexidade como mecanismo de captura do orçamento), desmascarando a fachada de voz crítica.

---

## Rodada 9 — Novo eixo: governança do próprio mapa · *ao vivo*

🤖 **Claude:**
A aula02 avisa (slide 49): *"mapa sem dono vira limbo."* Mas há tensão com a Rodada 7: se a AUDIN é 3ª linha (independente, *a posteriori*), pode ela ser dona operacional de um instrumento de gestão sem contaminar a independência? Três perguntas:
(1) Dono do mapa: Alta Administração via Comitê de Governança (Dec. 9.203/2017), AUDIN (com risco de contaminar a 3ª linha), ou arranjo híbrido (gestão é dona, AUDIN audita o uso)?
(2) O Gestor do Contrato está descartado como dono (parte fiscalizada — conflito)? Concorda?
(3) Gatilho de revisão: por evento (auditoria, troca de fornecedor, incidente de ateste) ou por calendário (a cada fase)?

👤 **Usuário:**
1. Sobre o dono do mapa e o conflito da AUDIN:
O arranjo deve ser estritamente o híbrido. A Alta Administração (via Comitê de Governança, atuando como instância de 2ª linha/direcionamento) é a dona institucional e mantenedora do mapa. A AUDIN sob nenhuma hipótese pode ser a dona operacional da ferramenta, sob pena de violação do princípio da independência e risco de auto-revisão (self-review threat). A 3ª linha consome o mapa e audita a eficiência com que a gestão o utiliza e o atualiza, mas a propriedade da ferramenta é exclusiva da gestão.

2. Sobre o Gestor do Contrato como dono:
Concordo integralmente com a exclusão. O Gestor do Contrato é a 1ª linha executiva e o objeto primário da análise de conformidade no ateste. Conceder a ele a propriedade do mapa de atores seria um conflito de interesses direto, permitindo que o fiscalizado defina as fronteiras e os pesos de quem o fiscaliza. Ele deve ser estritamente um usuário das diretrizes do mapa.

3. Sobre o gatilho de revisão do mapa:
A revisão exige uma abordagem combinada, priorizando o evento, mas com rede de segurança por calendário.
O calendário garante a linha de base (ex: revisão anual atrelada a ciclos macro de planejamento, como a atualização do PDTI ou do orçamento). Contudo, os gatilhos primários devem ser orientados a eventos críticos que alteram a dinâmica de forças, tais como: apontamentos graves de auditoria (CGU/TCU), denúncias materializadas via controle social, renovações ou aditivos contratuais que alterem o escopo da medição (IMR), ou a troca do fornecedor principal de tecnologia.

🤖 *Nó resolvido:* governança fixada como **arranjo híbrido** — dona institucional = **Alta Administração via Comitê de Governança** (2ª linha/direcionamento); **AUDIN não é dona** (evita *self-review threat*), apenas consome o mapa e audita o uso/atualização; **Gestor do Contrato = usuário, nunca dono** (fiscalizado não define quem o fiscaliza). Revisão **híbrida**: linha de base por calendário (anual, atrelada a PDTI/orçamento) + gatilhos por evento (apontamento grave de CGU/TCU, denúncia materializada, aditivo que altere o IMR, troca do fornecedor principal de tecnologia).

---

## Rodada 10 — Consolidação (v3) + próximo artefato da cadeia · *ao vivo*

🤖 **Claude:**
A grelha amadureceu, mas o `C_mapa_de_atores_v2.md` ainda não reflete os refinamentos das Rodadas 7–9 (Três Linhas rotuladas + external assurance; requisitante como validador com gate; fábricas de IMR como captura). Duas perguntas: (1) Qual o próximo artefato — (a) fluxo as-is + 3–5 pontos de fricção/failure demand, (b) framework de métricas, (c) análise de lacunas → plano de ação, (d) Design Tree do redesenho? (2) Antes disso, gero um `C_mapa_de_atores_v3` incorporando as Rodadas 7–9, ou sigo direto deixando o v2 como está?

👤 **Usuário:**
Atualize o mapa: Gere o C_mapa_de_atores_v3
Sim, consolide o v3 antes de avançar. Você não deve seguir em frente deixando a versão 2 como a "oficial", pois o v2 agora está defasado em relação ao seu próprio entendimento do problema. A definição de que o requisitante é um "validador com gate obrigatório" e não apenas um beneficiário passivo altera completamente as permissões e o fluxo de ateste.
Gere o v3 para que o próximo agente (ou o próximo prompt) herde esse contexto refinado. Se você alimentar o próximo passo com o v2, a IA vai gerar um fluxo baseado na premissa antiga, e você perderá todo o ganho das rodadas 7 a 9.

2. O Próximo Artefato: Opção (A)
O seu próximo passo lógico na esteira de Design de Serviços / Auditoria é a (a) Mapa do fluxo atual (as-is) + 3–5 pontos de fricção / failure demand.
Por que as outras opções vêm depois?
(d) Design Tree do redesenho: Você não pode redesenhar a arquitetura (focando no "ateste frouxo") sem antes desenhar exatamente onde e como o ateste atual é feito no tempo e no espaço.
(b) Framework de métricas e (c) Plano de Ação: Só faz sentido medir ou planejar ações corretivas depois de enxergar o gargalo visualmente no fluxo as-is.
O objetivo agora é pegar esses atores do v3 e colocá-los em movimento. O fluxo as-is vai mostrar, na prática da URA, o momento exato em que o cidadão desliga a ligação frustrado (failure demand), o momento em que o sistema gera o relatório de chamadas, e o momento em que a 1ª linha (gestor) assina o ateste sem consultar o requisitante.

🤖 *Nó resolvido:* gerar **`C_mapa_de_atores_v3`** consolidando as Rodadas 7–9 antes de avançar (o requisitante-validador com gate redefine permissões e fluxo de ateste — não pode ser herdado defasado). Próximo artefato confirmado = **(a) fluxo as-is + 3–5 pontos de fricção/failure demand**, que põe os atores do v3 "em movimento" no tempo/espaço antes de qualquer redesenho, métrica ou plano. *Observação registrada:* o usuário citou o cenário da **URA (Seguro-Desemprego)** como exemplo do as-is — a definir, na próxima grelha, se o fluxo as-is mapeia a jornada de **contratações/ateste** (objeto deste mapa) ou a jornada da **URA** (exercício da aula02).

---

## Rodada 11 — Ordenador de Despesa e a cadeia orçamentário-financeira · *ao vivo*

🤖 **Claude:**
O Ordenador ordena a liquidação e o pagamento — ato final que retira o dinheiro do cofre — o que levanta tensão de segregação de funções. Três perguntas:
(1) Posição nas Três Linhas: o Ordenador é 1ª linha (atos de gestão) ou autoridade decisória distinta? Tem dever próprio de verificar o lastro antes de liquidar, ou confia no ateste do fiscal?
(2) Trago o Coordenador Orçamentário (empenho/RAP) e a STN como atores, ou ficam como "regras de fundo"?
(3) O STF / Justiça do Trabalho (Tema 246) entra como ator (judiciário) ou permanece só como norma citada?

👤 **Usuário:**
1. Sobre o Ordenador de Despesa e a segregação de funções:
O Ordenador de Despesa pertence estritamente à 1ª Linha (Execução/Gestão). Ele é a autoridade máxima da execução orçamentária. Não há conflito em colocá-lo na mesma linha que o Gestor/Fiscal, pois a segregação de funções ocorre dentro da própria 1ª linha (quem atesta não é quem ordena o pagamento).
Quanto à responsabilidade (na visão do TCU): o Ordenador não tem o dever de refazer a validação técnica/física do ateste. Sua confiança no fiscal é legítima, desde que não seja cega. O Ordenador responde solidariamente se autorizar a liquidação com vícios formais evidentes, ausência de pareceres obrigatórios (da 2ª linha), ou por omissão grave (culpa in eligendo/vigilando). O ateste do fiscal garante o lastro fático; o Ordenador garante a regularidade processual e orçamentária.

2. Sobre a Cadeia Orçamentária (Coordenador Orçamentário, STN e RAP):
Traga o Coordenador Orçamentário/Setor Financeiro como um ator ativo no mapa (na 1ª linha). Ele é o operador real que sofre a pressão do ponto de fricção F4 (fechamento de exercício e inscrição em RAP).
Por outro lado, mantenha a STN (Secretaria do Tesouro Nacional) apenas como "regra de fundo" / restrição sistêmica. Inserir a STN como ator ativo no fluxo as-is da URA vai poluir o diagrama. A STN dita as regras do jogo e os limites via SIAFI, mas não opera a esteira diária de ateste e liquidação dessa contratação.

3. Sobre a Régua Judicial (STF / Tema 246 e passivo trabalhista):
O Judiciário deve permanecer fora das raias de atores ativos, figurando apenas como norma/contexto de risco. O fluxo as-is mapeia a operação do serviço e o controle. O Judiciário não é uma linha de defesa; ele é a instância de responsabilização que atua quando o Modelo de Três Linhas falha catastroficamente. O Tema 246 (responsabilidade subsidiária) é a consequência financeira grave da failure demand na fiscalização, não uma etapa do processo.

🤖 *Nó resolvido:* (a) **Ordenador de Despesa = 1ª linha** (autoridade máxima da execução orçamentária); **segregação de funções ocorre *dentro* da 1ª linha** — quem atesta ≠ quem ordena o pagamento. Confiança legítima (não cega) no ateste: ateste = **lastro fático** (fiscal); Ordenador = **regularidade processual/orçamentária**; responde solidariamente por vício formal evidente, ausência de parecer obrigatório (2ª linha) ou omissão grave. (b) **Coordenador Orçamentário/Setor Financeiro = ator ativo (1ª linha)** — operador que sofre a pressão do F4 (RAP); **STN = regra de fundo/restrição sistêmica via SIAFI** (não-ator). (c) **STF/Judiciário (Tema 246) = norma/contexto de risco** (não-ator) — instância de responsabilização *ex post*, não linha de defesa nem etapa do processo.

---

## Síntese da árvore de decisão (estado final)

| # | Nó / Eixo | Decisão | Efeito no artefato |
|---|---|---|---|
| 1 | Propósito (Passo 0) | Falha de fiscalização/ateste na execução | Centro de gravidade na Camada 1 e no nó-ponte do ateste |
| 2 | Recorte | Geral com TIC destacado → depois camada TIC própria | Seção dedicada de TIC (IN SGD 94/2022) |
| 3 | Visualização | Onion + Mendelow (+ mapa de influência) | 3 diagramas |
| 4 | Profundidade | Completo | Passos 0→5 + armadilhas + lacunas + governança + pontos cegos |
| 5 | Camada TIC | NMS/SLA via IMR | 6 modos de falha próprios de TIC |
| 6 | Renderização | Graphviz + Mermaid → PNG | `diagramas/*.png` incorporados |
| 7 | Auditoria (Três Linhas) | 1ª/2ª/3ª linha rotuladas + TCU/CGU como *external assurance* sobreposta | Camadas relabeladas; lastro do ateste = 1ª linha *ex ante*; AUDIN só *a posteriori* |
| 8 | Vozes críticas | Externas = rede de auditoria contínua; **requisitante = validador com gate**; fábricas de IMR = **captura** | Requisitante sai do núcleo passivo; gate antes do ateste; IMR no quadrante de captura |
| 9 | Governança | **Híbrido**: dono = Alta Adm/Comitê; AUDIN não-dona (*self-review*); Gestor = usuário | Revisão híbrida (calendário + evento) |
| 10 | Consolidação + próximo | Gerar **v3** antes de avançar; próximo = **(a) fluxo as-is** | v3 consolida R7–R9; as-is enfileirado |
| 11 | Cadeia orçamentário-financeira | Ordenador = 1ª linha (segregação dentro da 1ª linha); Coord. Orçamentário = ator ativo; STN e Judiciário/Tema 246 = não-atores (regra de fundo / norma de risco) | +2 atores no mapa final; STN/Judiciário como contexto |
