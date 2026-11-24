# Roteiro Completo do Vídeo de Apresentação Final — Rede Lilás
**Projeto Integrador — 2º Semestre de 2026 (Desenvolvimento Móvel & Data Science)**  
**Professor:** Alex Junior Nunes · **Universidade Positivo (Londrina)**  
**Equipe:** Rede Lilás — **Mateus Zichack** e **Samuel Augusto**  
**Duração Máxima Total (2 alunos):** **12 min 30s** *(meta recomendada: ~10 min 45s para ter margem de segurança)*

---

## 0. Regras Rígidas do Edital (LEIA ANTES DE GRAVAR — ISSO VALE NOTA!)

1. **REGRA DO TEMPO (ZERO TOLERÂNCIA):** tudo o que for falado ou mostrado **depois** do limite daquela fase é **automaticamente ignorado na nota** (nem 2 segundos de tolerância!). Usem um cronômetro visível ao lado da tela e **terminem 10–15 segundos antes do teto**.
2. **REGRA DA IDENTIFICAÇÃO (OBRIGATÓRIA):** no início de **CADA** segmento das Fases 2, 3 e 4, é obrigatório:
   * Mostrar um **cartão de texto na tela** (slide simples, overlay ou tela cheia do Bloco de Notas) escrito:
     * `Fase 1 — Visão Geral (Rede Lilás)`
     * `Fase 2 — Mateus Zichack` / `Fase 2 — Samuel Augusto`
     * `Fase 3 — Mateus Zichack` / `Fase 3 — Samuel Augusto`
     * `Fase 4 — Mateus Zichack` / `Fase 4 — Samuel Augusto`
   * **Dizer o nome completo claramente em voz alta** (*"Meu nome é Mateus Zichack..."* / *"Meu nome é Samuel Augusto..."*). Quem esquecer o nome completo no começo do trecho **zera aquele trecho**!
3. **REGRA DO VÍDEO ÚNICO:** podem gravar separados, mas precisam juntar tudo em **um único vídeo no YouTube** (configurado como **Público** ou **Não listado** — **NUNCA Privado!**), exatamente nesta ordem:
   `Fase 1` $\rightarrow$ `Fase 2 (Mateus)` $\rightarrow$ `Fase 2 (Samuel)` $\rightarrow$ `Fase 3 (Mateus)` $\rightarrow$ `Fase 3 (Samuel)` $\rightarrow$ `Fase 4 (Mateus)` $\rightarrow$ `Fase 4 (Samuel)`.
4. **REGRA DO BLACKBOARD:** conforme o aviso do professor na tarefa, **CADA INTEGRANTE (Mateus E Samuel)** precisa enviar a entrega na sua conta do Blackboard colando o link do vídeo no YouTube!
5. **⚠️ ALERTA MÁXIMO SOBRE A FASE 4 (`https://apiwp.smartcortex.ai:8888/`):**
   * **NUNCA acesse esse site com seu RGM antes de começar a gravar a Fase 4!**
   * O acesso pelo RGM é **único e irreversível** (não tem reset).
   * Toda a Fase 4 de cada aluno precisa ser gravada em **UMA ÚNICA TOMADA, SEM CORTES INTERNOS**: abrir o site $\rightarrow$ digitar o RGM na tela $\rightarrow$ clicar em gerar pergunta $\rightarrow$ ler em voz alta $\rightarrow$ responder mostrando o código/notebook.
   * Você tem **2 chances** (se não souber a 1ª pergunta, gere a 2ª na mesma tomada sem cortar o vídeo).

---

## 1. Preparação Antes de Apertar REC

Antes de gravar, deixem tudo rodando localmente (sem depender de internet ao vivo nas Fases 1–3):
* **Terminal 1 (`api/`):** `npm start` $\rightarrow$ rodando em `http://localhost:3333`
* **Terminal 2 (`app/`):** `npx expo start` + tecla `w` $\rightarrow$ aberto no navegador na tela de disfarce (*Minha Lista Diária*)
* **Aba 2 do navegador:** `http://localhost:3333/delegacia` (Painel Web da Delegacia já carregado)
* **VS Code aberto** com as abas de código de cada integrante já prontas + `data-science/notebook.ipynb` aberto e visível
* **OBS Studio / gravador de tela** gravando tela inteira + microfone (testar o áudio antes!)
* **Cronômetro** visível no celular ou em outra tela

---

