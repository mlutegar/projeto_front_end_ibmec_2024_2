# Requisitos do Sistema

## Narrativa Livre (Requisitos em linguagem natural)
- RN01: O sistema deve permitir que usuários inexperientes consigam operá-lo.
- RN02: O sistema deve permitir que o usuário anexe os resultados em pdf dos cálculos feitos pelo Slide 3D.
- RN03: O sistema deve fornecer uma interface para a visualização das solicitações do cliente.
- RN04: O sistema deve permitir apenas que funcionários da Dosimagem acessem-no.
- RN05: O usuário deve poder acessar os históricos dos relatórios já criados.
- RN06: O usuário deve poder visualizar os dados e imagens dos pacientes relacionados às solicitações.
- RN07: O usuário deve poder baixar as imagens de calibração do cliente.
- RN08: O usuário deve poder baixar as imagens do paciente do cliente.

## Lista de requisitos do sistema (linguagem precisa e técnica, código para identificação) 
### Requisitos funcionais

#### Referente ao requisito natural 01
- RF01-2: Incluir dicas contextuais em cada etapa da interface para fornecer orientações relevantes conforme necessário.
- RF01-2: Integrar um sistema de barra de progresso para orientar os usuários sobre seu progresso dentro do sistema.

#### Referente ao requisito natural 02
- RF02-1: Um botão para que os funcionários possam anexar o arquivo PDF do relatório à solicitação específica do cliente no painel de administrador.
- RF02-2: Desenvolver uma validação de formato para garantir que apenas arquivos PDF sejam aceitos como anexos.
- RF02-3: Incluir um sistema de limite de tamanho de arquivo para evitar anexos de PDF muito grandes que possam sobrecarregar o sistema.
- RF02-4: Desenvolver uma função de notificação para alertar os funcionários sobre o sucesso ou falha do processo de anexo de PDF.

#### Referente ao requisito natural 03
- RF03-1: Na tela de cada solicitação precisa ter o nome do cliente, dados do cliente como: ....

#### Referente ao requisito natural 04
- RF04-1: Implementar um sistema de autenticação para verificar a identidade dos usuários antes de conceder acesso ao sistema.

#### Referente ao requisito natural 07
- RF07-1: Deve haver um botão visível e identificável, posicionado abaixo das imagens de calibração do cliente.
- RF07-2: Após a conclusão do download, o sistema deve notificar o usuário sobre o sucesso da operação.
- RF07-3: Caso ocorra algum erro durante o download, o sistema deve exibir uma mensagem de erro explicativa e orientar o usuário sobre como proceder.

#### Referente ao requisito natural 08
- RF08-1: Deve haver um botão claramente identificável, de cor cinza, posicionado abaixo da imagem pré-visualizada.
- RF08-2: Após a conclusão do download, o usuário deve receber uma notificação ou mensagem indicando que o download foi bem-sucedido.
- RF08-3: Caso ocorra algum erro durante o download, o sistema deve exibir uma mensagem de erro explicativa e orientar o usuário sobre como proceder.

### Requisitos não funcionais

- RNF-01: O front-end do sistema deve ser desenvolvido utilizando a biblioteca ReactJS