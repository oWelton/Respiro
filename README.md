# Respiro — Ativação Comportamental Adaptativa e Micrometas

> Single Page Application (SPA) progressiva (PWA), 100% offline-first e ultra-acessível, desenhada com princípios de neuroergonomia, psicologia comportamental e baixa sobrecarga sensorial para pessoas enfrentando depressão profunda e exaustão cognitiva extrema.

---

## 🌟 Funcionalidades Avançadas de Ergonomia Sensorial e Clínica

### 1. Refinamento de UX & Ergonomia Sensorial
- **Modo "Névoa Extrema" (Ultra-Low Stimulus):**
  - Alternador no topo que remove completamente bordas, badges de categoria, barra de atrito, descrições secundárias e rodapés.
  - A tela exibe exclusivamente uma linha de texto com a microtarefa e dois botões elementares: `[ Concluir com calma ]` e `[ Hoje está muito difícil ]`. Ideal para momentos de sobrecarga sensorial ou crises agudas.
- **Micro-feedback Háptico Suave:**
  - Utiliza `navigator.vibrate([20, 35, 20])` para emitir uma pulsação amortecida no celular ao concluir ações ou avançar na trilha de pedras. Proporciona alívio físico tátil sem depender de áudio.
- **Soundscape Ambience Nativo (Web Audio API):**
  - 3 paisagens sonoras sintetizadas matematicamente no navegador (zero arquivos externos de áudio):
    1. **Ruído Marrom Profundo:** Abafamento de ruídos externos e alívio do sistema nervoso simpático.
    2. **Chuva Mansa:** Frequências em banda passa-baixa simulando gotas suaves na vegetação.
    3. **Brisa Noturna:** Modulação lenta (LFO) criando uma suave sensação de vento arejado.
- **Temas Circadianos Reativos:**
  - Ajuste de temperatura de cor baseado no relógio local:
    - **Dia (06h às 18h):** Carvão `#121417` com verde sálvia botânico `#68a090`.
    - **Noite (18h às 06h):** Tons terrosos âmbar (`#141210` e `#1c1916`) para preservar a melatonina e não agredir os olhos no escuro. Pode ser alternado manualmente a qualquer momento.

### 2. Mecânicas Clínicas e Comportamentais
- **Modo Espectador ("Validação por Presença"):**
  - Botão acolhedor: *"Não consigo fazer nada hoje, só abri o app"*.
  - Resposta do sistema: *"Abrir o app já é um movimento real. Sua presença aqui é suficiente por hoje."*
  - Concede um broto no terrário e avança uma pedra na trilha sem qualquer exigência motora.
- **Decaimento de Inércia (Temporizador de 30 Segundos):**
  - Botão *"Tentar por 30 segundos"*. Uma barra suave preenche o tempo sem números regressivos estressantes.
  - Ao expirar: *"Seu tempo acabou. Quer parar por aqui sem culpa ou deseja mais 30 segundos?"*. O usuário pode parar com mérito total de vitória.
- **Gaveta de Âncoras Positivas ("O que costuma te resgatar"):**
  - Tarefas que geraram alto alívio de humor ($\Delta \ge +2$) são salvas silenciosamente na gaveta de âncoras.
  - Em dias de bateria nível 1 (Repouso Profundo), o sistema prioriza automaticamente sugerir essas âncoras conhecidas.
- **Cronômetro Silencioso de Descompressão (Pacer):**
  - Guia de respiração fluida (Inspire... Retenha... Expire... Descanse) com círculo expansor suave para desacelerar o ritmo cardíaco.

### 3. Terrário Vivo, Fases do Dia & Coleção Silenciosa
- **Sincronização Circadiana Real (Fases do Dia):**
  - **Dia (06h às 17h):** Fundo florestal suave com feixes de luz solar filtrada (*god rays* dourados/esmeralda) e tons de sálvia botânico.
  - **Crepúsculo (17h às 19h30):** Pôr do sol acolhedor com tons quentes de âmbar e terra, propiciando desaceleração natural.
  - **Noite (19h30 às 06h):** Penumbra profunda com luar azul-petróleo/prateado vindo do topo e vaga-lumes bioluminescentes flutuando com pulsação suave em senoide.
