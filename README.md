# Projeto de Validação de APIs da Marvel usando Postman [![N|Solid](https://voyager.postman.com/logo/postman-logo-icon-orange.svg)](https://www.postman.com/product/what-is-postman/)

> I guess one person can make a difference. </p>
> Stan Lee

Este projeto tem como objetivo realizar a validação de dois serviços da API da Marvel usando a ferramenta Postman. As validações incluem verificação do status code, status code name, timeout, teste de contrato e validação do response.

## Serviços da Marvel

**Busca de Personagem**
Endpoint: **/characters/<character_id>**
Descrição: Este serviço retorna um personagem por ID.
**Histórias**
Endpoint: **/stories**
Descrição: Este serviço retorna uma lista de histórias da Marvel.

## Pré-requisitos

Antes de começar, verifique se você possui o seguinte:
- [Postman] instalado em seu computador. **
- Uma chave de API válida para autenticar no ambiente Marvel. Você pode obter uma chave gratuita em developer.marvel.com.

** Outras possibilidade é acessando o projeto direto por este [link].

[link]: <https://elements.getpostman.com/redirect?entityId=5114087-f3c706b8-d249-4472-937d-70b5d6e44d26&entityType=collection>

[postman]: <https://www.postman.com/downloads/>

## Configuração do Ambiente

Siga as etapas abaixo para configurar seu ambiente no Postman:

- Clone ou baixe o projeto do Postman contendo a collection e o environment. Você pode encontrar ele [aqui].
- Abra o Postman e importe os arquivos (colletion e environment).
- Altere os valores das variáveis de ambiete **api_public_key** e **api_private_key**.

[aqui]: <https://github.com/juliocfp/mottu-api>

## Testes de Validação

A collection contém dois blocos de teste que podem ser executados para validar os serviços da Marvel. Os testes são descritos a seguir:

- Verifica o status code da resposta para garantir que seja 200 (OK).
- Verifica o status code name para garantir que seja "OK".
- Define um timeout para as requisições.
- Testa o contrato da resposta para garantir que esteja correto.
- Valida o response da API.

### Cenários de Exceção

É importante considerar cenários de exceção para garantir a robustez do projeto. Abaixo estão alguns cenários que foram adicionados ao teste:

- Usuário não autorizado.
- Personagem não encontrado.
- Parâmetros invárlidos.
- Limites de borda de parâmetros.

## Executando os Testes

Para executar os testes das requisições da collection, siga as etapas abaixo:

- Com o projeto aberto no Postman, clique nas opções de sua collection e selecione **Run collection**.
- O **Runner** será aberto para seleção de requisições que deseja ser testada.
- Selecione as requisições desejadas e clique em **Run**.

Os testes serão executados para todas requisições selecionadas, exibindo o resultado de cada teste por requisição. É possível também exportar um relatório dos testes.

## Conclusão

Este projeto de validação no Postman permite verificar o status code, status code name, timeout, teste de contrato e validação do response para dois serviços da API da Marvel. Essas validações ajudam a garantir a integridade e o correto funcionamento dos serviços fornecidos pela Marvel.
