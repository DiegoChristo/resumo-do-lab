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

