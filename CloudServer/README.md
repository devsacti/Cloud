# SSh to EC2
[AWS > aws-documentation > Amazon EC2](https://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/AccessingInstancesLinux.html)

AwsServer(Amazon Linux2 AMI) powershell connect config

?
powershell 전 pem설정
https://www.overtop.co.kr/361

## Security config

## key login
(powershell)
```
ssh -i /path/my-key-pair.pem my-instance-user-name@my-instance-public-dns-name

_EIP 설정 시

ssh -i /path/my-key-pair.pem my-instance-user-name@[EIP]


ssh -v -i D:\Key\mission.pem ec2-user@54.180.177.202 ? 
```

(~.pem 방식 접근 후 유저 생성한 경우)

## id login

ec2-user only

root, admin, developer

```

ssh [username]@[dns]

ssh [username]@[EIP]

```

# config JDK
```
sudo yum install -y java-1.8.0-openjdk-devel.x86_64
sudo /usr/sbin/alternatives --config java
```