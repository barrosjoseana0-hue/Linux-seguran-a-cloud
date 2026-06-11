# Hardening Inicial

O sistema encontra-se com um serviço web ativo na porta 80/TCP. Foram identificadas algumas medidas iniciais de segurança que podem ser aplicadas para reduzir riscos.

## Medidas aplicáveis imediatamente

- Atualizar o sistema operativo e pacotes instalados:
  sudo apt update && sudo apt upgrade -y

- Manter apenas serviços necessários ativos (ex: Apache e desativar serviços não usados)

- Garantir que apenas a porta 80 está exposta externamente

- Verificar e corrigir permissões de ficheiros do site web

- Remover ou desativar serviços desnecessários (ex: impressão se não for usada)

## Medidas futuras (mais avançadas)

- Configurar HTTPS (porta 443) com certificado SSL
- Implementar firewall mais restritivo (UFW avançado)
- Monitorização de logs do sistema (/var/log)
- Proteção contra ataques de força bruta
- Utilização de ferramentas de deteção de intrusão (IDS)
