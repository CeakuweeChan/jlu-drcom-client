---------------
### Simple JLU drcom client dirty hack C-version

��Ҫ�޸� drcom.c �ļ��� user(�ʺ�), pass(����), mac(MAC ��ַ, 0x010203040506 ��ʽ) �Ȳ�������ȡ MAC ��ַ
	
	echo 0x`ifconfig eth | egrep -io "([0-9a-f]{2}:){5}[0-9a-f]{2}" | tr -d ":"`
	
����
	
	gcc drcom.c md5.c -o drcom
	

ֱ�����ն����� ./drcom 

haha, dirty hack ����ˬ (������)��

��Ϊ�� daemon ��ʽ���У�ȥ�� long ���ͣ�֧�� 32 λϵͳ

TODO: logout


