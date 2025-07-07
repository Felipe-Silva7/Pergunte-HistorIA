# Estratégias de Prompt para "Pergunte HistórIA"

Para otimizar as respostas da sua Inteligência Artificial em história, definimos estratégias de prompt específicas para cada categoria de perguntas. Essas abordagens visam garantir precisão, concisão e a profundidade adequada para o público do Ensino Médio e ENEM.

---

### 1. Grandes Períodos e Eventos Históricos

**Estratégia de Prompt Ideal:** **Cadeia de Pensamento (Chain of Thought - CoT)**

**Por que é ideal:** A estratégia de **Cadeia de Pensamento (CoT)** instrui a IA a detalhar seu processo de raciocínio passo a passo antes de fornecer a resposta final. Para perguntas sobre grandes períodos e eventos, isso é extremamente útil porque:

1.  **Eventos Complexos:** Muitos eventos históricos (como a queda de Roma ou a Primeira Guerra Mundial) têm múltiplas causas, consequências e interconexões. A CoT permite que a IA "pense" através dessas complexidades (ex: "identificar causas primárias", "listar fatores contribuintes", "sintetizar impactos") antes de formular a resposta.
2.  **Estrutura Lógica:** Garante que a resposta siga uma estrutura lógica, abordando os pontos essenciais (o que foi, quando, onde, por que, consequências principais) de forma organizada.
3.  **Redução de Alucinações:** Ao forçar a IA a justificar cada etapa de sua resposta internamente, a CoT ajuda a reduzir a probabilidade de "alucinações" ou informações incorretas, pois ela precisa seguir um caminho de raciocínio validado.
4.  **Respostas Concisas e Diretas:** Mesmo que o processo interno seja detalhado, a instrução final pode ser para apresentar a **síntese** dessa cadeia de pensamento de forma concisa, como nos exemplos que você forneceu.

**Exemplos de Prompts para a IA:**

1.  **Prompt para perguntas sobre Causas de Eventos Complexos:**
    ```
    Para a pergunta sobre as causas de um evento histórico (ex: "Qual foi a principal causa da queda do Império Romano do Ocidente?"), responda seguindo o seguinte roteiro:
    * Identifique o evento e o período.
    * Busque e liste as causas amplas envolvidas.
    * Detalhe as principais sub-causas ou fatores contribuintes.
    * Sintetize a natureza da causa: se foi única, múltipla, ou um processo gradual.
    * Formule a resposta concisa, utilizando as informações sintetizadas.
    ```

2.  **Prompt para perguntas sobre Características de Movimentos/Períodos:**
    ```
    Para a pergunta sobre as características de um movimento ou período (ex: "O que foi o Renascimento e quais suas características principais?"), responda detalhando:
    * Definição do movimento/período: O que foi e quando ocorreu.
    * Principais características: Liste e explique brevemente as 3-5 características mais importantes.
    * Formule uma resposta direta que abranja a definição e as características principais.
    ```

3.  **Prompt para perguntas sobre Importância/Impacto de Eventos:**
    ```
    Para a pergunta sobre a importância ou impacto de um grande evento (ex: "Qual a importância da Revolução Francesa para o mundo contemporâneo?"), responda focando em:
    * O evento e seu período.
    * Quais ideais ou mudanças fundamentais o evento introduziu.
    * Como esses ideais/mudanças influenciaram ou se espalharam para outras regiões/períodos.
    * Sintetize a sua relevância duradoura de forma concisa.
    ```

---

### 2. Conceitos e Termos Históricos

**Estratégia de Prompt Ideal:** **Modelo/Exemplo (Few-shot/In-context Learning)**

**Por que é ideal:** A estratégia de **Modelo/Exemplo** (também conhecida como Few-shot ou In-context Learning) funciona fornecendo à IA um ou mais exemplos de pares pergunta-resposta diretamente no prompt. Para a definição de conceitos, isso é altamente eficaz porque:

1.  **Padrão de Resposta Clara:** Termos e conceitos geralmente exigem uma definição direta e concisa. Ao mostrar exemplos de como esses conceitos devem ser explicados (o termo, sua essência, principais características), a IA aprende o "formato" desejado para a resposta.
2.  **Consistência:** Garante que todas as definições sigam um padrão similar de clareza e profundidade, facilitando a compreensão do usuário.
3.  **Eficiência:** Para definições, uma CoT pode ser excessiva. O modelo permite que a IA vá direto ao ponto, replicando o estilo e a estrutura dos exemplos.
4.  **Redução de prolixidade:** A IA entende que não deve divagar, mas sim focar na explicação essencial do termo.

**Exemplos de Prompts para a IA:**

1.  **Prompt para Definição Básica de Termos:**
    ```
    Siga o padrão abaixo para definir termos históricos:
    Pergunta: O que é [TERMO]?
    Resposta: [TERMO] é [definição concisa], caracterizado por [1-2 características principais].
    Exemplo:
    Pergunta: O que é o Iluminismo?
    Resposta: O Iluminismo foi um movimento intelectual e filosófico que surgiu na Europa no século XVIII, conhecido como o "Século das Luzes". Ele defendia o uso da **razão** para combater o obscurantismo e o absolutismo, buscando a liberdade de pensamento, a igualdade social e a crítica à Igreja e ao Antigo Regime.
    ```

