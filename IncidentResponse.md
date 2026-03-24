[Voltar ao README](README.md)

Com base na análise do alerta, foi identificado um padrão compatível com password spraying.

1. Classificação
- Tipo: Tentativa de acesso não autorizado
- Severidade: Média
- Status: Verdadeiro positivo (atividade maliciosa)
  
2. Análise
- Múltiplas tentativas de autenticação falhadas
- Uso de contas desativadas como alvo
- Origem comum (mesmo IP)
- Ocorrência repetida em curto intervalo de tempo

O comportamento indica tentativa automatizada de identificação de credenciais.

3. Ações Recomendadas
- Forçar redefinição de senha das contas afetadas
- Desabilitar temporariamente contas comprometidas pelo Active Directory
- Revisar histórico de login dos usuários impactados
- Monitorar novas tentativas provenientes do mesmo IP
  
4. Contenção
- Sugerido bloqueio do IP malicioso em nível de identidade (Conditional Access) ou endpoint
