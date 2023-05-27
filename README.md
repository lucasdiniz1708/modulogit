Este modulo foi um inicio ao trabalho com repositório remoto e local ao git hub, nele fiz alguns testes de commits, push, pul e alguns testes com branchs.

Comandos utilizados: 



git init                                                       //Comando para iniciar o repositorio git localmente

git config --global user.name "lucasdiniz1708"                  //Configurações de Usuario                
git config --global user.email "lucasmoraes1708@gmail.com"
git config --global core.editor vscode
git config --list

git log                                                       //Lista de Commits realizados no repositorio local
git status -verifica se ha comits ou alterações               // Verifica o estado e indica quais arquivos precisam ser adicionados ou commitados
git add -A                                                     // Adiciona todas as mudanças, preparando-as para serem incluídas em um commit. 

git diff                                                        //mostra as alterações feitas antes de commitar         
git diff --name-only                                            //mostra apenas o nome do arquivo que foi alterado.
git diff nomedoarquivo                                          //mostra as alterações apenas naquele arquivo

git commit -m "Criando os arquivos principais"                
git commit -am ""                                               //Junção do add com o commit

git restore 

git reset --soft iddocommit                             //Remove o commit indicado sem perder as alterações na maquina local, mandando o HEAD para o commit anterior
git reset --mixed iddocommit                            // Semelhante ao soft mas remove também as alterações feitas no indice(ADD)
git reset --hard  iddocommit                            //Remove o commit, remove do indice e também remove da maquina local

git revert --no-edit 276ddc98ac8057ea8b66076c3e06df69ade6166a       // Refaz as alterações do commit mas mantém no historico salvo 

git branch                                        //Lista os branches na maquina local
git branch teste                                  //Cria um novo branch com nome teste
git branch -D teste                               //Deleta o branch local

git checkout teste                             //Muda o branch de master para teste 
git checkout HEAD -- nomedoarquivo            //Retorna a ultima alteração feita ( ultimo commit semelhante ao git reset )

git push origin master                      //Envia as alterações para o repositorio remoto
git push origin teste                       //Manda o branch teste para o repositorio remoto
git push origin :teste                     //Deleta o branch do repositorio remoto

git fetch 
git pull origin master                      //Puxa as informações do repositorio remoto ao local
git clone urldoprojeto                      //Puxa as informaçoes de um repositorio publico para o repositorio local

git remote -v                           //Verificação das configurações do repositório remoto antes de realizar operações de push ou pull
