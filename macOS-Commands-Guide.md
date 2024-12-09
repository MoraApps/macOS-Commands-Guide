# Important Commands for macOS:


## Comandos Básicos do Terminal:


pwd
> Exibe o caminho do diretório atual.

ls
>  Lista os arquivos e diretórios no diretório atual.

ls -a
> Lista todos os arquivos, incluindo os ocultos (que começam com um ponto).

ls -l
> Lista os arquivos em formato longo (com permissões, proprietário, tamanho e data).

ls -lh
> Lista os arquivos com detalhes e tamanhos de arquivo em formato legível (ex: KB, MB).

ls -R
> Lista os arquivos de forma recursiva, ou seja, incluindo os arquivos dentro de subdiretórios.

cd
> Muda o diretório atual.

cd ..
> Vai para o diretório acima (um nível superior).

cd ~
> Vai para o diretório home do usuário.

cd -
> Volta para o diretório anterior.

mkdir
> Cria um novo diretório.

rm
> Remove um arquivo.

rm -r
> Remove um diretório e seu conteúdo.

rm -rf
> Remove um diretório e seu conteúdo de forma forçada (sem pedir confirmação).

touch
> Cria um novo arquivo vazio ou atualiza a data de modificação de um arquivo existente.

cat
> Exibe o conteúdo de um arquivo.

head
> Exibe as primeiras 10 linhas de um arquivo.

tail
> Exibe as últimas 10 linhas de um arquivo.

tail -f
> Exibe as últimas linhas de um arquivo e continua mostrando à medida que o arquivo é alterado (ideal para logs).

clear
> Limpa o terminal.

history
> Exibe o histórico de comandos usados no terminal.

exit
> Sai do terminal ou encerra a sessão.


## Comandos Git Essenciais:


git init
> Inicializa um novo repositório Git no diretório atual.

git status
> Mostra o status do repositório (quais arquivos foram modificados, adicionados, etc.).

git add .
> Adiciona todos os arquivos modificados ao repositório para o próximo commit.

git commit -m "Mensagem"
> Cria um commit com a mensagem fornecida.

git log
> Mostra o histórico de commits no repositório.

git remote add origin [url]
> Conecta o repositório local a um repositório remoto.

git push -u origin master
> Envia os commits locais para o repositório remoto.

git pull origin master
> Baixa as últimas mudanças do repositório remoto.

git clone [url]
> Clona um repositório remoto para o seu diretório local.

git branch
> Lista todas as branches no repositório.

git checkout nome_da_branch
> Muda para a branch especificada.

git merge nome_da_branch
> Mescla a branch especificada com a branch atual.


## Comandos Modernos e Úteis:


tree
> Exibe a estrutura de diretórios em forma de árvore (visualização hierárquica).

htop
> Exibe uma interface interativa para monitoramento do uso de recursos do sistema (como CPU, memória, processos).

df
> Exibe o uso do espaço em disco do sistema de arquivos.

du
> Exibe o uso de espaço de um diretório.

find
> Pesquisa por arquivos e diretórios em um diretório.

grep
> Pesquisa por um padrão dentro de arquivos.

ps
> Exibe os processos em execução no sistema.

kill
> Encerra um processo pelo seu ID (PID). “(Process ID). Esse ID é atribuído automaticamente pelo sistema quando o processo é iniciado.”

killall
> Encerra todos os processos com o nome especificado.

alias
> Cria um atalho para comandos mais longos.

unalias
> Remove um atalho criado com alias.

chmod
> Modifica as permissões de um arquivo ou diretório.

chown
> Altera o proprietário de um arquivo ou diretório.

scp
> Copia arquivos entre sistemas via SSH.

rsync
> Sincroniza arquivos e diretórios entre sistemas ou pastas locais.

curl
> Faz requisições HTTP e exibe a resposta.

wget
> Baixa arquivos da internet.

tar
> Comprime ou descomprime arquivos (arquivos tar).

zip
> Comprime arquivos em formato .zip.

unzip
> Descomprime arquivos .zip.

sudo
> Executa um comando como superusuário (root).


# Important Homebrew Commands:


## Instalação e Atualização:


> Instalar o Homebrew (caso ainda não tenha): 
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

brew update
> Atualizar Homebrew para a versão mais recente.

brew upgrade
> Atualizar todos os pacotes instalados.

brew cleanup
> Remover versões antigas de pacotes desnecessários.

brew update && brew upgrade
> Uso de comandos combinados, ex.# Uso de Comandos Combinados: brew update && brew upgrade.  
> O comando `brew update` verifica e atualiza o Homebrew para a versão mais recente. 
> O operador `&&` garante que o próximo comando (`brew upgrade`) seja executado apenas se o anterior foi bem-sucedido.  
> Isso é útil para atualizar o Homebrew e todos os pacotes instalados de forma eficiente.


## Pesquisa de Pacotes:


brew search nome_do_pacote
> Pesquisar um pacote disponível no Homebrew.

brew info nome_do_pacote
> Mostrar informações detalhadas sobre um pacote específico.


## Instalação e Remoção de Pacotes:


brew install nome_do_pacote
> Instalar um pacote específico.

brew reinstall nome_do_pacote
> Reinstalar um pacote já instalado.

brew uninstall nome_do_pacote
> Remover um pacote instalado.


## Gerenciamento de Serviços:


brew services list
> Listar serviços disponíveis instalados pelo Homebrew.

brew services start nome_do_pacote
> Iniciar um serviço gerenciado pelo Homebrew.

brew services stop nome_do_pacote
> Parar um serviço gerenciado pelo Homebrew.

brew services restart nome_do_pacote
> Reiniciar um serviço gerenciado pelo Homebrew.


## Diagnóstico:


brew doctor
> Verificar se o Homebrew está configurado corretamente.

brew list nome_do_pacote
> Mostrar o caminho de instalação de um pacote.

brew list
> Listar todos os pacotes instalados:

brew deps nome_do_pacote
> Verificar dependências de um pacote específico.


## Gestão de Casks (Aplicativos GUI e Pacotes Grandes):


brew install --cask nome_do_app
> Instalar um aplicativo usando um cask.

brew upgrade --cask
> Atualizar aplicativos instalados por casks.

brew uninstall --cask nome_do_app
> Remover um aplicativo instalado por cask.

brew search --cask nome_do_app
> Pesquisar aplicativos disponíveis para cask.

## Exemplo de Fluxo Completo

brew search git
> Pesquisar um pacote.

brew install git
> Instalar o pacote.

brew list
> Verificar a instalação.
