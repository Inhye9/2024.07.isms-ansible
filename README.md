# 📌 ansible 설치

- ansible 설치

```jsx
# Python 버전 확인 
python -V 

# pip3로 ansible 설치 
pip3 install --upgrade pip
pip install ansible
```

- ansible 설치 확인

```jsx
# ansible 설치 확인
ansible --version
[DEPRECATION WARNING]: Ansible will require Python 3.8 or newer on the controller starting with Ansible
2.12. Current version: 3.7.16 (default, May  6 2024, 19:30:00) [GCC 7.3.1 20180712 (Red Hat 7.3.1-17)].
This feature will be removed from ansible-core in version 2.12. Deprecation warnings can be disabled by
setting deprecation_warnings=False in ansible.cfg.
ansible [core 2.11.12]
  config file = None
  configured module search path = ['/root/.ansible/plugins/modules', '/usr/share/ansible/plugins/modules']
  ansible python module location = /usr/local/lib/python3.7/site-packages/ansible
  ansible collection location = /root/.ansible/collections:/usr/share/ansible/collections
  executable location = /usr/local/bin/ansible
  python version = 3.7.16 (default, May  6 2024, 19:30:00) [GCC 7.3.1 20180712 (Red Hat 7.3.1-17)]
  jinja version = 3.1.4
  libyaml = True
```

# 📌 ansible kubernetes collection 설치

```jsx
ansible-galaxy collection install kubernetes.core
ansible-galaxy collection install community.kubernetes
ansible-galaxy collection install cloud.common
```

# 📌 ansible syntax check

```jsx
ansible-playbook ./ansible/playbook.yaml --syntax-check 
```

# 📌 ansible playbook 실행 (localhost)

```jsx
# ansible playbook 실행 
ansible-playbook ./ansible/playbook.yaml 

# ansible playbook verbose 실행 
ansible-playbook ./ansible/playbook.yaml --verbose
```
