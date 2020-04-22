# Jumpserver Ansible-playbook

未完成

```
$ yum -y install epel-release git curl sshpass
$ yum -y install python2-pip
$ ssh-keygen -t rsa
$ cd /opt
$ git clone --depth=1 https://github.com/wojiushixiaobai/jms_ansible.git
$ cd jms_ansible
$ mkdir ~/.pip
$ echo -e "[easy_install]\nindex_url = https://mirrors.aliyun.com/pypi/simple/" > ~/.pydistutils.cfg
$ echo -e "[global]\nindex-url = https://mirrors.aliyun.com/pypi/simple/\n\n[install]\ntrusted-host=mirrors.aliyun.com" > ~/.pip/pip.conf
$ pip install -r requirements/requirements.txt
$ vi inventory.ini
$ ansible-playbook deploy_user.yml -uroot -k
$ ansible all -m shell -a 'whoami'
$ ansible-playbook deploy_prepare.yml
$ ansible-playbook deploy.yml

```
