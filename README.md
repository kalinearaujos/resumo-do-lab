# resumo-do-lab
Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab na DIO

Durante o Lab foi possível aprender conceitos importantes sobre computação em nuvem bem como os conceitos básico do GIT e Github, sem contar com a importância de criar um portfolio de excelência.
As aulas foram simples, porém com as explicações bem didaticas e com conteúdo enriquecedor, os professores sem mostrando domínio do conteúdo.

conceitos de nuvem

tipos de serviços de nuvem

IaaS, Paas e SaaS

IaaS (Infraestrutura como serviço)

Pode ser criado uma infraestrutura de TI de pagamento conforme o uso.

PaaS (Plataforma como serviço)

fornece um ambiente para criação, o teste e a implantação de aplicativos de software, sem focar no gerenciamento
da infraestrutura subjacente.

SaaS (software como serviço)

Usuários se conectam e usam aplicativos com base em nuvem pela internet: por exemplo, Microsoft office 365, email e 
calendários.

Se atentar com relação aos Modelos de responsabilidade compartilhada.

-------> Arquitetura e serviços do Azure <--------
 Componentes: regiões e zonas de disponibilidade e assinaturas e grupos de recursos

principais componentes arquitetônicos: 

Regiões: influência na questão de valores. (conta com mais de 60 regiões globais, representando 140 países). Compostas por um ou mais datacenters, fornece flexibilidade e escala para reduzir latência.
preservam a residência dos dados om uma oferta abrangente de conformidade.

Zona de disponibilidade: estão dentro da região

Pares de regiões: no mínimo 300 milhas de separação entre pares e regiões, replicação automática para alguns serviços e recuperação de região priorizada em caso de interrupção.

Regiões soberanas do Azure: atende as necessidades de segurança e conformidade das agências federais, governos estaduais e locais dos EUS e seus provedores de soluções.

Duas regiões soberanas: EUA e China

Recursos do Azure: são componentes como armazenamento, máquinas virtuais e redes que estão disponíveis para criar soluções de nuvem.

Grupo de recursos - não se limita a regiões: é um contêiner que você usa para gerenciar e agregar recursos em uma única unidade.
os recursos podem ser movidos para diferentes grupos e os aplicativos podem utilizar vários grupos também.

Assinaturas do Azure: Uma assinatura do Azure fornece a você acesso autenticado e autorizado às contas do Azure.
limite de cobranças, limite do controle de acesso.

Grupos de gerenciamento - organização, também esta relacionado a segurança. Pode ser criado manualmente.
Podem incluir várias assinaturas do Azure.
As assinaturas herdam as condições aplicadas ao grupo de gerenciamento

----> Arquitetura e serviços do Azure

Computação e Rede (tipos de computação, incluindo instâncias de contêiner, máquinas virtuais e funções. Recursos exigidos para máquinas virtuais, pontos de extremidade públicos e privados. Opções de máquinas virtuais, conjuntos de dimensionamento de máquinas virtuais, conjuntos de disponibilidade de máquinas e a áreas de trabalho do azure).

*serviços de computação: é um serviço sob demanda que fornece recursos de computação, como discos, processadores, memória, rede e sistemas operacionais.

máquinas virtuais: 
- São emulações de software de computadores físicos. 
- Inclui processador virtual, memória, armazenamento e rede. 
- Oferta IaaS que oferece personalização e controle total.

conjuntos de disponibilidade de VM:

área de trabalho virtual do Azure: é uma virtualização de área de trabalho e aplicativo executada em nuvem.
cria um ambiente completo de virtualização, reduz risco de recurso, implantações reais de várias sessões.

Serviços de contêineres do Azure: fornecem um ambiente leve e virtualizado que n~~ao exige o gerenciamento do sistema operacional e pode responder a alterações sob demanda.

Instâncias de contêiner do Azure: uma oferta de Paas que executa um contêiner ou pod de contêineres no Azure.

Aplicativos de contêiner do Azure: uma oferta de PaaS, como instâncias de contêineres, que pode balancear a carga e escalar.

Serviço de kubernetes o Azure: um serviço de orquestração para contêineres com arquiteturas distribuídas e grandes volumes de contêineres.

Azure functions: uma oferta de PaaS que dá suporta a operações de computação sem servidor.
O código baseado em eventos é executado quando chamado, sem exigir uma infraestrutura de servidor durante períodos inativos.

Comparar opções de computação do Azure:
*Máquinas virtuais: 
-servidor baseado em nuvem que dá suporte a ambientes Windows e Linux.
-útil para migrações de lift-and-shift (levar como estar) para a nuvem.
-pacote do sistema operacional completo, incluindo o sistema operacional do host.

