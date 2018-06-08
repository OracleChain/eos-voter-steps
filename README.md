doushadeMacBook-Pro:eosio.system cl$ cleos create key
Private key: 5HyzEzK6mPYnKwhiuSGMUbtSiVwP5rjXYf5EWhhkgiZsWch24DC
Public key: EOS89AcJYCj1P7KYnx756eT7vbnrEqucGkLijaPUEkc3Jn2krpsBJ
doushadeMacBook-Pro:eosio.system cl$ cleos create key
Private key: 5JpUtwUapGnqCWnuhQubwj9iJ1duJtQNaBWfo3FjRCE3jvfCc5w
Public key: EOS5c2fvwkzAcBK57irykyeGd8cuhag43U77peqYzMU71JKvmf91R


预创建账户:
cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/ create account eosio  eosio.bpay     EOS89AcJYCj1P7KYnx756eT7vbnrEqucGkLijaPUEkc3Jn2krpsBJ EOS5c2fvwkzAcBK57irykyeGd8cuhag43U77peqYzMU71JKvmf91R
cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/ create account eosio  eosio.msig     EOS89AcJYCj1P7KYnx756eT7vbnrEqucGkLijaPUEkc3Jn2krpsBJ EOS5c2fvwkzAcBK57irykyeGd8cuhag43U77peqYzMU71JKvmf91R
cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/ create account eosio  eosio.names     EOS89AcJYCj1P7KYnx756eT7vbnrEqucGkLijaPUEkc3Jn2krpsBJ EOS5c2fvwkzAcBK57irykyeGd8cuhag43U77peqYzMU71JKvmf91R
cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/ create account eosio  eosio.ram     EOS89AcJYCj1P7KYnx756eT7vbnrEqucGkLijaPUEkc3Jn2krpsBJ EOS5c2fvwkzAcBK57irykyeGd8cuhag43U77peqYzMU71JKvmf91R
cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/ create account eosio  eosio.ramfee     EOS89AcJYCj1P7KYnx756eT7vbnrEqucGkLijaPUEkc3Jn2krpsBJ EOS5c2fvwkzAcBK57irykyeGd8cuhag43U77peqYzMU71JKvmf91R
cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/ create account eosio  eosio.saving     EOS89AcJYCj1P7KYnx756eT7vbnrEqucGkLijaPUEkc3Jn2krpsBJ EOS5c2fvwkzAcBK57irykyeGd8cuhag43U77peqYzMU71JKvmf91R
cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/ create account eosio  eosio.stake     EOS89AcJYCj1P7KYnx756eT7vbnrEqucGkLijaPUEkc3Jn2krpsBJ EOS5c2fvwkzAcBK57irykyeGd8cuhag43U77peqYzMU71JKvmf91R
cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/ create account eosio  eosio.token     EOS89AcJYCj1P7KYnx756eT7vbnrEqucGkLijaPUEkc3Jn2krpsBJ EOS5c2fvwkzAcBK57irykyeGd8cuhag43U77peqYzMU71JKvmf91R
cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/ create account eosio  eosio.vpay EOS89AcJYCj1P7KYnx756eT7vbnrEqucGkLijaPUEkc3Jn2krpsBJ EOS5c2fvwkzAcBK57irykyeGd8cuhag43U77peqYzMU71JKvmf91R

cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/ create account eosio eosio.token EOS89AcJYCj1P7KYnx756eT7vbnrEqucGkLijaPUEkc3Jn2krpsBJ EOS5c2fvwkzAcBK57irykyeGd8cuhag43U77peqYzMU71JKvmf91R



cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/ create account --stake-net "10 EOS" --stake-cpu "10 EOS" --buy-ram "10 EOS" eosio producera EOS89AcJYCj1P7KYnx756eT7vbnrEqucGkLijaPUEkc3Jn2krpsBJ EOS5c2fvwkzAcBK57irykyeGd8cuhag43U77peqYzMU71JKvmf91R 


cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/ wallet import 5JpUtwUapGnqCWnuhQubwj9iJ1duJtQNaBWfo3FjRCE3jvfCc5w

cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/ set contract eosio ./ eosio.system.wast eosio.system.abi -p eosio


cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/ set contract eosio.token ./ eosio.token.wast eosio.token.abi -p eosio.token

cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/ set contract eosio.msig ./ eosio.msig.wast eosio.msig.abi -p eosio.msig


cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/ push action eosio.token create '{"issuer":"eosio" "maximum_supply":"10000000.0000 SYS"}' -p eosio.token
cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/ push action eosio.token create [ "eosio" "10000000.0000 EOS"] -p eosio.token


cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/ push action eosio.token issue [ "votera" "1000000.0000 SYS" "memo" ] -p eosio
cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/ push action eosio.token issue [ "votera" "1000000.0000 EOS" "memo" ] -p eosio

cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/ push action eosio.token issue '[ "aaaaaavotera" "1000000.0000 SYS" "memo" ]' -p eosio
cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/ push action eosio.token issue [ "aaaaaavotera" "1000000.0000 EOS" "memo" ] -p eosio

cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/ system regproducer producera EOS5c2fvwkzAcBK57irykyeGd8cuhag43U77peqYzMU71JKvmf91R

cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/  system voteproducer approve aaaaaavotera producera

cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/  system buyram eosio votera "100 SYS"

 cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/   system newaccount eosio producera EOS89AcJYCj1P7KYnx756eT7vbnrEqucGkLijaPUEkc3Jn2krpsBJ EOS5c2fvwkzAcBK57irykyeGd8cuhag43U77peqYzMU71JKvmf91R --stake-net "10 SYS" --stake-cpu "10 SYS" --buy-ram "10 SYS"  -p eosio

 cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/   system newaccount eosio aaaaaavotera EOS89AcJYCj1P7KYnx756eT7vbnrEqucGkLijaPUEkc3Jn2krpsBJ EOS5c2fvwkzAcBK57irykyeGd8cuhag43U77peqYzMU71JKvmf91R --stake-net "10 SYS" --stake-cpu "10 SYS" --buy-ram "10 SYS"  -p eosio


 cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/    system regproxy aaaaaavotera

 cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/ get  currency balance eosio.token aaaaaavotera SYS

cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/  get table eosio eosio  voters 

cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/  system  voteproducer prods aaaaaavotera producera

cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/   system delegatebw aaaaaavotera aaaaaavotera "10 SYS" "10 SYS"

cleos -u http://127.0.0.1:8888/ --wallet-url http://127.0.0.1:8890/   system  listproducers


 grep -R --include=*.{hpp,cpp,h} "staked =" ./