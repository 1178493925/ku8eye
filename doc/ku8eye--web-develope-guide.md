# ku8eye web���̱�������

���̲�����spring-boot������򻯿����Ͳ�������Դ�빤�̣�
https://github.com/bestcloud/ku8eye/tree/master/src/ku8eye-web
��eclipse�е���maven��Ŀ��ִ��Run As����> Maven Build�����ɱ���Դ�룬����ɹ��Ժ���targetĿ¼��������all in one��JAR��ku8eye-web-xxxxx.jar,���������������⣬���������� java -jar ku8eye-web-xxxxx.jar��������Web����������������http://localhost:8080���ɷ��ʡ�
eclipse�е����ʱ������Run As����>Java Application��������Web��
��Ŀ��������JDK 7��

## ����Ŀ¼˵��
src\mainĿ¼Ϊ��ҪԴ��
src\testĿ¼Ϊ����Դ�룬��ҪΪ��Ԫ����
src\mainĿ¼�����°��ṹ��

 - org.ku8eye.domainĿ¼Ϊ����������Щ������Ӧmysql���ݿ����һ����
 - org.ku8eye.bean��Ϊ����Java Bean�����������ݴ��ݻ�ת����Ŀ��
 - org.ku8eye.rest��Ϊ�ṩRest�����Java������������ڲ����ⲿϵͳ����
 - org.ku8eye.ctrl��ΪSpring MVC��Controller�������ڵط�
 - org.ku8eye.service��ΪSpring��Service Bean�������ڵط�
 ����ctrl����service�����԰���ģ�����Ʒ��Ӱ�������org.ku8eye.ctrl.user.xxx

ҳ���ļ�����̬��JSP��JS��Images�ȣ���������Ŀ¼
 - src\main\resources\static  ��Web������ROOTĿ¼