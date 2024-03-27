# Casos de Uso

## Caso de Uso 1: Solicitar Serviço

### Descrição:
Este caso de uso descreve o processo pelo qual um cliente solicita um serviço à Dosimagem, enviando imagens de calibração e do paciente para receber um relatório.

### Ator Principal: 
Cliente

### Pré-condições:
O cliente deve ter acesso ao site da dosimagem.
O cliente deve estar cadastrado no sistema.

### Fluxo Principal:
1. O cliente faz login no site da dosimagem.
2. O cliente acessa a opção de solicitação de serviço.
3. O sistema solicita as imagens de calibração para cada máquina que realizará a simetria.
4. O cliente envia as imagens de calibração.
5. O cliente compacta as imagens do paciente em um arquivo ZIP.
6. O cliente seleciona a calibração a ser usada.
7. O sistema recebe as imagens de calibração e do paciente.
8. O sistema gera o relatório com base nas informações fornecidas.
9. O sistema notifica o cliente quando o relatório estiver pronto.

### Pós-condições:
O relatório está disponível para o cliente.

## Caso de Uso 2: Processar Solicitações de Serviço

### Descrição:
Neste caso de uso, um funcionário da Dosimagem processa as solicitações de serviço pendentes, baixando as imagens de calibração e do paciente, enviando para o software 3D Slice para geração de relatório, e anexando o relatório à solicitação do cliente.

### Ator Principal: 
Funcionário da Dosimagem

### Pré-condições:
O funcionário deve ter acesso ao sistema de administrador da dosimagem.
Existem solicitações de serviço pendentes.

### Fluxo Principal:
1. O funcionário faz login no sistema da dosimagem.
2. O funcionário acessa o painel de administração.
3. O sistema exibe as solicitações de serviço pendentes.
4. O funcionário seleciona uma calibração de um cliente A.
5. O sistema exibe as imagens de calibração enviadas pelo cliente.
6. O funcionário baixa as imagens de calibração.
7. O funcionário seleciona uma solicitação de um cliente A.
8. O sistema exibe as imagens disponiveis do paciente e seus dados.
9. O funcionário baixa as imagens do paciente.
10. O funcionário envia as os dados e imagens do cliente e da calibração para o software 3D Slice.
11. O software gera o relatório com base nas imagens e informações recebidas.
12. O funcionário anexa o relatório na solicitação do cliente A.
13. O funcionário anexa o PDF à solicitação do cliente.

### Pós-condições:
O relatório está anexado à solicitação do cliente.

## Caso de Uso 3: Monitorar Status de Solicitações de Serviço

### Descrição:
Este caso de uso descreve como um funcionário da Dosimagem monitora o status das solicitações de serviço em andamento, verificando e atualizando o progresso das solicitações conforme necessário.

### Ator Principal:
Funcionário da Dosimagem

### Pré-condições:
- O funcionário deve ter acesso ao sistema da Dosimagem.
- Existir solicitações de serviço em andamento.

### Fluxo Principal:
1. O funcionário faz login no sistema da dosimagem.
2. O funcionário acessa o painel de controle de solicitações de serviço.
3. O sistema exibe uma lista das solicitações dos pacientes em andamento.
4. O funcionário seleciona uma solicitação para visualizar mais detalhes.
5. O sistema exibe o status atual da solicitação, como "Dados enviados", "Verificando Informações", "Informações Inválidas", "Processando a análise" ou "Análise concluída".
6. O funcionário verifica se há alguma ação necessária para avançar com a solicitação.
7. Se necessário, o funcionário atualiza o status da solicitação no sistema.
8. O funcionário pode adicionar notas ou comentários à solicitação, se necessário.

### Pós-condições:
- O status das solicitações é atualizado conforme as ações realizadas pelo funcionário, permitindo um acompanhamento eficaz do progresso dos serviços de imagem médica.

## Caso de Uso 4: Receber Relatório de Serviço

### Descrição:
Neste caso de uso, um cliente acessa o sistema da Dosimagem para receber um relatório de serviço previamente solicitado, selecionando-o na lista disponível e fazendo o download do relatório gerado.

### Ator Principal:
Cliente

### Pré-condições:
O cliente deve ter acesso ao sistema da Dosimagem. O relatório de serviço deve estar pronto para entrega.

### Fluxo Principal:
1. O cliente faz login no sistema da Dosimagem.
2. O cliente acessa a lista de relatórios de serviço prontos para entrega.
3. O sistema exibe os relatórios disponíveis para o cliente.
4. O cliente seleciona o relatório desejado para recebimento.
5. O sistema gera uma cópia do relatório para o cliente.
6. O cliente faz download do relatório gerado.

### Pós-condições:
O relatório é entregue ao cliente com sucesso.

### Caso de Uso 5:Atualizar Informações do Paciente

### Ator Principal: 
Cliente.
### Pré-condições:
O cliente deve ter acesso ao site dosImagem.
O cliente deve estar cadastrado no sistema.
### Fluxo Principal:
O cliente faz login no site dosImagem.
O cliente acessa a opção de perfil do paciente.
O sistema exibe as informações atuais do paciente.
O cliente atualiza as informações conforme necessário.
O cliente salva as alterações.
### Pós-condições:
As informações do paciente são atualizadas no sistema.