## 2. FASE 1 — Visão Geral do Projeto
* **Quem fala:** Mateus Zichack *(apenas 1 integrante fala nesta fase)*
* **Limite máximo:** **1 min 30s (fixo)** | **Meta de fala:** **1 min 15s**
* **Cartão na tela (2s):** `Fase 1 — Visão Geral | Grupo Rede Lilás`
* **O que mostrar na tela:** Tela inicial do disfarce (*Minha Lista Diária*) e, rapidamente, a tela principal lilás após abrir.

### Fala pronta (Mateus — leia em ritmo natural, ~1 min 15s):
> "Olá, professor! Eu sou o **Mateus Zichack** e, junto com o **Samuel Augusto**, formamos a equipe **Rede Lilás** do Projeto Integrador de Desenvolvimento Móvel e Data Science.
>
> O nosso aplicativo camuflado usa como disfarce a **'Minha Lista Diária'**, uma lista de compras de supermercado totalmente funcional. Escolhemos esse disfarce porque é um app comum no celular de qualquer pessoa, não desperta suspeitas caso o agressor pegue o aparelho e permite que a usuária acesse a área segura digitando o código secreto `1800` na barra de busca ou segurando o título.
>
> Por trás do disfarce, o sistema integra back-end em Node.js/Express, aplicativo React Native/Expo, Painel Web da Delegacia em tempo real e um modelo de Data Science sobre dados reais do DataSUS. As funcionalidades principais são: botão de emergência SOS com geolocalização e canais 180 e 190, Rede de Contatos de Confiança, Diário Seguro de Ocorrências, Pontos de Acolhimento em Londrina, Autoavaliação de Risco e Saída Rápida em um toque.
>
> Sobre os desafios éticos do tema: tivemos extremo cuidado para nunca coletar dados pessoais reais de vítimas — usamos apenas a base pública agregada do SINAN/DataSUS em conformidade com a LGPD —, removemos qualquer confirmação na Saída Rápida para não atrasar a fuga em perigo real e incluímos em todas as telas de risco o aviso explícito de que se trata de um protótipo acadêmico."

---

## 3. FASE 2 — Demonstração Ao Vivo das Telas (CRUDs + Indicador de Data Science)
* **Limite máximo:** **2 min por aluno** | **Meta:** **1 min 40s – 1 min 45s por aluno**
* *Lembrar: como ambos cursam Data Science, cada um precisa demonstrar seu CRUD completo (Create, Read, Update, Delete na API real) **e** mostrar onde o indicador de Data Science aparece no app!*

---

### Bloco 2A — Mateus Zichack (Meta: 1 min 45s)
* **Cartão na tela (2s):** `Fase 2 — Mateus Zichack`
* **Telas mostradas ao vivo:** `TelaDisfarce` $\rightarrow$ Aba `Rede Apoio` $\rightarrow$ Aba `Locais` $\rightarrow$ Aba do navegador `http://localhost:3333/delegacia`

#### Passo a passo + Fala pronta (Mateus):
1. **[0:00 – 0:15] Identificação + Entrada no Disfarce:**
   > "Meu nome é **Mateus Zichack**. Eu sou responsável pelos CRUDs de **Rede de Apoio (Contatos de Confiança)** e **Pontos de Acolhimento**, além da tela de disfarce. Vou digitar `1800` na busca da lista de compras para desbloquear a área segura." *(digita `1800`, abre o app)*
2. **[0:15 – 1:15] CRUD Completo de Contatos consumindo a API real (`POST`, `GET`, `PUT`, `DELETE`):**
   * *(clica na aba **Rede Apoio**)*
   > "Aqui na aba **Rede Apoio**, essa lista já vem direto da nossa API Node.js via `GET /contatos` — não há mais dados mocados.
   > Vou demonstrar o **Create**: clico em *Adicionar Contato de Confiança*, preencho nome *Carla Mendes*, parentesco *Vizinha*, telefone *(43) 99988-7766*, Prioridade 1 e salvo." *(salva — confirma `POST /contatos`, volta pra lista e mostra Carla listada = **Read**)*
   > "Agora o **Update**: toco no card da Carla para editar, mudo para Prioridade 2 e atualizo — ou posso alternar o alerta automático de SMS direto na lista via `PUT /contatos/:id`." *(salva edição e mostra atualizado)*
   > "Por fim, o **Delete**: clico na lixeira ao lado da Carla, confirmo e o registro é removido do JSON na API via `DELETE /contatos/:id`." *(remove)*
