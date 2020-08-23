## redis를 위한 설정 파일 (standalone, sentinel, cluster)
- 같은 머신에서 포트만 달리하여 여러 redis server를 띄우기 용도
- standalone을 위해서 6379(master), 6380(replica) 두 개의 redis server를 이용할 수 있음
- sentinel을 위해서 26379, 26380, 26381 포트에 띄워져 있는 sentinel을 연결할 수 있고 이들은 6379(master), 6380(replica)의 상태를 체크하고 있음
- cluster를 위해서 7000, 7001, 7002, 7003, 7004, 7005 포트에 띄워져 있는 노드를 연결할 수 있음