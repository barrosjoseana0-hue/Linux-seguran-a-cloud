# Superfície de Ataque

Foi identificado um serviço web ativo na porta 80/TCP, responsável pela disponibilização da página web.

Além disso, o sistema possui serviços internos que não estão expostos externamente:

- DNS local (127.0.0.53:53)
- Base de dados MySQL/MariaDB (127.0.0.1:3306)
- Serviço de impressão (127.0.0.1:631)
- Serviços de descoberta de rede (mDNS/Avahi)

## Riscos identificados

1. Exposição do serviço web na porta 80.
2. Possíveis vulnerabilidades em software desatualizado.
3. Serviços internos devem permanecer restritos ao localhost.
