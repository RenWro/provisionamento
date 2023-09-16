# Provisionamento
Provisionamento como Código (AWS)


<h1>Implantação de WordPress com Amazon ECS usando AWS CloudFormation</h1>



<h1>Descrição</h1>


Este projeto consiste em criar uma pilha do AWS CloudFormation para implantar um ambiente altamente disponível do WordPress usando o Amazon ECS (Elastic Container Service). O ambiente incluirá um cluster ECS, uma definição de tarefa, um serviço, um balanceador de carga, dimensionamento automático e um sistema de arquivos EFS para armazenar dados persistentes do WordPress.

<h1>Pré-requisitos</h1>


<h2>Antes de iniciar a implantação,foram realizados os seguintes passos:</h2>


1. Conta da AWS com permissões para criar recursos.
2. AWS CLI configurado com as credenciais adequadas.
3. Conhecimento básico sobre o uso do AWS CloudFormation.

<h1>Passos de Implantação</h1>

<h2>Template do CloudFormation</h2>

No repositório, foi criado um arquivo chamado ecs-wordpress-stack.yml (ou outro nome de escolha) que continha o template do CloudFormation. Este arquivo definiu todos os recursos necessários para a infraestrutura.

<h2>Infraestrutura</h2>

No template do CloudFormation, foram definidos os seguintes recursos:

1. Um cluster ECS para hospedar os containers do WordPress.
2. Uma definição de tarefa que especificava como os containers do WordPress seriam configurados.
3. Um serviço ECS para garantir que a tarefa do WordPress fosse sempre executada.
4. Um balanceador de carga para distribuir o tráfego entre os containers.
5. Configurações de dimensionamento automático para ajustar automaticamente o número de containers com base na carga.
6. Um sistema de arquivos EFS para armazenar dados persistentes do WordPress.



<h2>Parâmetros</h2>



No template, foram utilizados parâmetros para permitir a personalização durante a criação da pilha, como nome do cluster, tamanho da instância, etc.




<h2>Documentação do Template</h2>



Foram fornecidos comentários claros no template para explicar a finalidade de cada recurso e parâmetro. Isso ajudou outros desenvolvedores a entenderem e personalizarem a implantação conforme necessário.



<h2>Implanração da Pilha</h2>



A pilha foi implantada através do CLI ou do Management Console da AWS, a escolha foi livre.



<h2>Verificação do Ambiente</h2>



Após a conclusão da implantação, verificou-se se o ambiente do WordPress estava funcionando corretamente. O endereço do balanceador de carga foi acessado para acessar o WordPress.



<h2>Recursos Adicionais</h2>


<a href="https://docs.aws.amazon.com/cloudformation/index.html" target="_blank">Link para a Documentação Oficial da AWS CloudFormation</a>




<h2>Autoras</h2>


Ana Bea Ferraz

Bruna Leal

Kamilla Antunes

Ren Wrobleski


<h2>Licença</h2>

Este projeto está licenciado sob a licença MIT.

<h2>Contribuições</h2>

Contribuições são bem-vindas! Sinta-se à vontade para abrir um problema ou enviar um pull request.






