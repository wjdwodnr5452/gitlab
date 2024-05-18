# gitlab 구성법
#### 1. docker로 gitlab 구성
- docker pull gitlab/gitlab-ce:latest
- docker run --detach  --hostname gitlab.example.com  --publish 1980:80   --name gitlab  --restart always  --volume D:/docker/gitlab/config:/etc/gitlab --volume D:/docker/gitlab/logs:/var/log/gitlab --volume D:/docker/gitlab/data:/var/opt/gitlab gitlab/gitlab-ce

#### 2. 비밀번호 확인
- docker exec -it gitlab /bin/bash
- cat /etc/gitlab/initial_root_password


