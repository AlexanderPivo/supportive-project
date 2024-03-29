# ��� ����� Git?

## ��������
- Git � ��� ������� �������� ������, ������� �������� ����������� ��������� � �������. ���� ���������� ����� ������������ ��� ��� ��������������, ��� � ��� ��������� ������.
- Git ��������� ��������� ��������� �������� � ��� ������������� ������������ � ���������� ������� �������. ����� ����� ������� �������� ����� �� �������-���������, 
������� �������� � Git, � ���������� ����������� � �������.

��������� � ��������� ������� � �����: [������ �� ����](https://practicum.yandex.ru/trainer/git-basics/lesson/2b82fb35-f581-4cd4-8806-c2a780e53347/)

### ������ ����� �������������� �����:

��� ��������� � ������ ����� ������������ ��������� ������ Git bash, �������� �������:
* pwd - �������� ������� �����
* cd - ������� � ����������
* ls - ����� ����������� ����������
* touch - ������� �����
* mkdir - �������� �����
* cp - ����������� ������ � �����
* mv - ����������� ������ � �����
* cat - ��������� ���� (�� ����. concatenate and print � ����������� � ������������)
* rm - �������� �����  
* rmdir - �������� �����

### ���. �����:
* && - ����������� ���������� ������
* Tab - ������� �������������
* ~ - ������� � �������� ����������

## ����������������:
* git config - �������� ����.-����� � ������� � ���� (���, email)
����� �������� ��� ���������� ���������
* git init - ������������� ����������� � ������� �����
* rm -rf .git - "���������" �����
* git status - ��������� ��������� ����������� 

* git add <��� �����> (��� --all) - ����������� � ���������� ���� � �����������
* git commit -m '<����� ���������>' - ��������� ������� ������ �������������� ������
���� �� ������� ��������� - ��������� ���� ��� ����� ���������, ��������� ��������������: wq (��� ���� ����) 
* git log - ����������� ������� ��������

������� ������:
* git push - �������� (���������) ��������� �/�� ��������� �����������

# GitHub 

## Git � ��������� ��� �������� ������
Git � GitHub � ��� ��� ������ �������, ������� ����������� ���������� ���� �� �����. 
Git:
- ���������� ���������� ��� ������ � ���������� � ��������� �������������;
- ������ � �������� �������� �����.
GitHub:
- ��������� ��� ���������� �������� ������������;
- ����������� �������� Microsoft.

����������� � GitHub [������ �� GitHub](https://github.com/)
������ ��������� �����������:  �� ������� Repositories ������ �� ������ ������ New, ������� ��� (�� �����������, ���� ��������� � ���������)

�� ������ ������������� SSH-���� (��. �������� ����)
ssh-keygen -t ed25519 -C "����������� �����, � ������� �������� ������� �� GitHub"


## ���������� SSH-����� � GitHub-��������

1. ����� ���������� ������� ssh-keygen �� ����������� ����� � ���������� ~/.ssh ����� ������� ��� ����� � id_ed25519 � id_ed25519.pub (��� id_rsa � id_rsa.pub � � ����������� �� ����, ����� �������� �� ������������):<br>
  - id_ed25519/id_rsa � ��������� ���� (���� ��� .pub � �����). �� � ���� ������ �� ��������� ��� � �� �������� ��.<br>
  - id_ed25519.pub/id_rsa.pub � ��������� ���� (�� ��� ��������� ���������� .pub).<br>
���������� ���������� ����� � ��������� ������ � ����� ������:<br>
```  $ clip < ~/.ssh/id_rsa.pub``` <br>
��� ed25519:<br>
```  $ clip < ~/.ssh/id_ed25519.pub``` 


2. ��������� �� GitHub � �������� ����� Settings (����. ����������) � ���� ��������;<br>
� ���� ����� ������� �� ����� SSH and GPG keys;<br>
� ����������� ������� �������� New SSH key (����. ������ SSH-�����);<br>
� ���� Title (����. ����������) �������� �������� �����. ��������, Personal key (����. ������� �����);<br>
� ���� Key type (����. ���� �����) ������ ���� Authentication Key (����. ����� ��������������);<br>
� ���� Key ���������� ��� ���� �� ������ ������;<br>
������� �� ������ Add SSH key (����. ��������� SSH-�����);<br>
��������� ������������ ����� � ������� ��������� �������:<br>
```  $ ssh -T git@github.com``` 


## ������� ��������� � �������� �����������

��������� �������� ����������� � ����������:<br>
* ``` git remote add origin git@github.com:%���_��������%/first-project.git```
* git remote -v - �������� ����� ����� --verbose (����. ����������), � ������� ���� ������� ����� ���������, ��� ����������� �������<br>
������ ���:<br>
* git push -u origin master (��� main)<br>
��������� ����:<br>
* git push







