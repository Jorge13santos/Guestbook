# Guestbook exemplo

   Este exemplo mostra como criar um aplicativo da web simples de várias camadas usando Kubernetes e Docker
   O aplicativo consiste em um front-end da Web, mestre Redis para armazenamento e conjunto replicado de escravos Redis,
   para os quais criaremos implantações, pods e serviços do Kubernetes.
   
 # NOTAS 
     
   Os aplicativos dO Guestbook no meu teste foi no ambiente da DigitalOcean usando o tipo de serviço Kubernetes LoadBalancer 
   para expor o serviço em um endereço IP externo.
   
   Caso sua aplicações comece ser requisitada e voce precisar scalonar mais pods.
  # kubectl scale deployment frontend --replicas=4
