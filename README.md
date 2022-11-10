# avv-jenkins
#! /bin/bash
alias user='wc -l /etc/passwd'
for i in user
do
cat | awk -F':' '{print i++ ".\n"$1, "Username: "$1"\nPassword: "$2"\nUser ID(UID): "$3"\nGroup ID(GID): "$4"\nUser ID Info: "$5"\nHome Directory: "$6"\ncommand/shell: "$7"\n"}'
done < /etc/passwd
this my chnage i made
