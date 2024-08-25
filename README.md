# Colinha de Linux / WSL / Docker 

## 1 - WSL => Uma tecnologia para rodar linux dentro do windows sem Máquina Virtual
[Doc Oficial] (https://learn.microsoft.com/pt-br/windows/wsl/about)

Você acessa ele a partir do CMD ou do Powershell do windows. Todos os comandos dele começam com wsl.

### Comandos WSL:
- listar as "imagens" (distros) WSL instaladas
`wsl -l -v`

- listar as "imagens" disponíveis para instalar (todas elas disponíveis nos servidores da microsoft)
`wsl --list --online` - é tipo a "lojinha" do WSL

- Verificar se o WSL está instalado e qual a versão:
`wsl -v` ==> Assegure-se de que a versão do WSL 2 ou maior esteja instalada porque a 1 é um lixão que não serve pra nada

- instalar uma imagem escolhida
`wsl --install -d <NomeDaDistribuição>` Exemplo: `wsl --install -d Ubuntu`

- entrar em uma instalação do linux pelo WSL
`wsl -d <NomeDaDistribuição>` Exemplo: `wsl -d Ubuntu`

- Definir uma distribuição padrão
`wsl --set-default <NomeDaDistribuição>` Exemplo: `wsl --set-default Debian`



## 2 - Docker => Containers leves que rodam no linux
- precisa de linux para funcionar, não roda direto no windows. 
- Também não é uma máquina virtual, 
- ele cria divisões nos processos e recursos do linux para os programas "pensarem" que estão rodando em uma máquina virtual. 

Ou seja, ele funciona isolando processos, mas rodando em cima de um sistema operacional e kernel já existente


- [Explicação breve](https://www.alura.com.br/artigos/comecando-com-docker) do que é docker
- [Video](https://youtu.be/85k8se4Zo70) explicando como docker funciona nos bastidores
- [guia fácil](https://www.dio.me/articles/primeiros-passos-com-o-docker-um-guia-facil) 
- [post do red hat](https://www.redhat.com/pt-br/topics/containers/what-is-docker) sobre docker


### Comandos de docker
- A ser realizados dentro de um shell(*) linux em um pc com linux instalado, ou no WSL, ou em uma VM com linux

- Verificar a versão do docker (e se ele está instalado)
`docker -v `


## 3 - Docker Desktop => uma gambiarra para rodar o docker no windows
- ele instala em cima do WSL se o pc tiver suporte 
- ou instala uma máquina virtual se o pc não tiver suporte a WSL (aí sim estamos dentro de máquinas virtuais)


## 10 - Referências e utilidades
- como deixar o seu powershell customizado e chavoso: [Oh My Posh](https://ohmyposh.dev/) - siga os tutoriais de instalação e configuração
- como deixar o seu zsh customizado e chavoso: [Oh My ZSH!](https://ohmyz.sh/) - siga os passos e instale
- tem pra bash também mas só uso bash quando sou obrigado [Oh My BASH!](https://ohmybash.nntoan.com/)
- (*) shell? Não shabe o que é shell? Shai de caja e olha pra shima que voshê vê. 