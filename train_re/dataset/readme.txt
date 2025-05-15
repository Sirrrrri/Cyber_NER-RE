1. 文件说明
--sentences.txt 关系三元组所在的句子，其中，<e1>xxx</e1>中的xxx表示关系三元组中的头实体，<e2>zzz</e2>中的zzz表示关系三元组中的尾实体。
--labels.txt 文件sentences.txt中每个关系三元组对应的关系标签。

2. 标签说明
##########################################
1	noRelation：实体对之间不存在关系
0	isA ：（恶意软件）属于（某恶意软件家族）
2	targets：（恶意软件、攻击组织）攻击（地理位置）
3	uses：（恶意软件）使用（某应用）
4	hasAuthor：恶意软件由某攻击组织开发
6	variantOf：恶意软件变体
7	hasAlias：（恶意软件、攻击组织）别名
8	indicates：（IOC失陷指标，如命令、HASH、文件名、URL等）检测出（某恶意软件）
10	exploits：（恶意软件）利用（漏洞、恶意软件、邮件）

###### 修改了label中的 5 和 10

{
    "noRelation": 1,
    "isA": 0,
    "targets": 2,
    "uses": 3,
    "hasAuthor": 4,
    "variantOf": 5,
    "hasAlias": 6,
    "indicates": 7,
    "exploits": 8
}