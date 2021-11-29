# PlatOwner（平台方信息）
合约说明：CRUD合约，已继承了Base合约实现其基础的增删改查接口

**参数说明**

| address    | 平台方的地址                      |
| ---------- | --------------------------------- |
| name       | 平台方的名字                      |
| avatar     | 平台方的封面信息（以URL地址存储） |
| totalAsset | 平台被委托的资产总数              |



## exist_plat

#### 功能说明

* 根据地址判断此广告商是否存在

#### 接口说明

**入参**

| 参数    | 类型    | 说明           |
| ------- | ------- | -------------- |
| account | address | 该用平台的地址 |

**出参**

| 参数    | 类型 | 说明                                    |
| ------- | ---- | --------------------------------------- |
| message | bool | true则表示该平台方存在，false则是不存在 |

**出参示例：**

```json
{
    “true”
}
```

<img src="../picture\12.PNG" style="zoom:80%;" />



## getAllAddress

#### 功能说明

* 得到所有平台方的地址

#### 接口说明

**入参**

null

**出参**

| 参数   | 类型     | 说明                             |
| ------ | -------- | -------------------------------- |
| result | string[] | 每一个字符串代表一个平台方的地址 |

**出参示例：**

```json
{
    ["0x9865ac4d5608e12d24d4ca6c9e68c171dbd011c9","0xcce3632fe7e76ac09f5d71bf1ccd9886fbdd8cd7","0x05c8ff853d31090d0dc3c58b0c5f87a4f6ab4016"]
}
```

<img src="../picture/11.PNG" style="zoom:80%;" />