*Área de trabalho virtual:
-fornece uma experiência de área de trabalho do Windows baseado em nuvem.
-Aplicativos dedicados para conexão e uso ou acessíveis de qualquer navegador moderno.
-O logon de vários clientes permite que vários usuários façam logon no mesmo computador ao mesmo tempo

*Contêineres
-Ambiente leve e em miniatura adequado para execução de microsserviços.
Projetado para escalabilidade e resiliência por meio da orquestração.(AKS)

Serviços de aplicativo do Azure: consistem em uma plataforma totalmente gerenciada para criar, implantar e dimensionar aplicativos web e APIs rapidamente
Trabalha com .NET, .NET Core, Node.js, JAVA, Python ou PHP.
Oferta de PaaS com requisitos de nível corporativo de desempenho, segurança e conformidade.

Serviços de rede do Azure
A rede virtual do Azure (VNet) permite que os recursos do Azure se comuniquem uns com os outros, com a internet e com as redes locais.
Pontos de extremidade públicos, acessíveis de qualquer lugar na internet.
Pontos de extremidades privados, acessíveis somente dentro da sua rede.

As sub-redes virtuais segmentam sua rede para atender as suas necessidades.
O emparelhamento de rede conecta suas redes privadas diretamente.

Serviços de rede do Azure - Gateway de VPN: O gateway de VPN é usado para enviar tráfego criptografado entre uma rede virtual do Azure e uma no local pela internet pública.

Serviços de rede do Azure - ExpressRoute: estende as redes locais para o Azure por meio de uma conexão privada facilitada por um provedor de conectividade.

DNS do Azure:
-Confiabilidade e desempenho aproveitando uma rede global de servidores de nome DNS usando a rede Anycast.
-A segurança do DNS do Azure baseia-se no gerenciados de recursos do Azure, habilitando o controle de acesso baseado em função e o monitoramento e o registro em log.
-Facilidade de uso para gerencias seus recursos externos e do Azure com um único serviço de DNS.
-Redes virtuais personalizáveis permitem que você use nomes de domínio privados e totalmente personalizados em suas redes virtuais privadas.
-Os registros de alias dão suporte a conjuntos de registros de alias para apontar diretamente para um recurso do Azure.

 ----> Armazenamento do Azure <----

Armazenamento: Domínio de objeto
Contas de armazenamento
-Deve ter um nome globalmente exclusivo (3 a 24 caracteres).
-Fornecer acesso a internet em todo mundo.
-Determinar os serviços de armazenamento e as opções de redundância.(LRS- redundância local, ZRS - redundância de zona, GRS - redundância geográfica, GZRS - redundância de zona geográfica).

Blob do Azure: otimizado para o armazenamento de quantidades massivas de dados não estruturados como texto ou dados binários.
Disco do Azure: fornece discos para máquinas virtuais, aplicativos e outros serviços acessarem e utilizarem.
Fila do Azure: serviço de armazenamento de mensagens que fornece armazenamento e recuperação para grandes quantidades de mensagens, cada uma com até 64 KB.
Arquivo do Azure: Configura um compartilhamento de arquivos de rede altamente disponível que pode ser utilizado usando o protocolo de mensagens do servidor.
tabelas do Azure: fornece uma opção de chave/atributo para armazenamento de dados estruturados não relacionais com um design sem esquema.

Pontos de extremidade públicos do serviço de armazenamento: armazenamento de blobs, data lake storage Gen2, arquivos do Azure, armazenamento de fila e armazenamento de tabelas.
Camadas de acesso de armazenamento do Azure: 
-frequente (armazenamento de dados acessados com frequência),
-esporádico (para armazenamento de dados acessados com pouca frequência e armazenados por pelo menos 30 dias), 
-frio (para armazenamento de dados acessados com pouca e armazenados por pelo menos 90 dias), 
-arquivo morto (para armazenamento de dados acessados raramente e armazenados por pelo menos 180 dias com requisitos de latência flexíveis).

-- Migrações para o Azure: Plataforma de migração unificada, intervalo de ferramentas integradas e autônomas, avaliação e migração.

-- Azure data box: armazena até 80 terabytes de dados, move backups de recuperação de desastre para o Azure e protege os dados em uma caixa robusta durante o transito, migre dados do Azure para conformidade ou necessidades regulatórios, migre dados para o Azure de locais remotos com conectividade ou sem conectividade.

AzCopy: utilitário de linha de comando, copiar blobs ou arquivos para sua conta de armazenamento, sincronização em uma direção.

Gerenciados de armazenamento do Azure: Interface gráfica do usuário(de modo semelhante ao Windows Explorer). Compatível com o Windows, MacOS e Linux.

Sincronização de arquivos do Azure: Sincroniza os arquivos do Azure e locais de forma bidirecional. A camada de nuvem mantém os arquivos acessados com frequência no local, enquanto não libera espaço.