2.  **Prompt para Diferenciação de Conceitos:**
    ```
    Ao diferenciar dois conceitos históricos, utilize a seguinte estrutura:
    Pergunta: Diferencie [CONCEITO A] e [CONCEITO B].
    Resposta: [CONCEITO A] foi [definição A], caracterizado por [características A]. Já [CONCEITO B], por sua vez, foi [definição B], baseado em [características B].
    Exemplo:
    Pergunta: Diferencie Feudalismo e Capitalismo.
    Resposta: O **Feudalismo** foi um sistema socioeconômico predominante na Europa medieval, caracterizado pela relação de suserania e vassalagem, economia agrária de subsistência e poder descentralizado. O **Capitalismo**, por sua vez, é um sistema econômico baseado na propriedade privada dos meios de produção, busca pelo lucro, livre concorrência e economia de mercado, predominante na modernidade e contemporaneidade.
    ```

3.  **Prompt para Explicação de Conceitos Específicos/Eventos Pontuais:**
    ```
    Para perguntas sobre o significado de conceitos ou eventos específicos:
    Pergunta: O que significa "[CONCEITO/EVENTO]"?
    Resposta: "[CONCEITO/EVENTO]" refere-se a [definição principal]. Seu objetivo/contexto era [propósito/contexto]. Pode incluir [uma característica ou consequência notável].
    Exemplo:
    Pergunta: O que significa "Revolução Verde"?
    Resposta: A Revolução Verde foi um conjunto de inovações e técnicas agrícolas introduzidas a partir da metade do século XX, especialmente em países em desenvolvimento. Seu objetivo era aumentar a produção de alimentos por meio do uso de **sementes geneticamente modificadas, fertilizantes, agrotóxicos e maquinário agrícola**, embora tenha gerado debates sobre seus impactos ambientais e sociais.
    ```

---

### 3. Figuras Históricas Marcantes

**Estratégia de Prompt Ideal:** **Básico com Restrições (Basic Prompt with Constraints)**

**Por que é ideal:** Uma abordagem de **Prompt Básico com Restrições** é eficaz aqui. Você define claramente o que a IA deve buscar e incluir na resposta, sem a necessidade de um raciocínio complexo passo a passo (CoT) ou múltiplos exemplos para um padrão (Modelo).

1.  **Foco nos Pontos Chave:** Permite especificar que a resposta deve incluir quem foi a pessoa, o que ela fez de significativo e qual seu impacto ou legado.
2.  **Concisão e Direcionamento:** Garante que a resposta seja direta e não se desvie para detalhes biográficos irrelevantes para o contexto do ensino médio/ENEM.
3.  **Evitar Generalizações:** As restrições podem orientar a IA a focar na **contribuição histórica específica** da figura, e não apenas em aspectos gerais de sua vida.

**Exemplos de Prompts para a IA:**

1.  **Prompt para Papel de Personalidades em Eventos:**
    ```
    Para perguntas sobre o papel de uma figura histórica em um evento (ex: "Qual foi o papel de D. Pedro I na Independência do Brasil?"), responda em até 3 frases, cobrindo:
    * Identificação: Quem foi a pessoa.
    * Ação Principal: O que ela fez especificamente no evento.
    * Consequência/Legado Direto: O resultado imediato de suas ações.
    ```

2.  **Prompt para Importância Geral de Lideranças:**
    ```
    Para perguntas sobre a importância geral de uma liderança (ex: "Quem foi Getúlio Vargas e qual sua importância na história brasileira?"), responda focando em:
    * Identificação e Período de Atuação.
    * Principais áreas de impacto/reformas/políticas: Mencione 2-3 pontos cruciais.
    * Legado duradouro: Por que sua atuação foi importante.
    ```

3.  **Prompt para Símbolos de Causas/Movimentos:**
    ```
    Para perguntas sobre figuras que simbolizam causas (ex: "Por que Mahatma Gandhi é considerado um símbolo de resistência pacífica?"), responda abordando:
    * Quem foi e a causa que representou.
    * Métodos ou filosofia principal que o tornou um símbolo.
    * Resultado/Impacto de sua luta.
    ```

---

### 4. Relações entre História e Atualidade

**Estratégia de Prompt Ideal:** **Cadeia de Pensamento (Chain of Thought - CoT) com Enfoque em Conexão**

**Por que é ideal:** Assim como a primeira categoria, esta também se beneficia enormemente da **Cadeia de Pensamento**, mas com um enfoque específico na **conexão entre passado e presente**.

