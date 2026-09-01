### Siandro Sena

Engenheiro de Produção (com base em Engenharia de Materiais) migrando para automação de processos, dados e IA. MBA em Inteligência Artificial.

Minha base é mapear processo antes de tocar em ferramenta — é o que Engenharia de Produção ensina. Os projetos abaixo são todos do mesmo domínio (frota/transporte) de propósito, pra mostrar profundidade — mas a habilidade por trás é genérica: entender qualquer processo real de perto o suficiente pra saber o que vale automatizar, com o quê, e o que NÃO vale a pena virar sistema.

**Stack:** n8n · Python · Google Apps Script · Google Workspace (Sheets/Drive) · agentes de IA (LLMs de visão e texto) · visão computacional (YOLOv8, ByteTrack, OpenCV)

---

Nem todo processo automatizado devia virar app: boa parte do que mantenho em produção roda direto em Google Sheets + Apps Script — dashboard multi-fonte, validação de dado na entrada, alertas automáticos — porque é a ferramenta que quem usa já sabe abrir, sem precisar de deploy nem de mim no meio.

#### Projetos

**🚌 [contador-onibus](https://github.com/siandrosena/contador-onibus)**
Contagem de passageiros por vídeo com YOLOv8 + ByteTrack — detecção, rastreamento por ID e deduplicação de cruzamento de linha. Substitui contagem manual numa operação real de transporte.

**🛞 [fleet-tire-lifecycle-tracker](https://github.com/siandrosena/fleet-tire-lifecycle-tracker)**
Motor de regras de manutenção preventiva de pneus: classificação de severidade por 3 métricas e detecção automática de rodízio, transferência entre veículos e pneu remontado invertido, comparando cada leitura nova contra o estado de toda a frota. 31 testes.

**📸 [fleet-photo-intake-pipeline](https://github.com/siandrosena/fleet-photo-intake-pipeline)**
Pipeline n8n + IA de visão pra ler fichas de manutenção manuscritas — com uma camada em Python que valida a extração antes de qualquer gravação, sinalizando os padrões de erro de OCR já vividos em produção em vez de confiar cego na IA.

**🚦 [fleet-maintenance-priority-engine](https://github.com/siandrosena/fleet-maintenance-priority-engine)**
Diagnóstico automático de roda (alinhar vs. calibrar, a partir de 4 leituras de sulco) e motor de score que cruza várias categorias de inspeção pra dizer qual veículo da frota olhar primeiro. Generalizado de um sistema real em produção (Sheets + Apps Script), com seção honesta de limitações conhecidas.

**🔧 [n8n-nodes-wheel-diagnosis](https://github.com/siandrosena/n8n-nodes-wheel-diagnosis)**
A mesma regra de diagnóstico de roda, embrulhada como community node nativo do n8n (TypeScript, tipado contra a API real do n8n) — pra rodar dentro do editor visual sem precisar de um passo de código externo.

**⏱️ [garage-dwell-time-tracker](https://github.com/siandrosena/garage-dwell-time-tracker)**
Estudo de tempos e movimentos automatizado — mede quanto tempo cada pessoa fica perto de um veículo em manutenção, usando YOLOv8+ByteTrack, sem prancheta nem cronômetro manual.

---

Também levo isso pra prática de consultoria: [diagnóstico de priorização de frota](https://siandrosena.github.io/diagnostico-frota/) aplica essa mesma lógica como serviço, direto pra quem gerencia frota hoje.

---

Aberto a oportunidade remota em automação de processos, dados e IA.

[LinkedIn](https://www.linkedin.com/in/siandro-sena-847712314)
