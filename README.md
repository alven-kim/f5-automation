F5 Automation with JIRA(Python3)
================================

Version: Python3
----------------


F5 Node-Pool-Pool-Member-VServer 생성 자동화
-----------------------------------------------
### Directory : f5_automation
### File_Name : f5_auto_vserver.py.github
### Needs Tools
 - 없음.  

### 사용방법
 - insert_node.txt 파일에 [노드네임] [노드IP] 순으로 삽입.  
 - ~~자료구조(list/dict/split)를 직접 추가하여 생성하는 방법은 유연성이 떨어져 사용하지 않음.~~

### Running Result(Sample)
```bash
root# ./f5_auto_def_run.py
F5 Device Domain(or IP): 10.20.30.5
F5 GUI Username: alven-kim
F5 GUI Password:
VIP Insert: 10.20.50.100
VPORT Insert: 443
Description Insert: TEST-449
HTTP or HTTPS: https
############################## F5 Node ~ VServer Create Automation START ##############################
Success ----- Node Create Node: api01.test.node IP: 172.20.50.211
Success ----- Node Create Node: api02.test.node IP: 172.20.50.214
Success ----- Node Create Node: api03.test.node IP: 172.20.50.193
Success ----- Node Create Node: api04.test.node IP: 172.20.50.189
Success ----- Node Create Node: api05.test.node IP: 172.20.50.216
Success ----- Node Create Node: api06.test.node IP: 172.20.50.213
Success ----- Node Create Node: api07.test.node IP: 172.20.50.219
Success ----- Node Create Node: api08.test.node IP: 172.20.50.208
Success ----- Node Create Node: api09.test.node IP: 172.20.50.218
Success ----- Node Create Node: api10.test.node IP: 172.20.50.210
RPORT Input: 8080
Success ----- Pool Create Pool: test.alvenkim.com_8080
Success ----- Pool-Member Create Member-Node: api01.test.node Member-IP: 172.20.50.211
Success ----- Pool-Member Create Member-Node: api02.test.node Member-IP: 172.20.50.214
Success ----- Pool-Member Create Member-Node: api03.test.node Member-IP: 172.20.50.193
Success ----- Pool-Member Create Member-Node: api04.test.node Member-IP: 172.20.50.189
Success ----- Pool-Member Create Member-Node: api05.test.node Member-IP: 172.20.50.216
Success ----- Pool-Member Create Member-Node: api06.test.node Member-IP: 172.20.50.213
Success ----- Pool-Member Create Member-Node: api07.test.node Member-IP: 172.20.50.219
Success ----- Pool-Member Create Member-Node: api08.test.node Member-IP: 172.20.50.208
Success ----- Pool-Member Create Member-Node: api09.test.node Member-IP: 172.20.50.218
Success ----- Pool-Member Create Member-Node: api10.test.node Member-IP: 172.20.50.210
Success ----- Create Virtual-Server test.alvenkim.com_443
```


TODO
----
 - 불필요한 모듈 정리


See also
---------
F5-SDK - https://f5-sdk.readthedocs.io/en/latest/