3. **[1:15 – 1:45] Pontos de Acolhimento + Indicador de Data Science no App:**
   * *(clica na aba **Locais**)*
   > "Também cuido da aba **Locais**, carregada via `GET /pontos`, listando delegacia da mulher, CREAS, Casa Abrigo e Defensoria em Londrina e Cambé. Reparem neste selo lilás em cada card: ele traz o dado real da nossa análise no **SINAN/DataSUS** — em Londrina a taxa regional de reincidência é de **59,38%**, e em Cambé chega a **72,02%**. Isso ajuda a usuária e a rede de apoio a dimensionar a gravidade regional, sempre lembrando que é um indicador estatístico acadêmico."

---

### Bloco 2B — Samuel Augusto (Meta: 1 min 45s)
* **Cartão na tela (2s):** `Fase 2 — Samuel Augusto`
* **Telas mostradas ao vivo:** Aba `Diário` $\rightarrow$ Aba `Avaliação` $\rightarrow$ Aba `Início / SOS` + `Painel da Delegacia` $\rightarrow$ Botão `Sair` (Quick Exit)

#### Passo a passo + Fala pronta (Samuel):
1. **[0:00 – 0:15] Identificação + Responsabilidade:**
   > "Meu nome é **Samuel Augusto**. Eu sou responsável pelos CRUDs do **Diário Seguro de Ocorrências**, dos **Alertas SOS**, pela **Saída Rápida** e pela integração da **Autoavaliação de Risco** com o modelo de Data Science."
2. **[0:15 – 1:05] CRUD Completo do Diário + Relacionamento FK + Selo DS (`POST`, `GET`, `PUT`, `DELETE`):**
   * *(na aba **Diário**)*
   > "A lista do Diário vem de `GET /ocorrencias`. Vou **criar** um novo registro: escolho violência *Psicológica*, gravidade *Alta*, escrevo um relato de teste e vinculo ao ponto de apoio **DEAM Londrina** — esse vínculo é uma chave estrangeira validada de verdade na API." *(salva `POST /ocorrencias`)*
   > "Ao voltar à lista, o card já aparece com o ponto vinculado e com o selo **'Risco estimado (DS): Alto'**, calculado pela nossa API usando o modelo de Data Science, junto do aviso acadêmico no rodapé. Vou **editar** tocando no card para mudar a gravidade para *Média* (`PUT /ocorrencias/:id`), e agora **excluir** na lixeira (`DELETE /ocorrencias/:id`)." *(edita e exclui)*
3. **[1:05 – 1:45] Autoavaliação (Modelo DS) + SOS no Painel Web + Saída Rápida:**
   * *(clica na aba **Avaliação**)*
   > "Na aba **Avaliação**, mostramos as métricas reais do nosso modelo **Random Forest** (Recall de 71,1% e ROC-AUC 0,610) e o aviso obrigatório de que é uma estimativa acadêmica. Ao responder e calcular, a API combina as respostas com a probabilidade regional do DataSUS para Londrina e salva em `POST /avaliacoes`." *(mostra resultado rápido ou avaliação salva)*
   * *(clica em **Início / SOS**, dispara 1 alerta SOS, mostra rapidamente a aba `http://localhost:3333/delegacia` atualizando via polling, e volta ao app)*
   > "No Início, ao disparar o **Alerta SOS**, ele chega automaticamente no Painel Web da Delegacia em tempo real. E de qualquer tela, um único toque no botão vermelho **Sair** no topo ativa a **Saída Rápida**, fechando tudo sem confirmação de volta para a lista de compras." *(clica em **Sair** — volta para *Minha Lista Diária*)*

---

## 4. FASE 3 — Explicação do Código-Fonte + Pipeline de Data Science
* **Limite máximo:** **2 min por aluno** | **Meta:** **1 min 45s por aluno**
* **Ambiente:** VS Code com os arquivos já abertos em abas na ordem abaixo!

---

### Bloco 3A — Mateus Zichack (Meta: 1 min 45s)
* **Cartão na tela (2s):** `Fase 3 — Mateus Zichack`
* **Abas pré-abertas no VS Code:**
  1. `app/src/servicos/api.js`
  2. `app/src/screens/rede/ListaContatosScreen.js`
  3. `api/server.js` (linhas 103–235)
  4. `data-science/notebook.ipynb` (Seções 1 a 4)

