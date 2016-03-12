<h2>Criando uma máquina virtual com SliTaz no VirtualBox </h2>

Primeiramente, vamos fazer download do que será necessário:

VirtualBox (baixe no site oficial): https://www.virtualbox.org/wiki/Downloads </br>
SliTaz (baixe no site oficial): http://www.slitaz.org/pt/get 

Faça uma instalação padrão NNF (Next, next, finish)

Durante a instalação, poderá haver interrupção da conexão para a criação dos drivers de rede do VB assim,
criando a máquina virtual.

Para criação da máquina virtual, usaremos as seguintes configurações: </br>
Tipo: Linux </br>
Versão: Other Linux (32-bit)</br>
RAM: 512MB</br>
HD: 60GB</br>

Depois de abrir o VirtualBox, clique em "Novo" e preencha as "caixas" de acordo com as configurações acima. Caso haja algum item não especificado, preencha como quiser.

<h3>Iniciando a máquina virtual/SliTaz: </h3>

Selecione a máquina virtual já criada e clique em "Iniciar"
Como ainda não temos nenhum sistema operacional ainda o VirtualBox irá pedir para que selecione um. Selecione a ISO do SliTaz e selecione
logo após, clique em "SliTaz Live" ou aguarde o boot automático. Após iniciar o sistema, selecione o idioma (en_US) e o teclado (br-abnt2)

É necessário iniciar o sistema em inglês, para não haver nenhum problema na instalação.

<h3>Criando partição:</h3>

Após iniciar o sistema, clique em Applications -> System Tools -> GParted
Irá aparecer uma janela solicitando autenticação, use a senha padrão que é root. 
Na parte de cima da janela que irá abrir, selecione Device -> Create Partition Table... e depois Apply
Logo após, clique na partição "unallocated", "New" e "Add"
Para finalizar, clique em "Apply" e depois "Apply" novamente
Quando o carregar, clique em "Close" e feche o "GParted"

<h3>Instalando o SliTaz no HD:</h3>

No canto superior esquerdo da área de trabalho no botão vermelho com uma chave inglesa. Clique nele e
irá aparecer uma solicitação de autenticação, o usuário padrão é root e a senha também (igual a anterior)
Irá abrir uma nova janela e na parte de cima, selecione "Install -> Install SliTaz"
Logo após selecione "Continue Installation"
Em "Hard Disk Drive -> Install SliTaz to partition" selecione /dev/hda1/ (ou a única partição disponível)

Caso queira alterar o nome do computador, altere o "Set Hostname to". Para alterar a senha do Root, altere também o  "Root passwd". Caso queira alterar o nome e senha do usuário padrão, altere "User login", "User passwd" e a confirmação "Confirm password"
Desça a barra de rolagem, marque "Install Grub bootloader", selecione "Proceed to SliTaz installation", após todos os passos dê "Ok" e aguarde a instalação ser concluída
Por fim, clique em "Installation complete. You can now restart (reboot)"

<h3>Iniciando a máquina virtual com SliTaz localmente:</h3>

Após a instalação, a máquina virtual será reiniciada e irá mostrar a janela de seleção de idioma

Dessa vez, você já pode selecionar pt_BR como idioma
Irá aparecer a janela de autenticação de usuário. Autentique com os dados informados na hora da instalação e estará tudo pronto.
