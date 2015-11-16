# Ku8 Project

��ǩ�� ku8-project

---

## 1. Ϊʲô����Ku8 Project

����֪��J2EEƽ̨��WAR���Լ�EAR����׼�淶��ʹ���κ�����������������ķ���J2EE�淶�Ķ����Ʋ�����ܹ��ںܷ���ķ������������̵�J2EE���������С���ʹDockerƽ̨�ϣ�Ҳ�б�׼�ľ����ʽ��������򣬵�kubernetes��Ϊһ�����˵ķֲ�ʽ����ܹ�������ƽ̨��Ŀǰ��û��һ����׼��**�������淶**���������Ŀǰ���������е��߳����������ֵͲ�εĵ��ֹ��ظ������������������׳���������kubernetes�ϵĳ��򿪷��Ͳ���Ǩ�ƣ����ԣ�������ku8eye��Ŀ�����**ku8-project**�ĸ�����ƶ�һ����׼��kubernetes���������׼�������һϵ�еĹ�����ʹ��**ku8-project**�Ĵ���������������������ü򵥷��㡣
     

## 2. Ku8 Project���
һ��**Ku8 Project**��һ������kubernetes�ܹ���������kubernetes�����е�kubernetes��Ŀ������һ��YAML��ʽ���ļ����������̣�snakeYAML��Java��YAML�ο��Ľ����������ο�ʾ�����£�
```yaml
project:mykub8-project1
version:0.1
author:xxx@yyy.com
kuberneteVersion:v1
describe:demo kubernetes project
spec:
  services:
 - name: nginx
     describe:nginx service for my app
     tag:web
     replica:3
     version:0.1
     images: 
       - name:nginx
         version:latest
         registry:192.168.0.1:5000
         imageName:nginx.docker
         command:/bash/bin
         quotas:
            limits:
            cpu: 0.5
            memory: 128Mi
     ports:
      - containerPort: 80
        servicePort:8080
        nodePort:8888
```
����ע�⵽����Ķ�������Kubernetes ServiceΪ���ģ�һ�����̰������Service���壬ÿ��Service�Ķ��������Kuberntes RC��Service�Ķ��壬�Լ�������Ҫ���֣�������Դ�޶�塣
Ĭ������£�Ku8 Project���𵽸��û������⻧�������ռ������������ÿ���⻧������Project��ͬһ�������ռ��У���ͬ�⻧��Project�Ǹ���ģ���ҿ�����ͬ���ķ������ơ�Ҳ���Է��������û��Լ��������ռ��У��������ڸ���˽�е���Ŀ��ͨ���������������ԡ�ѧϰ��Ŀ�ġ�
һ��**Ku8 Project**����Ϊһ����׼��zip��ʽ���ļ���Ŀǰ�ƻ������������ݣ�
 - ��׺��Ϊ.kub8�Ĺ��̶����ļ�
 - docker�����ļ��б�������ѹ���ļ���

## 3. Ku8 Project Builder
����һ�����ӻ��ı༭���ߣ����ڴ���һ��**Ku8 Project**���������ݴ洢��MySQL������ku8project������Ŀ�����ļ�(YAML)��Ϊһ��text�ֶ������Ĵ洢����������У���Ҫ�Ƕ���Service��Project�Ľ��棬����չʾ������Ϣְλ����Ҫչʾ������б���Ϣ���ο����£�
![ImageLoadFailed](../../res/ku8-project-create.PNG)

ÿ������Ķ������ο����£�һ�����������Ӷ��������ͨ��Ϊ1������
 ![ImageLoadFailed](../../res/ku8-service-create.PNG)
 
## 4. Ku8 Project�ķ�������
�������̾����Ϊ���¼�����

 - ѡ�񷢲���**Ŀ�껷��**���������ڵ�Cluster���ĳ��ku8 Group�ϣ��Լ���Ŀ���ڵ�**�����ռ�**��Ĭ��Ϊ�⻧����������ռ䡣
 - ����Ŀ�껷����Project�Ķ�����Ϣ��ÿ���������ɶ�Ӧ��һϵ��Kubernetes���󣬰���RC��Service�Ķ���ȣ������ѡ�񷢲���ĳ��Group�ϣ�����Ҫ�޸�RC��Pod��NodeSelector���ԣ�ƥ��ָ����Group��Label��
 - ����Project�����Ĳ���ʵ�����Լ�������ı�Ku8projInstance�Լ�ku8projserviceinst��ku8projrcinst��
 - ˳�����API Server�����API����������������

## 5. ������
 **�����������ƣ�todo**

  

 