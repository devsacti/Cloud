# Cloud-Utilizations
(To Me) Utilizing AWS Cloud server instance for Applications

## How to config and run Server

### renting AWS Server instance and Access
After I sign up, and AWS confirmed that I have valid bank account,

[Making AWS EC2 free-tier instance](https://taetaetae.github.io/2019/04/14/aws-freetier-create-and-ssh-access/)
* 위 링크의 putty 설치없이, 윈도우 기본 powershell로도 접근 가능, 하단 목차 확인

#### Access by powershell
powershell : Window 제공 Character User Interface 터미널(GUI의 대척점), ssh, scp(sftp 유사) 명령어 및 기능이 기본 지원되어 서버접근이 가능하다.

+ cmd.exe보다 눈이 편하다.

[Accessing by powershell ssh](https://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/AccessingInstancesLinux.html)

### Firewall and Security Group of AWS

#### Firewall(웹 방화벽)
(To ME) client(or 외부 ip)에서 접근할 수 있는 추가 통로(포트) 열기

* 22번 포트는, i think, 관리자의 서버 접근을 위해 기본적으로 열려있고, ssh 접속은 이 통로로 서버에 접근하는 것으로 이해

#### Security Group of AWS
(To ME) AWS EC2 방화벽 설정을 지원해주는 AWS 서비스

* [To be supplemented : what is Security Group](https://m.blog.naver.com/PostView.naver?isHttpsRedirect=true&blogId=jwyoon25&logNo=221498209697)

##### basic port
80 : http , 443 : https, 22 : ssh

### Continuous Integration and Continuous Delivery(CI/CD)
(To ME)the sustainable and accessible platform where multiple developers can collarborate conveniently

#### Git and Github
(To ME)Implementation of CI/CD

(ex)

1. Link Projects like JAVA-APP of STS to repository of Github
[Link STS with Github](https://all-record.tistory.com/163)

* Caution! Based on 2022, github password is Security Token of Repo, not password of github account

##### steps of Git bash in Window VS its of STS
' git add . ' -> ' git commit -m "~" ' -> ' git push origin main ' in Git Bash

<=>

Right click the Project of Package Explorer
-> Team
-> Add to Index
-> perspective Git or Git Staging of STS
-> move certain file(s) from unstaging to staging
-> Insert Commit Message and Commit + Push (it requires Github login with same way of above)

2. config AWS Linux 2 Server to pull from above repository of github
[config AWS from jdk to git](https://tigger.dev/entry/aws-git)

* jdk has JRE that can make JAVA-APP work, with Git, it is component of CD

##### the related
 File Transfer Protocol(FTP), FTP is protocol(or guideline) to support sending file

Implementation method of FTP : [how to use Filezilla](https://luji.tistory.com/9)

[SCP vs SFTP](https://parkadd.tistory.com/129)

To be supplemented later.. 

# Utilization cases
## IaaS-Oriented
(Deploy of WEB-APP Impl Prjs) +

[DEVOPS](https://github.com/devsacti/Cloud-Utilizations/tree/main/DEVOPS)

## PaaS-Oriented
AWS RDS
+
to be supplemented later

## SaaS-oriented 
salesforce CRM,
+
to be supplemented later

# Docker and Kubernetes
to be supplemented later

# Background
[Server](https://github.com/devsacti/Server)