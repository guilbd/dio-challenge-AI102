
# Microsoft Certification Challenge #1 AI 102

## Bootcamp da DIO: Tradução de Artigos com Azure Translator

Este projeto faz parte do desafio "Microsoft Certification Challenge #1 AI 102" do Bootcamp da DIO. Nele, desenvolvemos uma aplicação que utiliza o serviço **Azure Translator** para realizar a tradução de artigos a partir de URLs fornecidas pelo usuário. O projeto demonstra como usar a API de tradução da Microsoft para extrair, traduzir e formatar textos em Markdown.

### Funcionalidades
- Extração de texto de páginas web utilizando **BeautifulSoup**.
- Tradução de texto usando a **API Azure Translator**.
- Geração do resultado em formato Markdown para fácil visualização.

### Tecnologias Utilizadas
- **Python**: Linguagem de programação principal.
- **Requests**: Para realizar requisições HTTP.
- **BeautifulSoup4**: Para realizar o parsing e extração de texto de páginas HTML.
- **Azure Translator API**: Serviço de tradução utilizado para traduzir o texto extraído.

### Como Utilizar
1. **Pré-requisitos**:
   - Python 3.11 ou superior.
   - Biblioteca `requests` e `beautifulsoup4`. Instale-as utilizando:
     ```sh
     pip install requests beautifulsoup4
     ```
   - Uma chave válida para o **Azure Translator API** e a região do serviço configurada.

2. **Configuração**:
   - No código, substitua `"SUA_CHAVE_DO_AZURE"` pela sua chave da API do Azure.
   - Ajuste o `endpoint` e `regiao` conforme suas configurações do Azure.

3. **Execução**:
   - Para traduzir um artigo, forneça a URL desejada na variável `url_artigo`.
   - Execute o script:
     ```sh
     python nome_do_script.py
     ```
   - O artigo traduzido será exibido no terminal em formato Markdown.

### Estrutura do Código
- **extrair_texto_de_url(url)**: Extrai o texto de uma página web removendo scripts e estilos desnecessários.
- **traduzir_texto_azure(texto, idioma_destino, chave_api, endpoint, regiao)**: Faz a tradução do texto extraído usando o Azure Translator.
- **translate_article(url)**: Função principal que orquestra a extração e tradução do artigo.

### Exemplo de Uso
```python
    url_artigo = "https://example.com/artigo-exemplo"  # URL do artigo a ser traduzido
    translate_article(url_artigo)
```

### Licença
Este projeto está sujeito às políticas de licença estabelecidas pelo Bootcamp da DIO.

### Observações
- Certifique-se de ter uma conexão de internet estável ao usar a API do Azure e ao realizar o scraping de páginas web.
- Verifique a política de acesso de cada site antes de fazer a extração de conteúdo.

### Contribuições
Contribuições são bem-vindas! Sinta-se à vontade para abrir uma *issue* ou um *pull request* para melhorias e novas funcionalidades.

### Sobre o Bootcamp
Este projeto faz parte do Bootcamp da DIO, em colaboração com a **Microsoft**, focado em habilidades práticas relacionadas a **Inteligência Artificial** e **tradução automática**.
