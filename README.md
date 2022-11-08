# java10-2022b-lipesanfelice
java10-2022b-lipesanfelice created by GitHub Classroom

###Código escolhido: sharedaccount

##Processo:

#Deposita:
1* Thread carrega o valor do  saldo de memoria;
2* Thread faz a soma do saldo existente com o valor depositado;
3* Coloca o valor da soma no saldo;

#Retira:
1* Thread carrega o valor do  saldo de memoria;
2* Thread faz a subtração do saldo existente com o valor que foi retirado;
3* Coloca o valor da subtração no saldo;

#ThreadDeposita:
1* Realiza o deposito na conta;
2* Pega o valor total;
3* Realiza n depositos;

#ThreadRetira:
1* Realiza a retirada na conta;
2* Pega o valor total;
3* Realiza n retiradas;

#main:
Em suma, é dado um valor inicial e são realizadas retiradas e depositos e a cada execução ele mostra o saldo que tem e o saldo que deveria ter.

#Explicação do resultado incorreto:
Já que duas operações estavam sendo feitas em pararelo e com vários objetos sendo rodados ao mesmo tempo dependendo da situação a segunda operação pode carregar os valores da memória (1° passo) antes da primeira ter atualizar os valores (3° passo), então o resultado sairia diferente do esperado.

#Indo além:
Eu achei muito interressante o fato de ter muitas operações executando em paralelo e como apenas uma palavra pode fazer uma diferença tão grande no meio de um código tão extenso ou não.
Você encontrou algo interessante buscando algum material de apoio relacionado? Achei um conceito bem legal que é o de Deadlock "Condição em que uma thread bloqueia um recurso X e precisa de um recurso Y para finalizar. Contudo, o recurso Y também está bloqueado por outra thread, que aguarda pelo recurso X para executar seu processamento" eu achei interressante pq quando ouvi falar de programação concorrente nas aulas eu pensei "problemas resolvidos para tarefas em paralelo", mas tem muitos detalhas sórdidos que estou gostando de descobrir.

#Curiosidade:
Pokemon Go foi por muito tempo meu jogo preferido e eu não sabia (ou não lembrava) que ele tinha sido feito em java... adorei descobrir isso.
"Niantic Lab que desenvolveu o Jogo em parceria com a Nintendo já havia feito um jogo de realidade Aumentada (sim, realidade aumentada de verdade) com geolocalização em JAVA usando LibGDX. Este jogo é o Ingres Prime, que combina geolocalização, RA em uma missão entre Iluminados e Resistência para obtenção do poder da Matéria Exótica."
