# Lista de Comandos VIM
*Modo Insert*
- i = Modo INSERT
- esc = Voltar para o modo normal
- :w = Salvar
- :q = Sair
- :wq = Salvar e sair
- :%s/substituido/substituir/g[global]c[pergunta se quer alterar] = 
- :vs + caminho do arquivo = divide a tela na vertical
- :sp + caminho do arquivo = divide a tela na horizontal
- [crtl] + ww = altera a tela divida
- vim .vimrc = Entra no arquivo
*Modo Normal*
 - [crtl] + w + seta = navega entre os splits
Setas:
  - L = Direita
  - J = Baixo
  - k = Cima
  - H = Esquerda
  - w = caminha palavra por palavra
  - Numero + [Letra das Setas] = Numero de vezes que a seta vai se repetir
  - u = Remove a ultima ação feita pelo usuario
  - [crtl] + R = Avança a ultima ação removida
  - o = entra em modo insert na linha abaixo onde você parou no modo normal 
  -[shift] + o = entra em modo insert na linha acima onde parou 
  - y = Copia
  - p = Cola
  - x = remove
  - == = Identação
  - gg = sobe para primeira linha do arquivo
  - [shift] + g = desce para a ultima linha do arquivo
  - [shift] + a = Vai para o final da linha e insere
  - dd = deleta a linha
Pesquisa:
 - / = Pesquisar
 - n = Proximo resultado
 - [shift] + n = Volta para o resulta anterior


*Modo Visual*
 - [shift] + v = Modo Visual
 - Setas = seleciona mais linhas

*Modo Bloco*
  - [crtl] + v = Entra no modo Bloco



# Arquivo de Configurações VIM
- :echo $HOME = Descobrir onde o VIM esta instalado
- colorscheme industry
- set tabstop=2 = Identação do TAB
- set shiftwidth=2 = Movimentação do TAB
- filetype plugin indent on = adiciona extensao de arquivos (ex: .html .js .php)
- sintax on = colocar cores de sintax
- set backspace=2 = autoriza deletar usando backspace
- set number = numera as linhas
- set realativenumber = fazer calculo das distancia das linhas
- set incsearch = busca incremental - feedback enquanto faço buscas
- set hlsearch =  Destaque de buscas em fechamento de tags


Pathogen - Gerenciador de plugins do VIM
Criar pasta .vim
Criar pasta autoload dentro da pasta .vim (pasta que carrega as coisas ao iniciar )
Criar pasta bundle dentro da pasta .vim (pasta bundle carrega as coisas que o pathogen carrega)

curl -LSso ~/.vim/autoload/pathogen.vim https://tpo.pe/pathogen.vim

Abra o arquivo vimrc e insira esse codigo no inicio do arquivo 
- execute pathogen#infect()

NERDTree
git clone https://github.com/scrooloose/nerdtree.git ~/.vim/bundle/nerdtree

Iniciar o plugin
- :NERDTree
s = abrir com splits
:q = Fechar o NERDTree 

*INSERIR NOVOS TEMAS*
Tomorrow theme
Navegar até a pasta .vim e criar uma pasta chamada colors
baixa o arquivo do tema escolhido e coloca no arquivo colors
Entra no .vimrc e coloque "colorscheme tomorrow"
