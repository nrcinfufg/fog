# FOG Project - Manual de Uso

Este manual fornece instruções detalhadas para utilizar o FOG Project, incluindo como registrar um novo host, instalar Snapins (somente para Windows), e gerenciar tasks e imagens.

## Índice

1. [Registrar um Novo Host](#registrar-um-novo-host)
2. [Instalação de Snapins (Somente Windows)](#instalação-de-snapins-somente-windows)
3. [Gerenciamento de Tasks](#gerenciamento-de-tasks)
4. [Gerenciamento de Imagens](#gerenciamento-de-imagens)

---

## Registrar um Novo Host

Para registrar um novo host no FOG, siga os passos abaixo:

1. **Acesse a Interface Web do FOG:**
   - Entre no painel de administração do FOG através do seu navegador digitando o IP do servidor no seguinte formato: xxx.xxx.xxx.xxx/fog.

2. **Navegue para a Seção de Hosts:**
   - No menu principal, vá para `Hosts` e clique em `List All Hosts`.

3. **Adicione um Novo Host:**
   - Para adicionar um novo Host que nao esteja cadastrado é necessário realizar o processo fisicamente na máquina em que se deseja registrar.
   - Inicialize a maquina pela rede (Servidor IPXE) digitando o IP do servidor FOG.
   - Clique em `Quick Registration and Inventory`.
   - Aguarde para que o processo de registro seja concluído.
   - Após a conclusão o Host estará adicionado, e poderá ser visualizado no menu de hosts do servidor Web.

## Instalação de Snapins (Somente Windows)

Snapins são pacotes de software que podem ser distribuídos para hosts Windows através do FOG. Para instalar Snapins, siga os passos abaixo:

> **Nota:** É preciso realizar a instalação do Fog Client para realizar o deploy do snapin pela rede. O passo a passo para a instalação do Fog Client está presente no seguinte link: 
[Instalação Fog Client](https://docs.fogproject.org/en/latest/installation/client/install-fog-client/?h=client#fog-client-silent-installation)

1. **Navegue para a Seção de Snapins:**
   - No menu principal, vá para `Snapins` e clique em `Create New Snapin`.

2. **Criar um Novo Snapin:**
   - Preencha os detalhes necessários, como o nome do Snapin e selecione o arquivo para upload.
   - Configure as opções de execução, como comandos adicionais se necessário.

3. **Deploy do Snapin:**
   - Vá para `Hosts` e selecione o host desejado.
   - No perfil do host, vá para a aba `Basic Tasks`.
   - Na aba `Basic Tasks` vá para `Advanced`
   - Dentro de `Advanced` procure por `Single Snapin`
   - Agora selecione o `Snapin` desejado e clique em `Task`

> **Nota:** Snapins são suportados apenas em sistemas Windows.

## Gerenciamento de Tasks
Tasks são ações que podem ser atribuídas a um ou mais hosts. Para gerenciar tasks, siga os passos:

1. **Gerenciar Tasks:**
   - No menu principal, vá para `Tasks`.
   - Neste menu, você poderá observar todas as tasks ativas, e as que estão em fila para execução.

## Gerenciamento de Imagens

Imagens são cópias de sistemas operacionais que podem ser implantadas em hosts. Para gerenciar imagens:

1. **Criar uma Nova Imagem:**
   - Vá para `Images` no menu principal e clique em `Create New Image`.

2. **Preencher os Detalhes da Imagem:**
   - Nomeie a imagem e selecione o tipo de sistema de arquivos.
   - Configure outras opções como desejado.

3. **Capturar ou Deploy de Imagem:**
   - Para capturar uma imagem de um host, vá para `Tasks`, selecione `Capture` e escolha o host.
   - Para deploy de uma imagem, selecione `Deploy Image` em `Tasks` --> `List All Hosts` e escolha a imagem e o host.

---

Para mais informações, consulte a [documentação oficial do FOG Project](https://docs.fogproject.org/).

