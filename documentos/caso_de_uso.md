# Casos de Uso

![Caso de uso](https://github.com/mlutegar/projeto_front_end_ibmec_2024_2/blob/casos_de_uso/documentos/imgs/casos_de_uso.png)

## Caso de Uso 1
### Titulo: Solicitar Serviço

### Descrição:
Este caso de uso descreve o processo pelo qual um cliente solicita um serviço à Dosimagem, enviando imagens de calibração e do paciente para receber um relatório.

### Ator Principal: 
Cliente

### Pré-condições:
O cliente deve ter acesso ao site da dosimagem.
O cliente deve estar cadastrado no sistema.

### Fluxo Principal:
1. O cliente faz login no site da dosimagem. (Caso de uso 6: Login no Sistema dosImagem)
2. O cliente acessa a opção de solicitação de serviço.
3. O cliente acessa a aba de envio de calibração.
4. O sistema solicita as imagens de calibração para cada máquina que realizará a simetria.
5. O cliente envia as imagens de calibração.
6. O sistema recebe as imagens de calibração
7. O cliente acessa a aba de envio de dados do paciente.
8. O sistema solicita os dados e as fotos do paciente.
9. O cliente compacta as imagens do paciente em um arquivo ZIP.
10. O cliente seleciona a calibração a ser usada.
11. O sistema recebe os dados e as imagens e do paciente.
12. (Caso de uso 2: Processar Solicitações de Serviço)
13. O sistema notifica o cliente quando o relatório estiver pronto.

### Pós-condições:
O relatório está disponível para o cliente.

## Caso de Uso 2
### Titulo: Processar Solicitações de Serviço

### Descrição:
Neste caso de uso, um funcionário da Dosimagem processa as solicitações de serviço pendentes, baixando as imagens de calibração e do paciente, enviando para o software 3D Slice para geração de relatório, e anexando o relatório à solicitação do cliente.

### Ator Principal: 
Funcionário da Dosimagem

### Pré-condições:
O funcionário deve ter acesso ao sistema de administrador da dosimagem.
Existem solicitações de serviço pendentes.

### Fluxo Principal:
1. O funcionário faz login no sistema da dosimagem. (Caso de uso 6: Login no Sistema dosImagem)
2. O funcionário acessa o painel de administração.
3. O sistema exibe as solicitações de serviço pendentes.
4. O funcionário escolhe a solicitação pendente que pretende processar. (Caso de uso 5: Baixar Arquivos de Paciente e Calibração)
5. O funcionário baixa as imagens do paciente e da calibração do cliente A selecionado.
6. O funcionário envia os dados e imagens do cliente e da calibração para o software 3D Slice.
7. O software gera o relatório com base nas imagens e informações recebidas.
8. O funcionário anexa o relatório na solicitação do cliente A.
9. O funcionário encerra a solicitação do cliente A. (Caso de Uso 3: Monitorar Status de Solicitações de Serviço)

### Pós-condições:
O relatório está anexado à solicitação do cliente.

## Caso de Uso 3
### Titulo: Monitorar Status de Solicitações de Serviço

### Descrição:
Este caso de uso descreve como um funcionário da Dosimagem monitora o status das solicitações de serviço em andamento, verificando e atualizando o progresso das solicitações conforme necessário.

### Ator Principal:
Funcionário da Dosimagem

### Pré-condições:
- O funcionário deve ter acesso ao sistema da Dosimagem.
- Existir solicitações de serviço em andamento.

### Fluxo Principal:
1. O funcionário faz login no sistema da dosimagem. (Caso de uso 6: Login no Sistema dosImagem)
2. O funcionário acessa o painel de controle de solicitações de serviço.
3. O sistema exibe uma lista das solicitações dos pacientes em andamento.
4. O funcionário seleciona uma solicitação para visualizar mais detalhes.
5. O sistema exibe o status atual da solicitação, como "Dados enviados", "Verificando Informações", "Informações Inválidas", "Processando a análise" ou "Análise concluída".
6. O funcionário verifica se há alguma ação necessária para avançar com a solicitação.
7. Se necessário, o funcionário atualiza o status da solicitação no sistema.

### Pós-condições:
- O status das solicitações é atualizado conforme as ações realizadas pelo funcionário, permitindo um acompanhamento eficaz do progresso dos serviços de imagem médica.

## Caso de Uso 4
### Titulo: Receber Relatório de Serviço

### Descrição:
Neste caso de uso, um cliente acessa o sistema da Dosimagem para receber um relatório de serviço previamente solicitado, selecionando-o na lista disponível e fazendo o download do relatório gerado.

### Ator Principal:
Cliente

### Pré-condições:
O cliente deve ter acesso ao sistema da Dosimagem. O relatório de serviço deve estar pronto para entrega.

### Fluxo Principal:
1. O cliente faz login no sistema da Dosimagem. (Caso de uso 6: Login no Sistema dosImagem)
2. O cliente acessa a lista de relatórios de serviço prontos para entrega.
3. O sistema exibe os relatórios disponíveis para o cliente.
4. O cliente seleciona o relatório desejado para recebimento.
5. O sistema gera uma cópia do relatório para o cliente.
6. O cliente faz download do relatório gerado.

### Pós-condições:
O relatório é entregue ao cliente com sucesso.

## Caso de Uso 5
### Título: Baixar Arquivos de Paciente e Calibração

### Descrição:
Neste caso de uso, um funcionário da Dosimagem realiza o download dos arquivos necessários, incluindo as imagens do paciente e da calibração, para processar uma solicitação de serviço.

### Ator Principal:
Funcionário da Dosimagem

### Pré-condições:
- O funcionário deve estar autenticado no sistema da Dosimagem.
- Existem solicitações de serviço pendentes que requerem o download de arquivos de paciente e calibração.

### Fluxo Principal:
1. O funcionário acessa o sistema da Dosimagem.
2. O funcionário navega até o painel de administração.
3. O sistema exibe uma lista das solicitações de serviço pendentes.
4. O funcionário seleciona uma solicitação específica para processamento.
5. O sistema exibe as informações da solicitação, incluindo detalhes do paciente e as calibrações necessárias.
7. O funcionário seleciona as aba de imagens do paciente.
8. O sistema oferece opções para baixar os arquivos selecionados.
9. O funcionário confirma o download dos arquivos.
10. O funcionário entra na seção de calibração.
11. O sistema oferece opções para baixar os arquivos selecionados.
12. O funcionário confirma o download dos arquivos.

### Pós-condições:
- Os arquivos necessários, incluindo as imagens do paciente e da calibração, são baixados com sucesso, prontos para serem processados conforme necessário.

## Caso de Uso 6
### Título: Login no Sistema dosImagem

### Descrição:
Este caso de uso descreve o processo pelo qual um usuário acessa o sistema dosImagem através de autenticação, fornecendo suas credenciais de login.

### Ator Principal:
Usuário

### Pré-condições:
- O usuário deve ter acesso ao site dosImagem.
- O usuário deve estar cadastrado no sistema dosImagem.

### Fluxo Principal:
1. O usuário acessa o site dosImagem. 
2. O usuário seleciona a opção de login.
3. O sistema exibe os campos de entrada para nome de usuário e senha.
4. O usuário insere seu nome de usuário e senha.
5. O sistema verifica as credenciais do usuário.
6. Se as credenciais estiverem corretas, o sistema autentica o usuário e concede acesso ao sistema.
7. Se as credenciais estiverem incorretas, o sistema exibe uma mensagem de erro e permite que o usuário tente novamente.

### Pós-condições:
O usuário está autenticado no sistema dosImagem e pode acessar as funcionalidades disponíveis de acordo com seu perfil de usuário.
