
# Instalação do Ansible

Ansible é uma ferramenta para controle e gerenciamento de hosts.
O Ansible por padrão gerencia maquinas pelo protocolo SSH
Uma vez instalado, ele não irá criar uma database, e não haverão daemons para iniciar ou manter rodando.
Você apenas precisará instalar em uma maquina, e podera  gerenciar uma frota inteira de maquinas remotas daquele ponto central.
Quando o Ansible gerencia maquinas remotas, ele não instala software ou roda algo nelas.

# Requerimentos da máquina de controle

Atualmente o Ansible pode rodar em qualquer maquina com Python 2 (2.6,ou 2.7) ou Python 3 (3.5 ou superior) instalado.
(Não existem versões suportadas pra windows como maquina de controle.)

# Requerimentos de máquina controlada
Nos nós gerenciados , você precisa de uma maneira de se comunicas , que normalmente é SSH.
Por padrão é usado o SFTP, se não estiver disponivel você pode mudar para o SPC no arquivo de conf do Ansble.
Você também precisará de Python 2.6 ou superior.

- $ sudo apt-get update
- $ sudo apt-get install software-properties-common
- $ sudo apt-add-repository ppa:ansible/ansible
- $ sudo apt-get update
- $ sudo apt-get install ansible