- **Interação Contemplativa sem Mecânicas de Jogo:**
  - **Movimento da Folhagem (*Sway*):** Mover o mouse ou deslizar o dedo produz uma leve brisa física e paralaxe que inclina suavemente as folhas, brotos e cogumelos.
  - **Ondulações de Luz (*Light Ripples*):** O cursor deposita auréolas de luz translúcida que se expandem e desvanecem pacificamente.
  - **Gotas de Orvalho (*Dewdrops*):** Clicar ou tocar em áreas livres do terrário faz cair uma gota de orvalho com gravidade suave, criando ondulações circulares concêntricas no solo e microvibração háptica.
- **Coleção Silenciosa Permanente:**
  - Elementos tranquilos que vão surgindo com os marcos (Ramo de Alfazema, Pedra Lisa de Rio, Cogumelo Luminescente, Folha de Ginkgo, Broto de Sálvia e Cristal de Orvalho).
  - Tocar em qualquer elemento no canvas ou nos botões da coleção revela uma frase curta de validação arquivada (ex.: *"A água molda a rocha com paciência, não com força. Seu ritmo é sábio."*).

### 4. Card Principal & Fluxo de Micrometas Acolhedor
- **Ajuste Fino do Botão "Trocar":**
  - Busca estritamente outra tarefa do **exato mesmo nível de atrito** (sem exigir menos nem mais energia). Ideal para quando o contexto impede aquela ação específica (ex.: chuva lá fora ou horário impróprio).
- **Dopamina Suave (Feedback de 2 Segundos):**
  - Ao concluir uma ação, o card realiza uma transição suave e exibe um micro-elogio sutil durante 2 segundos (*"Feito. Respeite sua pausa."*, *"Um micromovimento a mais no mundo."*, *"Isso foi o bastante por agora."*).
- **Opção de Fechar e Descansar ("Descansar por hoje"):**
  - Após o micro-elogio, o usuário tem a opção de continuar para o próximo passo ou clicar em **"Descansar por hoje (Fechar app)"**, ativando uma tela de repouso pleno e autorização psicológica para descansar sem culpa.
- **Ajuste Automático de Bateria por Feedback Negativo:**
  - Se o usuário clicar duas vezes consecutivas em *"Hoje está muito difícil"*, o app sugere silenciosamente mudar para o **Modo Preservação Máxima** (Atrito 1), poupando a pessoa de ter que ir ao menu reconfigurar manualmente.

### 5. Central de Apoio (A Âncora) & CVV 188
- **Atalhos Imediatos de Apoio:**
  - Ligação direta para o **CVV (188)** (`tel:188`) e atalho direto para o **Chat CVV Online**.
- **Técnica 5-4-3-2-1 Interativa e Guiada:**
  - Passo a passo visual e sensorial conduzido sentido por sentido (5 coisas para ver, 4 para tocar, 3 para ouvir, 2 para cheirar e 1 para sentir a ancoragem física no chão).

### 6. Guia de Respiração Descompressiva (Tela Cheia Nativa)
- **Zero Pop-up ou Distração:**
  - Experiência em tela cheia absoluta (`fixed inset-0` em fundo `#121417`), eliminando qualquer distração visual.
- **Círculo Amplo e Central:**
  - Ocupa 65vw a 70vw no celular (até 320px no desktop) com halo de luminosidade orgânico.
  - Curva de animação com `cubic-bezier(0.4, 0, 0.2, 1)` com pausas naturais no ápice (*plenitude*) e no esvaziamento (*repouso*).
- **Saída Simples e Universal:**
  - Um toque em qualquer ponto da tela fecha a respiração imediatamente, dispensando mira com mouse ou polegar. Também suporta botão X translúcido e tecla ESC.

---

## 🚀 Como Executar e Instalar

1. Abra o arquivo [`index.html`](file:///C:/Users/welton.moreira/.gemini/antigravity/scratch/respiro/index.html) em qualquer navegador moderno.
2. Para instalar no celular ou desktop, utilize a opção do navegador "Instalar aplicativo" ou clique no botão de instalação que surge na gaveta de opções.
3. Não requer conexão com a internet, servidor ou banco de dados externo.
