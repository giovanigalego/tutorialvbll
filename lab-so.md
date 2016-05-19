###TUTORIAL

* Saiba seu diretório atual usando.  
  `pwd`  

* Crie os diretórios: **mack**, **trabalho**, **mack/textos**.  
  `mkdir mack`  
  `mkdir trabalho`    
  `mkdir mack/textos` 
  
  
* Entre no diretório: mack  
  `cd mack`  
  
  
* Transfira o conteúdo de um arquivo para o outro, mas neste caso crie um arquivo "aberto" que será preenchido quando apertar ctrl+D  
 `cat > numeros.txt`  
 `10`   
 `100`    
 `50`    
 `25`    
 `1`    
 `2`    
 `^D` 
 
* Faça a cópia do conteúdo do arquivo **numeros.txt** para **numeros1.txt** e **numeros2.txt**  
  `cat numeros.txt >> numeros1.txt`  
  `cat numeros.txt >> numeros2.txt`  
  
* Copie todos os arquivos que possue a extensão **txt** para o diretório **trabalho**    
 `cp *.txt ../trabalho`  
 
* Liste de forma detalhada todos os arquivos de um diretório  
  `ls -l`  

* Troque as permissões do arquivo **numero.txt** para **-rwxr-xr-x**  
  `chmod 755 numero.txt`  
  
* Troque as permissões do arquivo **numero.txt** para **-rw-r--r--**  
  `chmod 644 numero.txt`  
  
* Copie o conteúdo do diretório **mack** de forma recursiva, para a pasta *trabalho_feito** que deve ser criada na raiz  
  `cp -r ../mack ~/trabalho_feito`  
  
* Remova todos os arquivos com extensão **txt**  
 `rm *.txt`  
 
* Remova de forma recursiva o diretório **mack**  
  `rm -r ../mack`  
  
* Entre na pasta **trabalho_feito** que está criada dentro da home  
  `cd ~/trabalho_feito`  
  
* Troque o nome do arquivo **numeros.txt** para **sequencia.txt**  
 `mv numeros.txt sequencia.txt`  
 
* Liste os arquivos da pasta **bin** para o arquivo **listabin.txt**  
  `ls /bin > listabin.txt`  
  
* Use o comando `rmdir` para efetuar a remoção de uma pasta vazia  

* Renomeie a pasta **trabalho_feito** para **lab_unip_01**
  `mv ../trabalho_feito ../lab_unip_01`  
  
* Faça a criação da pasta **info_system** na home, após feito isso crie a pasta **rede** no diretório **~/info_system, por fim,  
  liste o resultado do comando **ifconfig** para o arquivo **interface_maquina.txt**  
  `mkdir ~/info_system`  
  `mkdir ~/info_system/rede`  
  `ifconfig > ~/info_system/rede/interface_maquina.txt`  
  
  
  
  ###Lab-so .sh  
```  
pwd
mkdir mack
mkdir trabalho
mkdir mack/textos
cd mack
echo Digite 10, 100, 50, 25, 1, 2 e pressione CTRL + D
cat > numeros.txt
cat numeros.txt >> numeros1.txt
cat numeros.txt >> numeros2.txt
cp *.txt ../trabalho
ls -l
chmod 755 numeros.txt
chmod 644 numeros.txt
cp -r ../mack ~/trabalho_feito
rm *.txt
rm -r ../mack
cd ~/trabalho_feito
mv numeros.txt sequencia.txt
ls /bin > listabin.txt
rmdir
mv ../trabalho_feito ../lab_unip_01
mkdir ~/info_system
mkdir ~/info_system/rede
ifconfig > ~/info_system/rede/interface_maquina.txt  
```
  
  
  




















 
