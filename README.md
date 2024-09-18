# resumo-do-lab-azure
Resumo simples para o bootcamp Azure Essentials

	Ø Componentes de arquitetura do Azure
		○ Regiões e zonas de disponibilidade
		○ Assinaturas e grupos de recursos
		
	Ø Regiões
		○ Conta com mais de 60 regiões representado em mais de 140 países.
		○ As regiões são compostas de um ou mais datacenters muito próximos
		○ Fornece flexibilidade e escala, reduzindo a latência
		○ As regiões preservam a residência dos dados com uma oferta abrangente e conforme
		○ As zonas de disponibilidade fornecem proteção contra tempo de inatividade devido a falha do datacenter
		○ Separa fisicamente datacenters dentro da região
		○ Cada datacenter é totalmente equipado, com alimentação, resfriamento e redes independentes
		○ Conectadas por meio de redes privadas de fibra óptica.
		○ Pares de regiões
			§ No mínimo 300 milhas de separação entre pares de regiões.
			§ Replicação automática para alguns serviços
			§ Recuperação de região priorizada em caso de interrupção.
			§ As atualizações são distribuídas sequencialmente para minimizar o tempo de inatividade
			§ 
			§ Serviços governamentais dos EUA
				□ Atende às necessidades de segurança e conformidade das agências federais, governos estaduais e locais dos EUA e seus provedores de soluções.
				□ Instância separada do Azure.
				□ Fisicamente isolada de implantações que não sejam do governo dos EUA
				□ Acessível somente para pessoas autorizadas
			§ Regiões soberanas
				□ Azure EUA
				□ Azure China
					® Operada pela 21Vianet
					® Dados permanecem dentro da china para garantir a conformidade
	Ø Recursos do Azure
		○ Maquinas virtuais
		○ Contas de armazenamento
		○ Redes Virtuais
		○ Serviços de Aplicativos
		○ Bancos de dados SQL
		○ Funções
			§ Grupos de Recursos
				□ Conjunto de recursos que podem ser utilizados e organizados conforme a necessidade
				□ É um contêiner que você usa para gerenciar e agregar recursos em uma única unidade.
				□ Podem ser movidos para diferentes grupos de recursos
				□ Os aplicativos podem utilizar vários grupos de recursos
	Ø Assinaturas do Azure
		○ 
		○ Uma assinatura do Azure fornece a você acesso autenticado e autorizado às contas do Azure
		○ Limite de cobrança - gere relatórios de cobrança e faturas separados para cada assinatura
		○ Limite do controle de acesso - gerenciar e controlar o acesso aos recursos que os usuários podem provisionar com assinaturas específicas
		○ 
		○ Grupos de gerenciamento podem incluir várias assinaturas do Azure.
		○ As assinaturas herdam as condições aplicadas ao grupo de gerenciamento.


	Ø Arquitetura e Serviços do Azure
		○ Computação e Rede: domínio de objetivo
			§ Comparar tipos de computação, incluindo instâncias de contêiner, máquinas virtuais e funções.
			§ Descrever os recursos exigidos para as máquinas virtuais
			§ Definir pontos de extremidade públicos e privados.
			§ Descrever as opções de máquina virtual, incluindo VMs, conjuntos de dimensionamento de VMs, conjunto de disponibilidade de máquinas virtuais e a Área de Trabalho Virtual do Azure.
		○ Serviços de computação do Azure
			§ A computação do Azure é um serviço sob demanda que fornece recursos de computação, como discos, processadores, memória, rede e sistemas operacionais.
		○ Maquinas Virtuais do Azure
			§ As máquinas virtuais do Azure (VMs) são emulações de software de computadores físicos.
			§ Inclui processador Virtual, memória, armazenamento e rede.
			§ Oferta de Iaas que oferece personalização e controle total.
		○ Conjuntos de dimensionamento de VMs
			§ Os conjuntos de dimensionamento oferecem um oportunidade de balanceamento de carga para dimensionar os recursos automaticamente.
		○ Conjuntos de disponibilidade de VM
			§ 
		○ Area de trabalho Virtual do Azure
			§ A área de trabalho virtual do Azure é uma virtualização de área de trabalho e aplicativo executada na nuvem.
			§ Crie um ambiente completo de virtualização da área de trabalho sem precisar executar outros servidores de gateway
			§ Reduza o risco de que o recurso seja deixado para trás.
			§ Implantações reais de várias sessões.
		○ Serviços de contêiners do Azure
			§ Os contêineres do Azure fornecem um ambiente leve e virtualizado que não exige o gerenciamento do sistema operacional e pode responder a alterações sob demanda.
			§ Instâncias de contêiner do Azure: uma oferta de PaaS que executa um contêiner ou pod de contêineres no Azure.
			§ Aplicativos de contêiner do Azure: uma oferta de Paas, como instâncias de contêineres, que pode balancear a carga e escalar.
		○ Serviço de Kubernetes do Azure: um serviço de orquestração para contêineres com arquiteturas distribuídas e grandes volumes de contêineres.
		○ Azure Functions: uma oferta PaaS que dá suporte a operações de computação sem servidor
			§ O código baseado em eventos é executado quanto chamado, sem exigir uma infraestrutura de servidor durante períodos inativos.
		○ Comparação de opções de opção do azure
			§ Maquinas Virtuais
				□ Servidor baseado em nuvem que dá suporte a ambientes Windows ou Linux
				□ Útil para migrações de lift-and-shift para a nuvem (levar como está para a nuvem, migração)
				□ Pacote do sistema operacional completo, incluindo o sistema operacional do host.
			§ Área de trabalho Virtual
				□ Fornece uma experiencia de área de trabalho do windows baseada em nuvem
				□ Aplicativos dedicados para conexão e uso ou acessíveis de qualquer navegador moderno
				□ Logon de vários usuários no mesmo computador ao mesmo tempo
			§ Contêineres
				□ Ambiente leve e em miniatura adequado para a execução de microserviços
				□ Projetado para a escalabilidade resiliência por meio da orquestração. 
				□ Os aplicativos e serviços são empacotados em um contêiner que fica na parte superior do sistema operacional do host. Vários contêineres podem ficar em um sistema operacional do host.
		○ Serviços de aplicativo do Azure
			§ Os serviços de aplicativos do azure consistem em uma plataforma totalmente gerenciada para criar, implantar e dimensionar aplicativos Web e APIs rapidamente.
			§ Trabalha com .NET, .NET Core, Node.js, Java, Python ou PHP.
			§ Oferta de PaaS com requisitos de nível corporativo de desempenho, segurança e conformidade.
		○ Serviços de rede do Azure
			§ A Rede Virtual do Azure (Vnet) permite que os recursos do Azure se comuniquem uns com os outros, com a Internet e com as redes locais.
			§ Pontos de extremidade públicos, acessíveis de qualquer lugar na Internet.
			§ Pontos de extremidade privados, acessíveis somente de dentro da sua rede.
			§ As sub-redes virtuais segmentam sua rede para atender suas necessidades
			§ O emparelhamento de rede conecta suas redes privadas diretamente.
			§ Gateway de VPN
				□ O gateway de VPN é usado para enviar tráfego criptografado entre uma rede virtual do azure e uma no local pela internet pública.
				□ 
			§ Express Route
				□ Estende as redes locais para o Azure por meio de uma conexão privada, facilitada por um provedor de conectividade
				□ 
			§ DNS do Azure
				□ Confiabilidade e desempenho aproveitando uma rede global de servidores de nome DNS usando a rede Anycast.
				□ A segurança do DNS do Azure baseia-se no gerenciador de recursos do Azure, habilitando o controle de acesso baseado em função e o monitoramento e o registro em log.
				□ Facilidade de uso para gerenciar seus recursos externos e do Azure com um único serviço DNS
				□ As redes virtuais personalizáveis permitem que você use nomes de domínio privados e totalmente personalizados em suas redes virtuais privadas.
        Os registros de alias dão suporte de conjuntos de registros de alias para apontar diretamente para um recurso do Azure.