#### Passo a passo + Fala pronta (Mateus):
1. **[0:00 – 0:55] Código Mobile + API REST:**
   > "Meu nome é **Mateus Zichack**. Vou mostrar como implementamos o consumo REST e o back-end da minha parte.
   > Aqui em `app/src/servicos/api.js` (linha 16), centralizamos todas as requisições na função `requisitar`, que faz o `fetch` para o Express e converte erros HTTP 400/404 em exceções tratadas no app.
   > Em `ListaContatosScreen.js`, usamos o `useFocusEffect` para chamar `listarContatos()` toda vez que a tela ganha foco, sem `mockData`.
   > No back-end `api/server.js` (linha 103), criamos a função `criarRotasCrud`, que gera as 5 rotas RESTful (`GET`, `GET/:id`, `POST`, `PUT/:id`, `DELETE/:id`) persistindo em JSON. Na rota `/contatos` (linha 213), além de validar nome, telefone e prioridade (1, 2 ou 3), a função `validarUsuariaExiste` (linha 177) checa a chave estrangeira `usuariaId` contra `usuarias.json` e devolve status **400** se a usuária não existir."
2. **[0:55 – 1:45] Notebook de Data Science (Governança, 5 Dimensões, Tratamento e EDA):**
   * *(troca para a aba `data-science/notebook.ipynb`, rolando Seções 1 a 4)*
   > "Na trilha de Data Science, fiquei responsável por **Governança, Qualidade e EDA**. Trabalhamos com a base pública real do **SINAN Net / DataSUS** do Paraná (2023 a 2025), agregada por município para respeitar a LGPD.
   > Na Seção 3, diagnosticamos as **5 dimensões de qualidade**: o arquivo Tabnet veio em Latin-1 com 5 linhas de cabeçalho, 15 de notas de rodapé, 232 traços `'-'` representando zero e uma linha resumo `'Total'` que duplicaria a soma estadual. No tratamento, separamos código IBGE e município, imputamos os traços para zero e validamos que a soma dos **396 municípios** bate exatamente **112.443 notificações** com 100% de consistência aritmética.
   > Na EDA (Seção 4), vimos que **Londrina é o 2º maior polo do Paraná** com **6.762 casos** e **59,38% de reincidência**, enquanto a média estadual é de 53,5%."

---

### Bloco 3B — Samuel Augusto (Meta: 1 min 45s)
* **Cartão na tela (2s):** `Fase 3 — Samuel Augusto`
* **Abas pré-abertas no VS Code:**
  1. `app/src/components/BotaoSaidaRapida.js`
  2. `app/src/screens/diario/ListaOcorrenciasScreen.js`
  3. `api/server.js` (linhas 55–95, 243–295 e 410–460)
  4. `data-science/notebook.ipynb` (Seções 5 a 7)

#### Passo a passo + Fala pronta (Samuel):
1. **[0:00 – 0:55] Código Mobile + API REST + Painel Web:**
   > "Meu nome é **Samuel Augusto**. Vou apresentar o código da Saída Rápida, do Diário de Ocorrências e do Painel da Delegacia.
   > Em `BotaoSaidaRapida.js`, o botão está injetado no `headerRight` de todas as stacks e abas e chama `aoSair` diretamente — sem `Alert` de confirmação, garantindo escape imediato para a fachada.
   > Em `ListaOcorrenciasScreen.js`, usamos `Promise.all` para buscar `/ocorrencias` e `/pontos` juntos, exibindo o vínculo com o ponto de apoio e o selo de risco calculado pela API.
   > No `api/server.js` (linha 243), a rota `/ocorrencias` valida duas chaves estrangeiras reais: `usuariaId` e `pontoApoioId` opcional contra `pontos.json`. Antes de salvar, ela chama `estimarRiscoAcademico` (linha 55), que lê `modelo_risco.json` e combina os fatores com a probabilidade regional. Por fim, na linha 456, servimos o Painel Web da Delegacia (`/delegacia`), que faz polling a cada 5 segundos no endpoint `/painel`."