1.  **Análise Causal:** Exige que a IA não apenas descreva o evento histórico, mas também trace as linhas de causalidade até as manifestações atuais.
2.  **Pensamento Crítico:** Estimula a IA a identificar as **repercussões duradouras** e a explicar como eventos passados continuam a moldar a realidade contemporânea (ex: "identificar o evento histórico", "analisar suas consequências diretas", "traçar desdobramentos para o presente", "sintetizar a relevância atual").
3.  **Complexidade das Relações:** A conexão entre história e atualidade raramente é linear. A CoT permite que a IA explore nuances e múltiplas dimensões dessa relação.
4.  **Evitar Respostas Simplistas:** Garante que a resposta não seja apenas uma afirmação de que há uma conexão, mas uma explicação de *como* essa conexão se manifesta.

**Exemplos de Prompts para a IA:**

1.  **Prompt para Impacto de Regimes Políticos no Presente:**
    ```
    Para perguntas sobre o impacto de regimes passados na atualidade (ex: "Como o período da ditadura militar no Brasil (1964-1985) ainda impacta a sociedade brasileira hoje?"), responda seguindo o roteiro:
    * Identifique o regime/período histórico.
    * Liste as características mais marcantes do período.
    * Analise em quais áreas da sociedade atual (política, social, econômica, cultural) esse impacto é percebido.
    * Descreva como a herança do passado se manifesta no presente.
    * Formule a resposta de forma sintética e clara.
    ```

2.  **Prompt para Influência de Processos Históricos Amplos:**
    ```
    Para perguntas sobre a influência de processos históricos de longa duração (ex: "De que forma a colonização da América Latina influencia sua realidade atual?"), responda com a seguinte estrutura:
    * Defina o processo histórico em questão (e seu período).
    * Aponte as principais características/consequências desse processo na época.
    * Trace as linhas de continuidade: Como essas características iniciais se mantiveram ou se transformaram até o presente.
    * Mencione exemplos específicos de influência atual (ex: estruturas sociais, problemas, cultura).
    * Apresente uma resposta concisa que conecte passado e presente.
    ```

3.  **Prompt para Relevância Histórica de Desafios Atuais:**
    ```
    Para perguntas que conectam eventos passados a desafios contemporâneos (ex: "Como a Revolução Industrial afetou o meio ambiente e por que isso é relevante hoje?"), a IA deve:
    * Identificar o evento histórico e seu impacto inicial.
    * Descrever os desdobramentos desse impacto ao longo do tempo.
    * Explicar a relevância atual: Por que as consequências daquele evento ainda são importantes para os desafios contemporâneos.
    * Formule a resposta de maneira clara e direta.
    ```

---

### 5. Metodologia e Fontes Históricas

**Estratégia de Prompt Ideal:** **Conhecimento Gerado (Knowledge Generation)**

**Por que é ideal:** Para esta categoria, que lida com conceitos mais "metodológicos" da história, a estratégia de **Conhecimento Gerado** é muito potente. A IA é instruída a primeiro **gerar internamente** informações relevantes sobre o tópico (ex: "o que é fonte primária", "o que é arqueologia", "quais os passos do historiador") e só então usar esse conhecimento para formular a resposta.

1.  **Precisão Conceitual:** Garante que a IA opere a partir de um entendimento construído dos conceitos metodológicos, evitando imprecisões.
2.  **Autonomia na Explicação:** Permite que a IA construa a explicação a partir de "dados brutos" que ela mesma organiza, resultando em respostas mais robustas.
3.  **Clareza e Organização:** Ao gerar o conhecimento internamente e depois sintetizá-lo, a IA pode produzir respostas bem estruturadas e fáceis de entender.

**Exemplos de Prompts para a IA:**

1.  **Prompt para Diferença entre Tipos de Fontes:**
    ```
    Para perguntas que pedem a diferença entre tipos de fontes históricas (ex: "Qual a diferença entre fonte histórica primária e secundária?"), siga o roteiro:
    * Gere internamente a definição de 'fonte primária' e forneça exemplos.
    * Gere internamente a definição de 'fonte secundária' e forneça exemplos.
    * Sintetize a distinção entre elas, focando na origem e propósito.
    * Formule a resposta concisa com base nessa síntese.
    ```

2.  **Prompt para Contribuição de Disciplinas Auxiliares da História:**
    ```
    Para perguntas sobre como outras disciplinas contribuem para a história (ex: "Como a arqueologia contribui para o estudo da história?"), a IA deve:
    * Gere internamente a definição da disciplina (ex: arqueologia).
    * Gere internamente os métodos ou objetos de estudo dessa disciplina.
    * Conecte diretamente como esses métodos/objetos fornecem informações para a história.
    * Formule a resposta explicando a contribuição de forma clara.
    ```

3.  **Prompt para o Papel de Agentes no Estudo Histórico:**
    ```
    Para perguntas sobre o papel de historiadores ou o processo de escrita da história (ex: "Qual o papel do historiador na construção do conhecimento histórico?"), a IA deve:
    * Gere internamente o conceito do agente (ex: historiador) ou do processo (ex: historiografia).
    * Liste as principais ações ou funções desse agente/processo.
    * Descreva o resultado ou o impacto dessas ações na compreensão da história.
    * Apresente a resposta de forma direta e explicativa.
    ```