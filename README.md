# Cloud-Utilizations
(To Me) Utilizing AWS Cloud server instance for Applications

## How to config and run Server

### renting AWS Server instance and Access
After I sign up, and AWS confirmed that I have valid bank account,

[Making AWS EC2 freetier instance](https://taetaetae.github.io/2019/04/14/aws-freetier-create-and-ssh-access/)
* 위 링크의 putty 설치없이, 윈도우 기본 powershell로도 접근 가능, 하단 목차 확인

#### Access by powershell
powershell : Window 제공 Character User Interface 터미널(GUI의 대척점), ssh, scp(sftp 유사) 명령어 및 기능이 기본 지원되어 서버접근이 가능하다.

+ cmd.exe보다 눈이 편하다.

[Accessing by powershell ssh](https://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/AccessingInstancesLinux.html)

### Firewall and Security Group of AWS

####Firewall(웹 방화벽)
(To ME) client(or 외부 ip)에서 접근할 수 있는 추가 통로(포트) 열기

* 22번 포트는, i think, 관리자 제어를 위해 기본적으로 열려있고, ssh 접속은 이 통로로 서버에 접근하는 것으로 이해

####Security Group of AWS
to be supplemented later

#### FTP, Git
to be supplemented later

# Utilization cases
## IaaS-Oriented
(Deploy of WEB-APP Impl Prjs) +

[DEVOPS](https://github.com/devsacti/Cloud-Utilizations/tree/main/DEVOPS)

## PaaS-Oriented
AWS RDS
+
to be supplemented later

## SaaS-oriented 
salesforce,
+
to be supplemented later

# Docker and Kubernetes
to be supplemented later