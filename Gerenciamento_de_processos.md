
Um pouco sobre o comando ps aux e suas colunas

USER: Esta é uma das informações mais intuitivas do comando, ela é a coluna que contém o usuário que executou certo processo.
PID :  Essa coluna contém os números de identificação do processo, PID (Process ID). Alguns dizem que essa é uma das informações mais importantes desse comando, porque quando queremos “matar” esse processo utilizamos seu ID.
%CPU : Essa coluna contém um dado muito interessante, ela é a coluna onde mostra o quanto o processo está utilizando da CPU, ela utiliza um formato como “XX.X” para poder exibir seu valor. Há um cálculo para descobrir o quanto é usado, esse cálculo é feito pelo tempo de uso da cpu divido por tempo do processo sendo executado (cputime / realtime ratio)
%MEM: Essa coluna também consiste em uma informação dos nossos hardwares, ela contém a informação da porcentagem que o processo está alocado em nossa memória física 
VSZ : essa coluna não é nada intuitiva com o nome, ela mostra as informação do tamanho da memória virtual do processo em Kib (Kilo bytes) e VSZ significa “Virtual memory size”. 
RSS: (Resident Set Size) mostra o quanto estamos usando da RAM do tempo da saída de dado do comando, ele também consiste em mostrar toda a pilha de memória que está alocada na memória física.

STAT : (Process State Codes) são os estados que aquele processo está, existe uma lista desses estados:
D -  Sono ininterrupto 
R - Em execução ou executável (Isto na fila de execuções)
S – Sono Interrompível
T – Parado
W – Paginação (mas ele foi descontinuado desde o kernel com versão 2.6)
X – Morto 
Z – Extinto (Encerrado)

Caso o formato seja em BSD:
< - Alta prioridade
N – Baixa prioridade
L – Contém páginas fechadas na memória
s – Sessão principal
l – Multi-threaded
+ - está no grupo de processos 

E quais os estados possiveis de um processo no sistema operacional Linux?

1.	Process ID (PID) ou Identificação do processo
2.	O ID do usuário que está executando determinado processo
3.	O ParentID 
4.	Variáveis de ambiente
5.	Diretório do trabalho
6.	Temporizadores
7.	Finalizado

