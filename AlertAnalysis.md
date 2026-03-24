A imagem demonstra um alerta identificado no Microsoft Defender relacionado a tentativas suspeitas de autenticação, caracterizadas por múltiplos acessos a contas desativadas a partir de um mesmo endereço IP. Esse comportamento é compatível com técnicas de ataque como password spraying, indicando possível tentativa de intrusão.

No painel à direita, é possível visualizar o menu “Manage alert”, utilizado para gerenciamento do alerta.

![labSIEM5](https://github.com/user-attachments/assets/0babe376-3970-47ee-b5bc-9f77d2fe1c8c)

Na aba Advanced Hunting, há mais informações sobre o alerta. Diferente da visualização padrão de alertas, essa aba possibilita investigar padrões, relacionar eventos e identificar comportamentos suspeitos com maior precisão.

Na imagem, foi utilizada uma consulta simples (SecurityAlert) para retornar eventos relacionados ao alerta previamente analisado, incluindo tentativas de login suspeitas a partir de um mesmo endereço IP. Os resultados exibem informações relevantes como:

Data e hora do evento (TimeGenerated)
Nome do alerta (AlertName)
Nível de severidade (AlertSeverity)
Descrição da detecção
Origem do provedor (Microsoft)

Esse tipo de análise permite validar o alerta inicial e expandir a investigação, identificando recorrência, múltiplos alvos e possíveis indicadores de ataque, como padrões compatíveis com password spraying.

![labSIEM6](https://github.com/user-attachments/assets/2340997f-7ec1-41c0-bd6d-9f1754f66649)