2. **[0:55 – 1:45] Notebook de Data Science (Modelagem 5-Fold, Avaliação e Integração):**
   * *(troca para `data-science/notebook.ipynb`, rolando Seções 5 a 7)*
   > "Em Data Science, conduzi a **Modelagem, Avaliação e Integração**. Filtramos os 350 municípios do Paraná com pelo menos 10 notificações e definimos o alvo binário `alto_risco_reincidencia` acima da mediana estadual (53,85%). Para evitar *data leakage*, removemos as colunas de `Sim`/`Não` das preditoras e colocamos `SimpleImputer`, `StandardScaler` e `OneHotEncoder` dentro de um `Pipeline`.
   > Comparamos **Regressão Logística, Árvore de Decisão e Random Forest** usando **Validação Cruzada Estratificada de 5 folds**. O **Random Forest** teve o melhor F1 e Recall na validação cruzada. No conjunto de teste, ajustamos o limiar de 0,50 para **0,45** para priorizar o **Recall** e reduzir falsos negativos, atingindo **Recall de 71,1%**, **F1 de 0,627** e **ROC-AUC de 0,610**, como mostra a Matriz de Confusão e a Curva ROC. Por fim, na Seção 7, exportamos `api/dados/modelo_risco.json` diretamente para a API do aplicativo."

---

## 5. FASE 4 — Verificação Individual Ao Vivo (1 min 30s por aluno — SEM CORTES!)

⚠️ **REGRAS CRÍTICAS DESTA FASE:**
* **NÃO abra `https://apiwp.smartcortex.ai:8888/` antes de gravar!**
* **UMA ÚNICA TOMADA SEM NENHUM CORTE** do cartão inicial até o fim da resposta!
* **Se não souber a 1ª pergunta:** clique para gerar a 2ª (e última) pergunta **sem cortar a gravação**!
* Mantenha o VS Code já aberto atrás do navegador para alternar com `Alt + Tab` em 1 segundo.

### Roteiro exato (igual para Mateus e para Samuel):
1. **Mostre o cartão na tela:** `Fase 4 — Mateus Zichack` *(ou `Fase 4 — Samuel Augusto`)*
2. **Diga em voz alta:** *"Meu nome é [Nome Completo]. Vou abrir agora o site da verificação individual."*
3. **Abra o navegador e digite/acesse:** `https://apiwp.smartcortex.ai:8888/` *(com a tela toda visível)*
4. **Digite seu RGM** no campo indicado falando em voz alta: *"Estou digitando meu RGM, que é [seu RGM]."*
5. **Clique em Gerar Pergunta:** *"Agora vou clicar em gerar pergunta."*
6. **Leia a pergunta inteira em voz alta** deixando o texto bem legível na gravação: *"A pergunta sorteada foi: '[leia tudo]'."*
7. **Dê `Alt + Tab` para o VS Code / Notebook e responda objetivamente mostrando a linha de código ou célula correspondente** (tente fechar tudo dentro de **1 min 15s – 1 min 25s**!).

---

## 6. Cola Rápida de Estudo para a Fase 4 (Mapa do Código — Ache em 3 Segundos!)

Estudem esta tabela antes de gravar para responder qualquer pergunta sorteada com segurança e mostrando o código na hora:

