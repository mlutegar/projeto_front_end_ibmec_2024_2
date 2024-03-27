# Requisitos do Sistema

## Narrativa Livre (Requisitos em linguagem natural)
- O sistema deve permitir que funcionários inexperientes consigam operá-lo.
- O sistema deve permitir que o funcionários anexe os resultados dos cálculos feitos pelo Slide 3D.
- O sistema deve apresentar uma interface amigável ao usuário.
- O sistema deve fornecer uma interface para a criação de relatórios e resultados de exames.
- O sistema deve permitir apenas que funcionários da Dosimagem acessem-no.
- O sistema precisa enviar o relatório criado para o site principal, onde foi feita a solicitação do relatório.
- Os funcionários devem poder acessar os históricos dos relatórios já criados.
- Os funcionários devem ser capazes de visualizar as solicitações recebidas.
- Os funcionários devem poder visualizar os dados e imagens dos pacientes relacionados às solicitações.
- Os funcionários devem poder baixar as imagens de calibração e do cliente.

## Lista de requisitos do sistema (linguagem precisa e técnica, código para identificação) 
### Requisitos funcionais

- RF-01: O nome do relatório deve ser padronizado e informativo (por exemplo, "Relatório_<nome da clinica>_<data>.pdf").
- RF-02: Um botão para que os funcionários possam anexar o arquivo PDF do relatório à solicitação específica do cliente no painel de administrador.
- RF-03: Um botão para download das imagens de calibração.
- RF-04: Um botão para download do arquivo zip contendo as imagens do paciente.
- RF-05: Uma interface que exiba os dados e anexos dos pacientes associados a cada solicitação.
- RF-06: Uma interface onde os funcionários possam ver todas as solicitações recebidas.
- RF-07: Um sistema de autenticação para que os funcionários possam acessar o painel de administrador do site.

### Requisitos não funcionais

- RNF-01: O front-end do sistema deve ser desenvolvido utilizando a biblioteca ReactJS