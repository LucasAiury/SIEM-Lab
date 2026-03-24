[Voltar ao README](README.md)

A imagem demonstra um alerta identificado no Microsoft Defender relacionado a tentativas suspeitas de autenticação, caracterizadas por múltiplos acessos a contas desativadas a partir de um mesmo endereço IP. Esse comportamento é compatível com técnicas como password spraying, indicando possível tentativa de intrusão.

No painel à direita, é possível visualizar o menu “Manage alert”, utilizado para gerenciamento do evento, permitindo classificação, atribuição e acompanhamento da investigação.

![labSIEM5](https://github.com/user-attachments/assets/0babe376-3970-47ee-b5bc-9f77d2fe1c8c)

A aba Advanced Hunting permite aprofundar a investigação por meio de consultas estruturadas, possibilitando correlacionar eventos e identificar padrões com maior precisão.

Foi utilizada uma consulta simples (SecurityAlert) para retornar eventos relacionados, incluindo tentativas de login suspeitas a partir de um mesmo endereço IP. Os resultados apresentam informações como:

- Data e hora do evento (TimeGenerated)
- Nome do alerta (AlertName)
- Nível de severidade (AlertSeverity)
- Descrição da detecção
- Origem do provedor (Microsoft)

Esse tipo de análise permite validar o alerta inicial e expandir a investigação, identificando recorrência, múltiplos alvos e possíveis indicadores de ataque, como padrões compatíveis com password spraying.

![labSIEM6](https://github.com/user-attachments/assets/2340997f-7ec1-41c0-bd6d-9f1754f66649)

A análise detalhada confirma que um único endereço IP foi responsável por múltiplas tentativas de autenticação, reforçando a hipótese de atividade automatizada maliciosa.

![labSIEM7](https://github.com/user-attachments/assets/5fa66325-ad26-4d5f-94f2-faeb75e4c05c)
![labSIEM8](https://github.com/user-attachments/assets/b979e42e-75ed-4422-b4b5-92f3a4647880)
![labSIEM9](https://github.com/user-attachments/assets/e7456ab2-1089-4e74-89b9-f59e697c9f78)
