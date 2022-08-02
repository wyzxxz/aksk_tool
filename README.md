# aksk_tool
aksk tool
```
download_url : https://toolaffix.oss-cn-beijing.aliyuncs.com/20220801/aksk_tool.jar

部分优化
> java -jar aksk_tool.jar
[-] Usage: java -jar aksk_tool.jar ak sk
[-] Usage: java -jar aksk_tool.jar ak sk token
[-] Usage: java -jar aksk_tool.jar ak sk region=xxx         指定地域
[-] Usage: java -jar aksk_tool.jar ak sk product=oss,cos    指定产品
[-] Usage: java -jar aksk_tool.jar ak sk region=xxx  product=oss,cos    指定地域和产品

[-] qiniu Usage: java -jar aksk_tool.jar ak sk bucket_name bucket_url


目前支持 阿里云，腾讯云，华为云，七牛云存储

阿里云
支持 AKSK认证，STS认证
支持 ECS, OSS, RDS, REDIS, RAM , DOAIM 的功能调用
1. ECS      ECS详情查询，命令执行，安全组添加/删除
2. OSS      OSS文件上传，下载，删除，查询
3. RDS      RDS详情查询，数据库账号添加/删除，IP白名单修改
4. REDIS    REDIS详情查询，密码修改
5. RAM      RAM账号添加/删除, 新增/删除AK
6. DOMAIN   DOMAIN域名查询，子域名解析增删改查等


腾讯云
支持 AKSK认证，TOKEN认证
支持 CVM, DOAIM, COS 的功能调用
1. CVM      CVM详情查询，实例启动，关闭，密码重置，命令执行（需要安装Agent）
2. DOMAIN   DOMAIN域名查询
3. COS      COS文件存储，文件的增删改查和临时url生成
4. CDB      CDB数据库账号操作，增删改查等
5. CAM      账号（包含AK）增删改查


华为云
支持 AKSK认证，TOKEN认证
支持 ECS, RDS, IAM 的功能调用
1. ECS      CVM详情查询，密码重置，安全组操作
2. RDS      RDS实例查询
3. IAM      账户查询，新增AK，用户组用户增删改查



七牛云存储
支持 AKSK认证
> qiniu Usage: java -jar aksk_tool.jar ak sk bucket_name bucket_url


$java -jar aksk_tool.jar LTAI*******  aaaaaaaaaaaaaaaaaaaaaaaa
$java -jar aksk_tool.jar STS.AAI*******  aaaaaaaaaaaaaaaaaaaaaaaa   TOKENASDASDSADSADASDSAADADSADSA
[-] AK: LTAI*******  SK: aaaaaaaaaaaaaaaaaaaaaaaa
> account name: wyzxxz
> account uid:  100000000000000
> account cash: 999999999999999999999
[-] regions list: 
| Num | Region_Id            | Region_Name         |
| 1   | cn-qingdao           | 华北1（青岛）             |
| 2   | cn-beijing           | 华北2（北京）             |
| 3   | cn-zhangjiakou       | 华北3（张家口）            |
| 4   | cn-huhehaote         | 华北5（呼和浩特）           |
| 5   | cn-wulanchabu        | 华北6（乌兰察布）           |
| 6   | cn-hangzhou          | 华东1（杭州）             |
| 7   | cn-shanghai          | 华东2（上海）             |
| 8   | cn-shenzhen          | 华南1（深圳）             |
| 9   | cn-heyuan            | 华南2（河源）             |
| 10  | cn-guangzhou         | 华南3（广州）             |
| 11  | cn-chengdu           | 西南1（成都）             |
| 12  | cn-hongkong          | 中国（香港）              |
| 13  | ap-northeast-1       | 亚太东北 1 (东京)         |
| 14  | ap-southeast-1       | 亚太东南 1 (新加坡)        |
| 15  | ap-southeast-2       | 亚太东南 2 (悉尼)         |
| 16  | ap-southeast-3       | 亚太东南 3 (吉隆坡)        |
| 17  | ap-southeast-5       | 亚太东南 5 (雅加达)        |
| 18  | ap-south-1           | 亚太南部 1 (孟买)         |
| 19  | us-east-1            | 美国东部 1 (弗吉尼亚)       |
| 20  | us-west-1            | 美国西部 1 (硅谷)         |
| 21  | eu-west-1            | 英国 (伦敦)             |
| 22  | me-east-1            | 中东东部 1 (迪拜)         |
| 23  | eu-central-1         | 欧洲中部 1 (法兰克福)       |
| 24  | cn-nanjing           | 华东5（南京-本地地域）        |

[-] search Resource: 
INFO > cn-qingdao          - ECS: 1    - MYSQL: 0    - SQLServer: 0    - PostgreSQL: 0    - REDIS: 0    - OSS_BUCKET: 1 
INFO > cn-beijing          - ECS: 1    - MYSQL: 3    - SQLServer: 0    - PostgreSQL: 1    - REDIS: 0    - OSS_BUCKET: 1   
INFO > cn-zhangjiakou      - ECS: 1    - MYSQL: 1    - SQLServer: 0    - PostgreSQL: 0    - REDIS: 0    - OSS_BUCKET: 1   
INFO > cn-huhehaote        - ECS: 1    - MYSQL: 0    - SQLServer: 0    - PostgreSQL: 0    - REDIS: 0    - OSS_BUCKET: 1   
INFO > cn-wulanchabu       - ECS: 0    - MYSQL: 0    - SQLServer: 0    - PostgreSQL: 0    - REDIS: 0    - OSS_BUCKET: 1   
INFO > cn-hangzhou         - ECS: 1    - MYSQL: 1    - SQLServer: 0    - PostgreSQL: 1    - REDIS: 0    - OSS_BUCKET: 1   
INFO > cn-shanghai         - ECS: 1    - MYSQL: 1    - SQLServer: 0    - PostgreSQL: 0    - REDIS: 0    - OSS_BUCKET: 1   
INFO > cn-shenzhen         - ECS: 1    - MYSQL: 0    - SQLServer: 0    - PostgreSQL: 0    - REDIS: 1    - OSS_BUCKET: 1   
INFO > cn-heyuan           - ECS: 1    - MYSQL: 0    - SQLServer: 0    - PostgreSQL: 0    - REDIS: 0    - OSS_BUCKET: 1   
INFO > cn-guangzhou        - ECS: 0    - MYSQL: 0    - SQLServer: 0    - PostgreSQL: 0    - REDIS: 0    - OSS_BUCKET: 1   
INFO > cn-chengdu          - ECS: 1    - MYSQL: 0    - SQLServer: 0    - PostgreSQL: 0    - REDIS: 0    - OSS_BUCKET: 1   
INFO > cn-hongkong         - ECS: 1    - MYSQL: 1    - SQLServer: 0    - PostgreSQL: 0    - REDIS: 0    - OSS_BUCKET: 1   
INFO > ap-northeast-1      - ECS: 2    - MYSQL: 0    - SQLServer: 0    - PostgreSQL: 0    - REDIS: 0    - OSS_BUCKET: 1   
INFO > ap-southeast-1      - ECS: 1    - MYSQL: 0    - SQLServer: 0    - PostgreSQL: 0    - REDIS: 0    - OSS_BUCKET: 1   
INFO > ap-southeast-2      - ECS: 1    - MYSQL: 0    - SQLServer: 0    - PostgreSQL: 0    - REDIS: 0    - OSS_BUCKET: 1   
INFO > ap-southeast-3      - ECS: 1    - MYSQL: 0    - SQLServer: 0    - PostgreSQL: 0    - REDIS: 0    - OSS_BUCKET: 1   
INFO > ap-southeast-5      - ECS: 1    - MYSQL: 0    - SQLServer: 0    - PostgreSQL: 0    - REDIS: 0    - OSS_BUCKET: 1   
INFO > ap-south-1          - ECS: 1    - MYSQL: 0    - SQLServer: 0    - PostgreSQL: 0    - REDIS: 0    - OSS_BUCKET: 1   
INFO > us-east-1           - ECS: 1    - MYSQL: 0    - SQLServer: 0    - PostgreSQL: 0    - REDIS: 0    - OSS_BUCKET: 1   
INFO > us-west-1           - ECS: 4    - MYSQL: 0    - SQLServer: 0    - PostgreSQL: 0    - REDIS: 0    - OSS_BUCKET: 1   
INFO > eu-west-1           - ECS: 1    - MYSQL: 0    - SQLServer: 0    - PostgreSQL: 0    - REDIS: 0    - OSS_BUCKET: 1   
INFO > me-east-1           - ECS: 1    - MYSQL: 0    - SQLServer: 0    - PostgreSQL: 0    - REDIS: 0    - OSS_BUCKET: 1   
INFO > eu-central-1        - ECS: 2    - MYSQL: 0    - SQLServer: 0    - PostgreSQL: 0    - REDIS: 0    - OSS_BUCKET: 1   
INFO > cn-nanjing          - ECS: 0    - MYSQL: 0    - SQLServer: 0    - PostgreSQL: 0    - REDIS: 0    - OSS_BUCKET: 1       
[-] find regions list: 
0: cn-qingdao -->   ECS: 1  MYSQL: 1
1: cn-beijing -->   ECS: 10  MYSQL: 1  REDIS: 2
2: cn-zhangjiakou -->   ECS: 1  MYSQL: 1
3: cn-huhehaote -->   ECS: 1
4: cn-hangzhou -->   ECS: 1  MYSQL: 1  REDIS: 1
5: cn-shanghai -->   ECS: 1  MYSQL: 1
6: cn-shenzhen -->   ECS: 1
7: cn-heyuan -->   ECS: 1
8: cn-chengdu -->   ECS: 1
9: cn-hongkong -->   ECS: 1  MYSQL: 1
10: ap-northeast-1 -->   ECS: 1
11: ap-southeast-1 -->   ECS: 1
12: ap-southeast-2 -->   ECS: 1
13: ap-southeast-3 -->   ECS: 1
14: ap-southeast-5 -->   ECS: 1
15: ap-south-1 -->   ECS: 1
16: us-east-1 -->   ECS: 1
17: us-west-1 -->   ECS: 4
18: eu-west-1 -->   ECS: 1
19: me-east-1 -->   ECS: 1
20: eu-central-1 -->   ECS: 1
[-] please enter the number(0-20)
> 0
[-] use region: cn-qingdao
[-] use region: cn-qingdao
[-] please choose product: 
1. ECS
2. OSS
3. RDS
4. REDIS
5. RAM
6. DOMAIN
> 1
[-] Instance list: 
| Num   | Instance_ID  | Public_IP    | CPU   | Memory     | Instance_Status | OS_Name              | Instance_Name        | Security_Group       |
| 1     | i-test       | 1.1.1.1      | 4     | 16G        | Running         | Ubuntu  18.04 64位   | test-qingdao-01      | sg-secgroupid        |

[-] find instance list: 
0: i-test,test-qingdao-01
[-] please enter the number(0-0),  enter back to re-choose region
> 0
[-] use instance: i-test,test-qingdao-01
[-] Instance Detail: 
# Os name: Ubuntu  18.04 64位
# Hostname: test-qingdao-01
# RegionId: cn-qingdao
# Instance Id: i-testname
# Instance Name: i-test
# InnerIp: 
# Public Ip: 1.1.1.1
# Security GroupId: sg-secgroupid
# Start Time: 2011-01-04T12:36Z
# Expired Time: 2023-01-02T12:00Z
# CPU: 4
# Memory: 16384 M
# Status: Running
# Disk size: 150 G
[-] please enter command, enter q or quit to quit, enter back to re-choose instance
[-] example: cmd=whoami    sec_group_info=SecruityGroupId    sec_group_add=SecruityGroupId:ip    sec_group_del=SecruityGroupId:ip
> sec_group_info=sg-secgroupid
[-] Security Group Detail: 
# Protocol: TCP, Ip:0.0.0.0/0, PortRange:3389/3389, SourceRange:, Policy:Drop, NicType:intranet, CreatTime:2011-01-02T09:17:10Z
# Protocol: TCP, Ip:0.0.0.0/0, PortRange:3389/3389, SourceRange:, Policy:Accept, NicType:intranet, CreatTime:2011-01-02T09:17:10Z
# Protocol: ICMP, Ip:0.0.0.0/0, PortRange:-1/-1, SourceRange:-1/-1, Policy:Accept, NicType:intranet, CreatTime:2011-01-02T09:17:09Z
# Protocol: TCP, Ip:0.0.0.0/0, PortRange:22/22, SourceRange:, Policy:Accept, NicType:intranet, CreatTime:2011-01-02T09:17:09Z
[-] please enter command, enter q or quit to quit, enter back to re-choose instance
[-] example: cmd=whoami    sec_group_info=SecruityGroupId    sec_group_add=SecruityGroupId:ip    sec_group_del=SecruityGroupId:ip
> cmd=whoami
[-] command: whoami
命令创建完成
命令执行完成
root

[-] please enter command, enter q or quit to quit, enter back to re-choose instance
[-] example: cmd=whoami    sec_group_info=SecruityGroupId    sec_group_add=SecruityGroupId:ip    sec_group_del=SecruityGroupId:ip
> sec_group_add=sg-secgroupid:8.8.8.8
入方向安全组新增成功
[-] please enter command, enter q or quit to quit, enter back to re-choose instance
[-] example: cmd=whoami    sec_group_info=SecruityGroupId    sec_group_add=SecruityGroupId:ip    sec_group_del=SecruityGroupId:ip
> q

```
