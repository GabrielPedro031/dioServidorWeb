#ApacheBench-ab#

Banco apache autônomo - ferramenta de benchmarking do servidor Apache HTTP

##Instruções de construção##

Construir:
        $fazer
Limpar:
        $ limpar

##Uso##

#####Usa mais simples#####
       #ab -c 25 -n 100 
           
       As três opções são:
       * simultaneidade (-c 25)
       * número de solicitações (-n 100)
      

#####Usando com GnuPlot#####
       #ab -c 25 -n 100 -r -g out.dat .
       Use o template plot.p que vem com a fonte
       #gnuplot plot.p

       
######Usando com GnuPlot#####
       #ab -c 25 -n 100 -r -g out.dat 
       Use o template plot.p que vem com a fonte
       #gnuplot plot.p

       
####SINOPSE####
       ab [ -A auth-username:password ] [ -b windowssize ] [ -c simultaneidade ] [
       -C cookie-name=value ] [ -d ] [ -e arquivo csv ] [ -f protocol ] [ -g gnu‐
       plot-file ] [ -h ] [ -H custom-header ] [ -i ] [ -k ] [ -n request ] [
       -p POST-file ] [ -P proxy-auth-username:password ] [ -q ] [ -r ] [ -s ]
       [ -S ] [ -t timelimit ] [ -T content-type ] [ -u PUT-file ] [ -v ver‐
       bosity] [ -V ] [ -w ] [ -x <table>-attributes ] [ -X proxy[:port] ] [
       -y <tr>-attributes ] [ -z <td>-attributes ] [ -Z ciphersuite ]
       [http[s]://]hostname[:port]/path



####RESUMO####
       ab é uma ferramenta para benchmarking do seu Apache Hypertext Transfer Protocol
       (HTTP). Ele é projetado para lhe dar uma impressão de como o seu
       a instalação atual do Apache é executada. Isso mostra especialmente como
       muitas requisições por segundo sua instalação do Apache é capaz de atender
       ing.



####OPÇÕES####
       -Auth-username:password
              Forneça credenciais de autenticação BASIC ao servidor. O usuário-
              nome e senha são separados por um único : e enviados no
              fio codificado em base64. A string é enviada independentemente de
              o servidor precisa dele (ou seja, enviou uma autenticação 401
              precisava).
####fIM####