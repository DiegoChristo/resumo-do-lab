# resumo-do-lab
Este repositorio tem como finalidade os projetos para a DIO
Como resumo desse lab percebi que as empresas por onde pssei poderiam tem estruturas melhores trbalhndo em nuvem com seus sistemas e ferramentas.
benefícios da nuvem

disponibilidade - sempre funciona se o sla não for cumprido uma porcentagem do valor é devolvido 
escalabilidade - pagando apenas pelos serviços necessários
elasticidade - recursos expandindo automaticamente ou manualmente
confiabilidade - configurar replicações e não fica sem sistema
previsibilidade - confiança para avançar com desempenho e custo
segurança - o cliente também é responsável
governança - auditoria
gerenciabilidade - escalar a implantação de recursos de acordo com a necessidade

benefícios da nuvem

disponibilidade - sempre funciona se o sla não for cumprido uma porcentagem do valor é devolvido 
escalabilidade - pagando apenas pelos serviços necessários
elasticidade - recursos expandindo automaticamente ou manualmente
confiabilidade - configurar replicações e não fica sem sistema
previsibilidade - confiança para avançar com desempenho e custo
segurança - o cliente também é responsável
governança - auditoria
gerenciabilidade - escalar a implantação de recursos de acordo com a necessidade
     configurando uma maquina
quanto mais 9 menor o tempo de indisponibilidade, dicas de segurança são dados em mais de uma localidade

      tipos de serviços em nuvem
iaaS infra, paas plataforma, saas sistemas  

iaas - servidores - segurança de rede - planta física- serviço flexível - configura e gerencia o hardware para o su app

Paas - tudo IaaS + sistemas operacionais - ferramentas para dev - focado em desenvolver app - o gerenciamento é realizado pelo provedor de nuvem

Saas - iaas, paas + aplicativos - preço pago pelo uso - sw por assinatura

modelo de responsabilidade compartilhada
no local físico tudo é de responsabilidade da empresa


Componentes e arquitetura do azure.

Regiões e zonas de disponibilidade
Assinaturas e grupos de recursos

_ componentes - podemos criar recursos em varias regiões cada região é composto de um ou mais DC próximos
flexibilidade para reduzir latencia 

pares de regiões
300 milhas de distancia, replica automática para alguns serviços
recuperação de região priorizada em caso de interrupção

projeto

_estrutura global azure
-disponibilidade
-DC - estruturas e projetos
-regiões - brasil - são Paulo ( rio de janeiro em caso de desastre recovery ) replica para US - o cliente precisa requerer a MS o recovery para o Rj por questões de dados que não pode sair do brasil
algumas replicações são feitas no brasil

grupo de recursos
-assinatura - sua assinatura ou escolha quando tiver mais de uma
-grupo de recursos - é uma coleção, ciclo de vida, politica, permissões
-região - alguns recursos especifico pode não esta habilitado em algumas regiões ai aparece em cinza
Marcações
nome - marcações ou tag - centro de custo
valor - o valor pelos recursos.

arquitetura e serviços 
- tipos de computação
- hospedagem de aplicativos
- redes virtuais
-- computação do azure é um serviço sob demanda que fornece recursos de computação, como discos, processadores, memoria, rede e sistemas
--- maquinas virtuais (VMs)
---- emulação de sw de computadores físicos
---- inclui processadores virtuais, memoria, armazenamento e redes
---- oferta de infra que oferece personalização e controle total
- conjunto de dimensionamento de VMs
-- os conjuntos de dimensionamentos oferecem uma oportunidade de balanceamento de carga para dimensionar os recursos automaticamente 
- Conjunto de disponibilidade de maquinas virtuais
-- são distribuídas em rack de falhas
--- cada linhas de maquinas são distribuídas de linhas de atualização
- área de trabalho virtual azure
-- podemos configurar maquinas exclusivas ou compartilhada
- contêineres do azure - PaaS - AKS
-- uma maquina física com varias maquinas virtuais
-- Docker
--kubernetes - orquestração para contêineres
- azure functions e serviços de app azure
-- código baseado em eventos é executado quando chamado sem precisar de infra do servidor durante período inativo
-- serviços de app azure
--- trabalha com .NET, .NET CORE, NDES.JS, JAVA, PYTHON OU PHP

       armazenamento

- Redundancia de armazenamento
-- LRS - armazenamento local - região primaria
-- ZRS - armazenamento de zona - 3 zonas de disponibilidade na região primaria
-- GRS - armazenamento geográfico - único no primário e região secundaria
-- GZRS - armazenamento de zona geográfica - 3 zonas de disponibilidade na região primaria e um na região secundaria.
- blobs
- data lake storage
- filas
- tabelas
    camadas de acesso
- frequente
- esporádico - 30 dias
- frio - 90 dias
- arquivo morto - 180 dias
    migração para azure
- plataforma de migração
- intervalo de ferramentas integradas e autônomas
- avaliação e migração
    azure data box
- ate 80 tb de dados
     azcopy
- utilitário de linha de comando
- copiar blobs ou arquivos de ou para sua conta de armazenamento
- sincronização em uma direção
    gerenciador de armazenamento azure
- interface gráfica
- compatível com o Windows, MacOS e Linux


   Identidade, acesso e segurança
- Serviços de diretório
- Métodos de autenticação
- Modelos de segurança

entra id e domain services
- serviço de gerenciamento de identidades e acessos baseados em nuvem do azure

- MS entra ID
-- copia os usuários para a nuvem ( usuários criados na nuvem não são importados para o on-premices )
--- permanentemente deletado o usuário após 30 dias




