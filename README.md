# Mineração de Conhecimento

Na plataforma do Azure, criaremos três recursos:

    - Serviço de IA do Azure:
    - Serviços cognitivos:
    - Conta de Armazenamento:

## Configurando conta de Armazenamento

 - Ao acessar a conta, buscaremos configurações
 - Ativaremos a opção de permitir acesso anonimo ao job
 - Acessaremos o item containers e criaremos um container
    - Escolher opção container e adicionaremos um nome ao container

 - Clicar no container criado e acessar a opção carregar
 - Escolher arquivos de texto desejado e importá-los para a conta.

 ## Configurar Serviço de IA

 - Acessar o serviço de IA do Azure criado
 - Buscar a opção importar dados
 - Escolheremos a fonte de dados como armazenamento de blobs do azure
 - Preenchemos os campos de nome de origem
 - Na cadeia de ligação, vamos na opção selecionar uma ligação existente
    - Vamos selecionar a conta de armazenamento criada e, dentro dela, nosso container criado

- Em Anexar recursos de IA, manteremos o escolhido para o recurso
- Em adicionar melhoramentos:

    - Adicionar nome a aplicação
    - Marcar "Ativar OCR e intercalar todo o texto com campo merge_content"
    - Marcar opçoes:
        - Extrair nomes de localização
        - Detectar sentimentos
        - Competencias cognitvas de imagem
        - Gerar etiquetas a partir de imagens
        - Gerar legendas a apartir de imagens

 - Em cadeia de conexão, escolheremos a opção procurar por uma conexão existente, buscaremos a conta de armazenamento e o container criado nela
 - Em projeções de ficheiros, marcaremos:
    - Projeções de imagens

 - Em projeções de tabelas, marcaremos:
    - Documentos
    - Paginas
    - Entidades
    - Detalhes de imagem
    - Referencia de imagem

 - Em projeções de Blobs do Azure, marcaremos:
    - Documento

 - Em criar indexadores, vamos nomear o indíce a ser criado e manteremos a opção agenda em "uma vez"
 - Encerrar importação

 - No Serviço de IA do Azure, na guia indexadores, encontraremos as informações de criação dos índices.
 - Na página inicial do Serviço de IA do Azure, Acessaremos a guia "Explorador de procura"
 - Nessa guia é possível buscar informações nos arquivos filtrando eles pelo índice criado
 - Nele podemos adicionar pesquisa por informações por meio de informações json, o resultado da procura nos documentos é retornado abaixo
