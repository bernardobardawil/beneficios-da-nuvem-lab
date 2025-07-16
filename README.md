# beneficios-da-nuvem-lab
Estudo prático da criação de máquinas virtuais no Microsoft Azure via portal, com conexão RDP e instalação do IIS. Inclui os conceitos essenciais do Módulo 1 da certificação AZ-900, como alta disponibilidade, escalabilidade, elasticidade, confiabilidade, segurança, governança e gerenciabilidade na nuvem.

 Conceitos de Nuvem (AZ-900 – Módulo 1)
Alta Disponibilidade

A nuvem garante acesso contínuo aos serviços, mesmo diante de falhas. O Azure oferece SLAs que garantem isso.

Escalabilidade

Aprendi que posso aumentar ou reduzir os recursos conforme a demanda (escalar verticalmente ou horizontalmente), pagando apenas pelo uso real.

Elasticidade

A capacidade de se adaptar automaticamente a variações repentinas de demanda torna os sistemas mais eficientes.

Confiabilidade

A nuvem é descentralizada: se uma região falhar, outras mantêm os serviços funcionando.

Previsibilidade

A nuvem permite prever custos e desempenho com mais segurança, com ajuda de boas práticas como o Azure Well-Architected Framework.

Segurança

A nuvem oferece ferramentas robustas de segurança, mas o cliente também é responsável por configurá-las corretamente, dependendo do modelo de serviço (IaaS, PaaS, SaaS).

Governança

Através de políticas e auditorias automatizadas, é possível manter conformidade e controle sobre os recursos na nuvem.

Gerenciabilidade

Os recursos da nuvem podem ser gerenciados por portal web, CLI, PowerShell ou APIs, com automações que reduzem o trabalho manual.

Criação de Máquina Virtual Windows no Azure

1. Acesso ao Portal

Aprendi a entrar no Azure Portal com minha conta Microsoft para iniciar a criação e o gerenciamento de recursos na nuvem.

2. Criação da VM

Criei uma máquina virtual Windows Server 2022, definindo nome, usuário e senha, e permitindo o acesso remoto via RDP (porta 3389) e HTTP (porta 80).

3. Conexão via RDP

Usei o arquivo .rdp gerado pelo portal para me conectar à VM com segurança usando credenciais administrativas.

4. Instalação de IIS

Instalei o servidor web IIS via PowerShell com o comando:

powershell
Copiar
Editar
Install-WindowsFeature -name Web-Server -IncludeManagementTools
Isso tornou minha VM apta a servir páginas web.

5. Verificação

Acessei o IP público da VM pelo navegador e visualizei a página de boas-vindas do IIS.

6. Limpeza de Recursos

Deletei o resource group para evitar custos adicionais, encerrando corretamente o ciclo do recurso.
