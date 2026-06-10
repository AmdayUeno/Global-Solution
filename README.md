🌕 Sailor-1 | Sistema de Gestão de Recursos

Protótipo navegável de um sistema web para monitoramento e controle de recursos de uma colônia lunar fictícia — Base Selene, Setor 7.


📋 Sobre o Projeto
O Sailor-1 é uma interface de gestão de recursos desenvolvida como resposta ao desafio da Global Solution FIAP — Indústria Espacial. O sistema simula um painel de controle operacional para uma colônia lunar com 47 habitantes distribuídos em 6 módulos, permitindo monitorar energia, água, oxigênio, estoque alimentar e emitir alertas críticos em tempo real.
Embora o contexto seja espacial, a lógica do sistema reflete problemas reais da Terra: gestão hídrica em cidades, monitoramento ambiental, segurança alimentar e resposta a emergências.

🚀 Funcionalidades
O protótipo conta com 7 telas navegáveis por meio de sidebar lateral:
TelaDescriçãoDashboardVisão geral do sistema com 4 métricas críticas, gráfico de consumo 24h e alertas ativosEnergiaGeração solar vs. consumo, status da bateria e autonomia estimadaÁguaReserva hídrica, taxa de reaproveitamento e consumo por móduloQualidade do ArMonitoramento de O₂, CO₂, pressão atmosférica e umidadeAlimentosEstoque atual, produção agrícola e projeção para 30 dias com 2 cenáriosAlertasCentral de alertas com níveis de prioridade (crítico, atenção, info, resolvido)MódulosStatus detalhado individual dos 6 módulos habitacionais da colônia

🎨 Decisões de Design e UX
Identidade Visual
O sistema adota uma estética de cockpit técnico espacial — escura, precisa e funcional — sem recorrer a clichês genéricos de ficção científica.

Paleta: fundo profundo #06090F com superfícies #0C1220 e #111827. A cor de sistema é ciano #4DD9E8, que representa o estado operacional neutro. Um semáforo consistente — verde (normal), laranja (atenção), vermelho (crítico) — codifica o estado de cada recurso de forma imediata e intuitiva.
Tipografia: Space Grotesk para display e navegação (personalidade técnica, mas humanizada) + JetBrains Mono para todos os valores numéricos e dados de telemetria (precisão e leitura rápida).
Assinatura visual: animações pulse nos indicadores de estado crítico — um detalhe sutil que comunica urgência sem poluir a interface.

Hierarquia de Informação
Cada tela segue a mesma estrutura descendente:

Strip de status — métricas-chave em destaque numérico com barra de nível
Gráficos e painéis — contexto histórico e distribuição por módulo
Alertas e detalhes — informação acionável para tomada de decisão

Essa estrutura permite que um operador identifique o estado crítico do sistema em menos de 3 segundos ao abrir qualquer tela.
Acessibilidade e Responsividade

Todos os elementos <canvas> possuem role="img" e aria-label descritivo para leitores de tela
Interface responsiva: sidebar colapsa em telas menores que 900px; grids adaptam para coluna única
Contraste de texto respeitado em todos os estados de cor
Redução de movimento prevista na estrutura (sem animações de layout que causem desorientação)


🛰️ Conexão com ODS
ODSRelação com o projetoODS 2 — Fome ZeroMódulo de gestão alimentar com projeção de déficit e impacto da produção agrícola interna