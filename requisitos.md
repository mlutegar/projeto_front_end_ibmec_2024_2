# Requisitos do Sistema
Com base nas especificações fornecidas, apresentamos abaixo os requisitos detalhados do sistema de relatórios da Dosimagem. Estes requisitos foram elaborados para garantir um sistema eficiente e intuitivo, capaz de atender às necessidades específicas da empresa. Por meio deste documento, descrevemos as funcionalidades essenciais e as características fundamentais do sistema, visando proporcionar uma experiência fluida e satisfatória aos usuários.

## Narrativa Livre (Requisitos em linguagem natural)
- O sistema deve permitir que usuários inexperientes consigam operá-lo.
- O sistema deve permitir que o usuário anexe mais de uma imagem de uma só vez.
- O sistema deve possibilitar a adição intuitiva de imagens aos relatórios.
- O sistema deve permitir que o usuário anexe os resultados dos cálculos feitos por software externo.
- O sistema deve apresentar uma interface amigável ao usuário.
- O sistema deve fornecer uma interface para a criação de relatórios, com suporte para inclusão de imagens e resultados de exames.
- O sistema deve apresentar a criação de um relatório como um assistente passo a passo.
- O sistema deve possibilitar a geração de relatórios em formato PDF.
- O sistema deve permitir apenas que funcionários da Dosimagem acessem-no.
- O sistema precisa alertar caso algum dado esteja faltando durante a criação do relatório.
- O sistema precisa enviar o relatório criado para o site principal, onde foi feita a solicitação do relatório.
- Os usuários devem poder acessar os históricos dos relatórios já criados.
- O sistema devera organizar as informações de forma intuitiva facilitando a localização de informações relevantes, agrupando-as por categorias e utilizando recursos visuais como ícones e menus. 

## Lista de requisitos do sistema (linguagem precisa e técnica, código para identificação) 
### Usabilidade:

- **US-1**: A interface do sistema deve ser intuitiva e fácil de usar, com ícones e menus autoexplicativos.
- **US-2**: O sistema deve fornecer dicas e instruções contextuais para auxiliar o usuário na execução de tarefas.
- **US-3**: As tarefas do sistema devem ser divididas em etapas pequenas e fáceis de seguir.
- **US-4**: O sistema deve oferecer uma interface para criação de relatórios, com suporte para inclusão de imagens e resultados de exames.

### Desempenho:

- **EF-1**: O sistema deve permitir o usuário anexar múltiplas imagens simultaneamente.
- **EF-2**: O sistema deve facilitar a adição de imagens aos relatórios de forma intuitiva.
- **EF-3**: O sistema deve permitir que o usuário anexe resultados de cálculos feitos por software externo.
- **EF-4**: O sistema deve possibilitar a geração de relatórios em formato PDF.
- **EF-5**: O sistema deve enviar automaticamente o relatório criado para o site principal, onde a solicitação foi feita.
- **EF-6**: Os usuários devem ter acesso aos históricos dos relatórios já criados.
- **EF-7**: O sistema deve fornecer uma pré-visualização das imagens selecionadas antes de anexá-las.

### Integridade e Confiabilidade:

- **CF-1**: O sistema deve alertar o usuário caso haja dados faltantes durante a criação do relatório.
- **CF-2**: O acesso ao sistema deve ser restrito apenas a funcionários da Dosimagem
- **CF-3**: O sistema deve notificar o usuário sobre o sucesso ou falha da operação de anexar os arquivos.
- **CF-4**: O nome do relatório deve ser padronizado e informativo (por exemplo, "Relatório_<nome_clinica_<data>.pdf").
- **CF-5**: O sistema deve registrar erros que possam ocorrer durante o envio do relatório em um log de erros.

### Manutenibilidade:
- **MT-1**: O sistema deve validar que os arquivos upados sejam arquivos válidos (JPEG, PNG, PDF, etc.).
- **MT-2**: O sistema deve validar que os arquivos upados não excedam o tamanho máximo permitido por arquivo.

### Acessibilidade:
- **AS-1**: O sistema deve fornecer recursos de acessibilidade, como leitores de tela, lupas e navegação por teclado.
