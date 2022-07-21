# Renting Cloud Server
make instance of server

## Oracle
[goto](https://iter.kr/%EC%98%A4%EB%9D%BC%ED%81%B4-%ED%81%B4%EB%9D%BC%EC%9A%B0%EB%93%9C-%EC%9D%B8%EC%8A%A4%ED%84%B4%EC%8A%A4-%EC%83%9D%EC%84%B1/)
Oracle Linux 8
Image build: 2022.06.30-0

#### 윈도우10 SSH 접속시 PEM 파일 퍼미션 에러 해결방법
Permissions for '~' are too open. blabla

[solution](https://techsoda.net/windows10-pem-file-permission-settings/)

## AWS
(To Be Supplemented..)


# SSh to Server

## Oracle
[Oracle](https://docs.oracle.com/en-us/iaas/Content/Compute/Tasks/accessinginstance.htm)

*단, 위 문서대로는 윈도우10 퍼미션 에러 해결이안되므로 상단 링크 확인 필수

```
ssh -i <private_key_file> <username>@<public-ip-address>

```

## AWS
[AWS > aws-documentation > Amazon EC2](https://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/AccessingInstancesLinux.html)

[powershell 전 pem설정](https://www.overtop.co.kr/361)

```
ssh -i /path/my-key-pair.pem my-instance-user-name@my-instance-public-dns-name

_EIP 설정 시

ssh -i /path/my-key-pair.pem my-instance-user-name@[EIP]


ssh -v -i D:\Key\mission.pem ec2-user@54.180.177.202 ? 
```


## Security config



# id login
(~.pem 방식 접근 후 유저 생성한 경우)

## Oracle

## AWS
ec2-user only

root, admin, developer

```

ssh [username]@[dns]

ssh [username]@[EIP]

```

# Extensions
1. [install jdk and jenkins for cicd](./jenkins.md)

2. [temp](./temp.md)