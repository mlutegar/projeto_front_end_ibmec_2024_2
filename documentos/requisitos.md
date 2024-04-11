# Requisitos do Sistema

## Narrativa Livre (Requisitos em linguagem natural)
- RN01: O sistema deve permitir que usuários inexperientes consigam operá-lo.
- RN02: O sistema deve permitir que o usuário anexe os resultados em pdf dos cálculos feitos pelo Slide 3D.
- RN03: O sistema deve fornecer uma interface para a visualização das solicitações pendente do cliente.
- RN04: O sistema deve fornecer uma interface para a visualização dos dados do paciente de uma solicitação do cliente.
- RN05: O sistema deve fornecer uma interface para a visualização imagens de calibração de uma solicitação do cliente.
- RN06: O sistema deve fornecer uma interface para a visualização das imagens do paciente de uma solicitação do cliente.
- RN07: O sistema deve permitir apenas que funcionários da Dosimagem acessem-no.
- RN08: O usuário deve poder acessar os históricos dos relatórios já criados.
- RN09: O usuário deve poder visualizar os dados e imagens dos pacientes relacionados às solicitações.
- RN10: O usuário deve poder baixar as imagens de calibração do cliente.
- RN11: O usuário deve poder baixar as imagens do paciente do cliente.

## Lista de requisitos do sistema (linguagem precisa e técnica, código para identificação) 
### Requisitos funcionais

#### Referente ao requisito natural 01 (RN01: O sistema deve permitir que usuários inexperientes consigam operá-lo)
- RF01-2: Incluir dicas contextuais em cada etapa da interface para fornecer orientações relevantes conforme necessário.
- RF01-2: Integrar um sistema de barra de progresso para orientar os usuários sobre seu progresso dentro do sistema.

#### Referente ao requisito natural 02 (RN02: O sistema deve permitir que o usuário anexe os resultados em pdf dos cálculos feitos pelo Slide 3D)
- RF02-1: Um botão para que os funcionários possam anexar o arquivo PDF do relatório à solicitação específica do cliente no painel de administrador.
- RF02-2: Desenvolver uma validação de formato para garantir que apenas arquivos PDF sejam aceitos como anexos.
- RF02-3: Incluir um sistema de limite de tamanho de arquivo para evitar anexos de PDF muito grandes que possam sobrecarregar o sistema.
- RF02-4: Desenvolver uma função de notificação para alertar os funcionários sobre o sucesso ou falha do processo de anexo de PDF.

#### Referente ao requisito natural 03 (RN03: O sistema deve fornecer uma interface para a visualização das solicitações pendente do cliente)
- RF03-1: Na interface de visualização das solicitações, deve ser exibida uma lista de todas as solicitações pendentes, ordenada pela coluna "criação data/hora".
- RF03-2: Cada solicitação na lista deve ser representada por uma linha na tabela, contendo as informações "ID", "Usuario do Cliente", "Tipo do Isotopo", "Nome da calibração" e "Criação data/hora", separadas por coluna.
- RF03-3: Deve haver opções de filtragem para permitir que os usuários reduzam a lista de solicitações pendentes com base em critérios específicos, como tipo de isótopo ou nome do cliente.
- RF03-4: Para cada solicitação, deve ser exibida uma coluna para o ID da solicitação, garantindo uma identificação única e inequívoca de cada item na lista.
- RF03-5: O sistema deve incluir uma coluna para o usuário do cliente associado a cada solicitação, exibindo o nome ou identificador do cliente responsável pela solicitação.
- RF03-6: Deve ser fornecida uma coluna para o tipo do isótopo relacionado a cada solicitação, indicando o isótopo específico envolvido na solicitação de calibração.
- RF03-7: Para cada solicitação, deve haver uma coluna para o nome da calibração solicitada, permitindo uma identificação clara e rápida do tipo de calibração necessária.
- RF03-8: Além disso, o sistema deve incluir uma coluna para a data e hora de criação da solicitação, fornecendo informações sobre quando a solicitação foi registrada no sistema.
- RF03-9: O sistema deve fornecer opções de paginação para lidar com grandes volumes de solicitações pendentes.
- RF03-10: Para cada solicitação na lista, deve haver um botão que permite visualizar a solicitação de forma mais detalhada.
  
#### Referente ao requisito natural 04 (RN04: O sistema deve permitir apenas que funcionários da Dosimagem acessem-no)
- RF04-1: Implementar um sistema de autenticação para verificar a identidade dos usuários antes de conceder acesso ao sistema.

#### Referente ao requisito natural 05 (RN05: O usuário deve poder acessar os históricos dos relatórios já criados)
- RF06-1: Deve haver uma página claramente identificada na interface do usuário para visualização dos dados e imagens dos pacientes relacionados às solicitações.
- RF06-2: Os dados dos pacientes devem seguir a ordem definida, começando pelo nome do paciente, seguido pelo tipo do exame, tipo da isometria, e assim por diante, conforme especificado.

#### Referente ao requisito natural 07 (RN07: O usuário deve poder baixar as imagens de calibração do cliente)
- RF07-1: Deve haver um botão visível e identificável, posicionado abaixo das imagens de calibração do cliente.
- RF07-2: Após a conclusão do download, o sistema deve notificar o usuário sobre o sucesso da operação.
- RF07-3: Caso ocorra algum erro durante o download, o sistema deve exibir uma mensagem de erro explicativa e orientar o usuário sobre como proceder.

#### Referente ao requisito natural 08 (RN08: O usuário deve poder baixar as imagens do paciente do cliente)
- RF08-1: Deve haver um botão claramente identificável, de cor cinza, posicionado abaixo da imagem pré-visualizada.
- RF08-2: Após a conclusão do download, o usuário deve receber uma notificação ou mensagem indicando que o download foi bem-sucedido.
- RF08-3: Caso ocorra algum erro durante o download, o sistema deve exibir uma mensagem de erro explicativa e orientar o usuário sobre como proceder.

### Requisitos não funcionais

- RNF-01: O front-end do sistema deve ser desenvolvido utilizando a biblioteca ReactJS