| Se a pergunta cair sobre... | Onde abrir no VS Code | Resposta curta e direta |
|---|---|---|
| **Diferença entre GET, POST, PUT e DELETE / status HTTP** | `api/server.js` (L103–175) e `app/src/servicos/api.js` (L16–65) | `GET` lista/busca (`200` ou `404`); `POST` cria registro novo enviando JSON no `body` (`201` ou `400`); `PUT /:id` atualiza parcialmente um registro existente (`200`, `400` ou `404`); `DELETE /:id` remove pelo ID sem body (`200` ou `404`). |
| **Como validam chaves estrangeiras / relacionamento na API** | `api/server.js` (L177 `validarUsuariaExiste` e L243 `/ocorrencias`) | Antes de gravar no POST ou PUT, a função `relacionar` lê a coleção pai (`usuarias.json` ou `pontos.json`), verifica com `.some()` se o ID existe; se não existir, barra a requisição com HTTP **400** e lista de erros. |
| **Como o app recarrega os dados ao voltar de um formulário** | `ListaContatosScreen.js` ou `ListaOcorrenciasScreen.js` | Usamos `useFocusEffect` do `@react-navigation/native` chamando a função `async` que faz `fetch` na API, com estados `carregando` (`ActivityIndicator`) e `erro` (botão "Tentar novamente"). |
| **Como funciona o Disfarce (entrada) e a Saída Rápida (Quick Exit)** | `App.js`, `RaizNavegacao.js`, `TelaDisfarce.js` (L58) e `BotaoSaidaRapida.js` | O estado `emApoio` em `App.js` alterna entre `TelaDisfarce` e `TabsPrincipais`. Na entrada, digitar `1800` (ou segurar o título) chama `aoDesbloquear()`. Na saída rápida, `BotaoSaidaRapida` no `headerRight` de todas as telas chama `aoSairRapido()` em **1 toque, sem confirmação**. |
| **Como funciona o Painel Web em Tempo Real (polling)** | `api/server.js` (L410 `/painel` e L456 `/delegacia`) e `api/public/delegacia.html` | A página `delegacia.html` usa `setInterval(atualizarPainel, 5000)` para consultar `GET /painel` a cada 5s e atualizar KPIs, alertas SOS e contatos automaticamente; os botões do operador chamam `PUT /alertas/:id`. |
| **Base pública real, LGPD e 5 dimensões de qualidade** | `data-science/notebook.ipynb` (Seções 1–3) | Base real do Tabnet SINAN/DataSUS Paraná (`112.443` casos em `396` cidades, agregada por município para garantir LGPD sem nomes/CPFs). Tratamos Completude (`"-"` $\rightarrow$ `0`), Validade (cabeçalho/rodapé Tabnet), Consistência (regex IBGE + soma), Unicidade (remoção da linha `"Total"`) e Acurácia (soma bate exata). |
| **O que é data leakage e como evitamos no Pipeline** | `data-science/notebook.ipynb` (Seção 5) | *Data leakage* ocorre quando informação do alvo ou do conjunto de teste vaza pro treino. Evitamos de duas formas: (1) removemos `Sim`, `Não` e `taxa_reincidencia_pct` das preditoras `X`; (2) colocamos `SimpleImputer`, `StandardScaler` e `OneHotEncoder` dentro de um `sklearn.pipeline.Pipeline`, ajustado só no treino em cada fold. |
| **Validação Cruzada (StratifiedKFold 5-fold)** | `data-science/notebook.ipynb` (Seção 5) | Divide o treino em 5 partes mantendo a proporção da classe alvo (*estratificada*). Cada modelo é treinado 5 vezes em 4 partes e validado na 5ª, gerando média e desvio padrão para não depender de "sorte" de uma única divisão. |
| **Por que priorizamos Recall e ajustamos limiar para 0,45** | `data-science/notebook.ipynb` (Seção 6 — Matriz de Confusão + Curva ROC) | Em violência contra a mulher, um **Falso Negativo** (não sinalizar uma situação/região de alto risco) é muito mais grave que um Falso Positivo. Usando `class_weight="balanced"` e baixando o limiar de `0,50` para `0,45`, o **Recall** subiu para **71,1%** (F1 `0,627`, ROC-AUC `0,610`). |
| **Como o modelo de DS se integra no aplicativo** | `notebook.ipynb` (Seção 7) $\rightarrow$ `api/dados/modelo_risco.json` $\rightarrow$ `api/server.js` (L55) $\rightarrow$ `AutoavaliacaoScreen.js` | O notebook exporta `modelo_risco.json` com métricas e probabilidades regionais da RM de Londrina. A API lê esse arquivo em `estimarRiscoAcademico`, combina 70% dos fatores individuais (CNJ) + 30% da probabilidade regional do modelo e devolve ao app com o aviso acadêmico obrigatório. |

---

## 7. Checklist Final Antes de Enviar

- [ ] **Fase 1:** gravada em $\le$ 1 min 30s (com os 4 itens na ordem).
- [ ] **Fase 2:** Mateus ($\le$ 2 min) e Samuel ($\le$ 2 min), cada um com cartão + nome completo dito em voz alta + CRUD ao vivo na API real + indicador DS no app.
- [ ] **Fase 3:** Mateus ($\le$ 2 min) e Samuel ($\le$ 2 min), cada um com cartão + nome completo dito em voz alta + código Mobile/API + etapa do notebook DS e métricas.
- [ ] **Fase 4:** Mateus ($\le$ 1 min 30s) e Samuel ($\le$ 1 min 30s), cada um em **uma única tomada sem cortes** (cartão + nome completo + abrir `https://apiwp.smartcortex.ai:8888/` + digitar RGM + gerar pergunta + ler em voz alta + responder no código/notebook).
- [ ] **Vídeo único** juntado na ordem exata (`Fase 1 → F2 Mateus → F2 Samuel → F3 Mateus → F3 Samuel → F4 Mateus → F4 Samuel`), total $\le$ 12 min 30s.
- [ ] **Upload no YouTube** como **Público** ou **Não listado** (testar abrindo em aba anônima sem login!).
- [ ] **Envio no Blackboard:** tanto **Mateus** quanto **Samuel** colam o link do vídeo no YouTube na tarefa (conforme exigência de envio individual!).
