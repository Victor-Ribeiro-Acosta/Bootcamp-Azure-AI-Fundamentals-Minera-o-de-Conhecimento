# Mineração de Conhecimento

Na plataforma do Azure, criaremos três recursos:

- Serviço de IA do Azure:
  
  ![](https://github.com/Victor-Ribeiro-Acosta/Bootcamp-Azure-AI-Fundamentals-Mineracao-de-Conhecimento/blob/main/Passos/3.png)

  ![](https://github.com/Victor-Ribeiro-Acosta/Bootcamp-Azure-AI-Fundamentals-Mineracao-de-Conhecimento/blob/main/Passos/4.png)

  ![](https://github.com/Victor-Ribeiro-Acosta/Bootcamp-Azure-AI-Fundamentals-Mineracao-de-Conhecimento/blob/main/Passos/5.png)

- Serviços cognitivos:

  ![](https://github.com/Victor-Ribeiro-Acosta/Bootcamp-Azure-AI-Fundamentals-Mineracao-de-Conhecimento/blob/main/Passos/2.png)

- Conta de Armazenamento:
  
  ![](https://github.com/Victor-Ribeiro-Acosta/Bootcamp-Azure-AI-Fundamentals-Mineracao-de-Conhecimento/blob/main/Passos/6.png)
  
  ![](https://github.com/Victor-Ribeiro-Acosta/Bootcamp-Azure-AI-Fundamentals-Mineracao-de-Conhecimento/blob/main/Passos/7.png)


## Configurando conta de Armazenamento

 - Ao acessar a conta, buscaremos configurações

![](https://github.com/Victor-Ribeiro-Acosta/Bootcamp-Azure-AI-Fundamentals-Mineracao-de-Conhecimento/blob/main/Passos/8.png)

 - Ativaremos a opção de permitir acesso anonimo ao job

![](https://github.com/Victor-Ribeiro-Acosta/Bootcamp-Azure-AI-Fundamentals-Mineracao-de-Conhecimento/blob/main/Passos/9.png)
![](https://github.com/Victor-Ribeiro-Acosta/Bootcamp-Azure-AI-Fundamentals-Mineracao-de-Conhecimento/blob/main/Passos/10.png)

 - Acessaremos o item containers e criaremos um container
    - Escolher opção container e adicionaremos um nome ao container

![](https://github.com/Victor-Ribeiro-Acosta/Bootcamp-Azure-AI-Fundamentals-Mineracao-de-Conhecimento/blob/main/Passos/11.png)

 - Clicar no container criado e acessar a opção carregar

![](https://github.com/Victor-Ribeiro-Acosta/Bootcamp-Azure-AI-Fundamentals-Mineracao-de-Conhecimento/blob/main/Passos/12.png)
![](https://github.com/Victor-Ribeiro-Acosta/Bootcamp-Azure-AI-Fundamentals-Mineracao-de-Conhecimento/blob/main/Passos/13.png)

 - Escolher arquivos de texto desejado e importá-los para a conta.

 ## Configurar Serviço de IA

 - Acessar o serviço de IA do Azure criado
 - Buscar a opção importar dados

![](https://github.com/Victor-Ribeiro-Acosta/Bootcamp-Azure-AI-Fundamentals-Mineracao-de-Conhecimento/blob/main/Passos/21.png)

 - Escolheremos a fonte de dados como armazenamento de blobs do azure

![](https://github.com/Victor-Ribeiro-Acosta/Bootcamp-Azure-AI-Fundamentals-Mineracao-de-Conhecimento/blob/main/Passos/14.png)

 - Preenchemos os campos de nome de origem

![](https://github.com/Victor-Ribeiro-Acosta/Bootcamp-Azure-AI-Fundamentals-Mineracao-de-Conhecimento/blob/main/Passos/15.png)

 - Na cadeia de ligação, vamos na opção selecionar uma ligação existente
    - Vamos selecionar a conta de armazenamento criada e, dentro dela, nosso container criado

- Em Anexar recursos de IA, manteremos o escolhido para o recurso

![](https://github.com/Victor-Ribeiro-Acosta/Bootcamp-Azure-AI-Fundamentals-Mineracao-de-Conhecimento/blob/main/Passos/16.png)

- Em adicionar melhoramentos:

    - Adicionar nome a aplicação
    - Marcar "Ativar OCR e intercalar todo o texto com campo merge_content"
    - Marcar opçoes:
        - Extrair nomes de localização
        - Detectar sentimentos
        - Competencias cognitvas de imagem
        - Gerar etiquetas a partir de imagens
        - Gerar legendas a apartir de imagens

![](https://github.com/Victor-Ribeiro-Acosta/Bootcamp-Azure-AI-Fundamentals-Mineracao-de-Conhecimento/blob/main/Passos/17.png)

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
![](https://github.com/Victor-Ribeiro-Acosta/Bootcamp-Azure-AI-Fundamentals-Mineracao-de-Conhecimento/blob/main/Passos/18.png)

 - Em criar indexadores, vamos nomear o indíce a ser criado e manteremos a opção agenda em "uma vez"
 - Encerrar importação
![](https://github.com/Victor-Ribeiro-Acosta/Bootcamp-Azure-AI-Fundamentals-Mineracao-de-Conhecimento/blob/main/Passos/19.png)

 - No Serviço de IA do Azure, na guia indexadores, encontraremos as informações de criação dos índices.
![](https://github.com/Victor-Ribeiro-Acosta/Bootcamp-Azure-AI-Fundamentals-Mineracao-de-Conhecimento/blob/main/Passos/20.png)

 - Na página inicial do Serviço de IA do Azure, Acessaremos a guia "Explorador de procura"
![](https://github.com/Victor-Ribeiro-Acosta/Bootcamp-Azure-AI-Fundamentals-Mineracao-de-Conhecimento/blob/main/Passos/21.png)

 - Nessa guia é possível buscar informações nos arquivos filtrando eles pelo índice criado
 - Nele podemos adicionar pesquisa por informações por meio de informações json, o resultado da procura nos documentos é retornado abaixo
![](https://github.com/Victor-Ribeiro-Acosta/Bootcamp-Azure-AI-Fundamentals-Mineracao-de-Conhecimento/blob/main/Passos/22.png)

