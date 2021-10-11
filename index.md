<!--
 * @Author: 戈灵虎
 * @Date: 2021-08-16 17:33:28
 * @LastEditTime: 2021-10-11 15:15:23
 * @LastEditors: Please set LastEditors
 * @Description: In User Settings Edit
 * @FilePath: /undefined/Users/gelinghu/Documents/100baotech/接口文档/数据同步接口文档.md
-->

<h1 align='center'> 百保科技数据同步接口文档 </h1>
<!-- TOC -->

- [1. 版本信息](#1-版本信息)
- [2. 请求网关](#2-请求网关)
- [3. 请求资源类型](#3-请求资源类型)
- [4. 参数类型说明](#4-参数类型说明)
- [5. 名词解释](#5-名词解释)
- [6. 响应](#6-响应)
    - [6.1. Http状态码](#61-http状态码)
    - [6.2. 业务状态码](#62-业务状态码)
- [7. 公共请求参数](#7-公共请求参数)
    - [7.1. 请求示例](#71-请求示例)
    - [7.2. 响应 200](#72-响应-200)
- [8. 接口列表](#8-接口列表)
    - [8.1. 保单托管](#81-保单托管)
        - [8.1.1. 明细数据](#811-明细数据)
            - [8.1.1.1. 描述](#8111-描述)
            - [8.1.1.2. request](#8112-request)
                - [8.1.1.2.1. HTTP请求示例](#81121-http请求示例)
            - [8.1.1.3. response](#8113-response)
                - [8.1.1.3.1. HTTP响应示例](#81131-http响应示例)
                    - [8.1.1.3.1.1. 响应 200](#811311-响应-200)
        - [8.1.2. 统计数据](#812-统计数据)
            - [8.1.2.1. 描述](#8121-描述)
            - [8.1.2.2. request](#8122-request)
                - [8.1.2.2.1. HTTP请求示例](#81221-http请求示例)
            - [8.1.2.3. response](#8123-response)
                - [8.1.2.3.1. HTTP响应示例](#81231-http响应示例)
                    - [8.1.2.3.1.1. 响应 200](#812311-响应-200)
    - [8.2. 产品对比](#82-产品对比)
        - [8.2.1. 明细数据](#821-明细数据)
            - [8.2.1.1. 描述](#8211-描述)
            - [8.2.1.2. request](#8212-request)
                - [8.2.1.2.1. HTTP请求示例](#82121-http请求示例)
            - [8.2.1.3. response](#8213-response)
                - [8.2.1.3.1. HTTP响应示例](#82131-http响应示例)
                    - [8.2.1.3.1.1. 响应 200](#821311-响应-200)
        - [8.2.2. 统计数据](#822-统计数据)
            - [8.2.2.1. 描述](#8221-描述)
            - [8.2.2.2. request](#8222-request)
                - [8.2.2.2.1. HTTP请求示例](#82221-http请求示例)
            - [8.2.2.3. response](#8223-response)
                - [8.2.2.3.1. HTTP响应示例](#82231-http响应示例)
                    - [8.2.2.3.1.1. 响应 200](#822311-响应-200)
    - [8.3. 单品计划书](#83-单品计划书)
        - [8.3.1. 明细数据](#831-明细数据)
            - [8.3.1.1. 描述](#8311-描述)
            - [8.3.1.2. request](#8312-request)
                - [8.3.1.2.1. HTTP请求示例](#83121-http请求示例)
            - [8.3.1.3. response](#8313-response)
                - [8.3.1.3.1. HTTP响应示例](#83131-http响应示例)
                    - [8.3.1.3.1.1. 响应 200](#831311-响应-200)
        - [8.3.2. 统计数据](#832-统计数据)
            - [8.3.2.1. 描述](#8321-描述)
            - [8.3.2.2. request](#8322-request)
                - [8.3.2.2.1. HTTP请求示例](#83221-http请求示例)
            - [8.3.2.3. response](#8323-response)
                - [8.3.2.3.1. HTTP响应示例](#83231-http响应示例)
                    - [8.3.2.3.1.1. 响应 200](#832311-响应-200)
    - [8.4. 家庭计划书](#84-家庭计划书)
        - [8.4.1. 明细数据](#841-明细数据)
            - [8.4.1.1. 描述](#8411-描述)
            - [8.4.1.2. request](#8412-request)
                - [8.4.1.2.1. HTTP请求示例](#84121-http请求示例)
            - [8.4.1.3. response](#8413-response)
                - [8.4.1.3.1. HTTP响应示例](#84131-http响应示例)
                    - [8.4.1.3.1.1. 响应 200](#841311-响应-200)
        - [8.4.2. 统计数据](#842-统计数据)
            - [8.4.2.1. 描述](#8421-描述)
            - [8.4.2.2. request](#8422-request)
                - [8.4.2.2.1. HTTP请求示例](#84221-http请求示例)
            - [8.4.2.3. response](#8423-response)
                - [8.4.2.3.1. HTTP响应示例](#84231-http响应示例)
                    - [8.4.2.3.1.1. 响应 200](#842311-响应-200)
    - [8.5. 保单置换](#85-保单置换)
        - [8.5.1. 明细数据](#851-明细数据)
            - [8.5.1.1. 描述](#8511-描述)
            - [8.5.1.2. request](#8512-request)
                - [8.5.1.2.1. HTTP请求示例](#85121-http请求示例)
            - [8.5.1.3. response](#8513-response)
                - [8.5.1.3.1. HTTP响应示例](#85131-http响应示例)
                    - [8.5.1.3.1.1. 响应 200](#851311-响应-200)
        - [8.5.2. 统计数据](#852-统计数据)
- [9. 相关字典](#9-相关字典)
    - [9.1. 家庭成员关系](#91-家庭成员关系)
    - [9.2. 证件类型](#92-证件类型)
    - [9.3. 产品类型](#93-产品类型)
    - [9.4. 保单状态](#94-保单状态)

<!-- /TOC -->

# 1. 版本信息

*当前版本* : v1.5

| 序号 | 更新内容概要                                                                         | 更新人 | 更新日期   | 版本号 |
|------|--------------------------------------------------------------------------------------|--------|------------|--------|
| 1    | 建立                                                                                 | 戈灵虎 | 2021.08.17 | v0.1   |
| 2    | 发布                                                                                 | 戈灵虎 | 2021.08.17 | v1.0   |
| 3    | 1、增加数据字典<br> 2、增加家庭成员证件号<br>3、增加被保人受益人<br> 4、新增险种类型 | 戈灵虎 | 2021.08.18 | v1.1   |
| 4    | 1、新增家庭编码、计划书编码等<br> 2、新增代理人数据统计                              | 戈灵虎 | 2021.09.01 | v1.2   |
| 5    | 1、参数名称修正                                                                      | 戈灵虎 | 2021.09.10 | v1.3   |
| 6    | 1、置换新增创建时间 2、单页增加创建时间                                              | 戈灵虎 | 2021.09.29 | v1.4   |
| 7    | 增加更新时间                                                                         | 戈灵虎 | 2021.09.30 | v1.5   |

# 2. 请求网关

```js
https://api.100baotech.com
```

# 3. 请求资源类型

| 类型   | 名称   | 说明     |
|--------|--------|----------|
| GET    | get    | 获取资源 |
| POST   | post   | 创建资源 |
| PUT    | put    | 更新资源 |
| DELETE | delete | 删除资源 |

# 4. 参数类型说明

| 类型   | 名称   | 说明         | 示例                    |
|--------|--------|--------------|-------------------------|
| Header | herder | 请求头       | Authorization='*******' |
| Path   | path   | PathVariable | /report/{familyCode}    |
| Query  | query  | RequestParam | /report?code=123        |
| Body   | body   | RequestBody  | Object                  |

# 5. 名词解释

| 名称                         | 说明               |
|------------------------------|--------------------|
| 租户编码 (tenantCode)        | 平台提供           |
| 应用编码 (appId)             | 平台提供           |
| 应用密钥 (appSecret)         | 平台提供           |
| 平台公钥 (platformPublicKey) | 平台提供           |
| 应用公钥 (appPublicKey)      | RSA2生成(2048长度) |
| 应用私钥 (appPrivateKey)     | RSA2生成(2048长度) |

# 6. 响应

## 6.1. Http状态码

| HTTP代码 | 说明         | 类型       |
|----------|--------------|------------|
| **200**  | OK           | data       |
| **201**  | Created      | 无内容     |
| **401**  | Unauthorized | 未授权登录 |
| **403**  | Forbidden    | 权限不足   |
| **404**  | Not Found    | 资源不存在 |

## 6.2. 业务状态码

| 业务代码 | 说明         | 类型 |
|----------|--------------|------|
| 20000    | 操作成功     |      |
| 40000**  | 参数校验失败 |      |
| 40100**  | 未登录       |      |
| 40300**  | 权限不足     |      |
| 40400**  | 资源不存在   |      |
| 50000**  | 服务器异常   |      |

# 7. 公共请求参数

| 类型       | 名称                          | 说明                       | 类型   | 默认值 |
|------------|-------------------------------|----------------------------|--------|--------|
| **Header** | **Authorization**  <br>*可选* | SDK中 acquireDataToken获取 | string |        |

## 7.1. 请求示例

```java
Platform client = new PlatformClient(API_GATEWAY, APP_ID, APP_SECRET, APP_PRIVATE_KEY, APP_PUBLIC_KEY, PLATFORM_PUBLIC_KEY);

        //封装请求参数
        BaiBaoOauthTokenRequest dataRequest = BaiBaoOauthTokenRequest.builder()
                .tenantCode(APP_ID)
                .appId(APP_ID)
                .appSecret(APP_SECRET)
                .build();

        //请求数据token
        BaiBaoResponse result = client.acquireDataToken(dataRequest);
        if (result.isSuccess()) {
            System.out.println(JSON.toJSONString(result.getData()));
        } else {
            throw new RuntimeException("获取Token失败" + result.getMsg());
        }
```

## 7.2. 响应 200

```json
{
  "code" : 20000,
  "data" : {
    "accessToken" : "ZXlKaGJHY2lPaUpJVXpJMU5pSXNJblI1Y0NJNklrcFhWQ0o5LmV5SmxlSEFpT2pFMk1qa3hPVE01TlRRc0luWmxjbk5wYjI0aU9pSXlMakFpTENKMWMyVnlYMjVoYldVaU9pSk5XVUZRVURBd01EQXdNQ0lzSW1wMGFTSTZJalE0WW1JNE5XVTRMVFZrWWpJdE5HSXlNUzFpWVdVekxUYzNPR0l4TmpBME9EbGlZeUlzSW1Oc2FXVnVkRjlwWkNJNklrMVpRVkJRTURBd01EQXdJaXdpYzJOdmNHVWlPbHNpZEdWdVlXNTBJbDE5LldmUDJpSi0teUFqOTBhR0hBclBjb1FCMEprUkhINjBqaXY1aVBYZWtzY0U=",
    "expiresIn" : "3600"
  },
  "msg" : "成功",
  "success" : true,
  "trace" : "string"
}
```

---

# 8. 接口列表

## 8.1. 保单托管

### 8.1.1. 明细数据

```js
GET /data/report/details?buzDate=20210101
```

#### 8.1.1.1. 描述

> 获取保单托管明细数据

#### 8.1.1.2. request

| 请求类型  | 名称                   | 说明     | 数据类型 | 默认值 |
|-----------|------------------------|----------|----------|--------|
| **query** | **buzDate** <br>*必填* | 业务日期 | String   |        |

##### 8.1.1.2.1. HTTP请求示例

```js

```

#### 8.1.1.3. response

| 名称                                | 说明         | 数据类型 | 备注                             |
|-------------------------------------|--------------|----------|----------------------------------|
| familyCode                          | 家庭编码     | String   |                                  |
| familyTitle                         | 标题         | String   |                                  |
| gmtCreate                           | 创建时间     | String   |                                  |
| tenantUserCode                      | 代理人编码   | String   |                                  |
| tenantUserName                      | 代理人姓名   | String   |                                  |
| tenantUserMobile                    | 代理人手机号 | String   |                                  |
| members                             | 家庭成员信息 | Object[] |                                  |
| members.relationType                | 家庭关系     | string   |                                  |
| members.name                        | 姓名         | string   |                                  |
| members.sex                         | 性别         | string   | 男性 女性                        |
| members.birthday                    | 生日         | string   | yyyy-MM-dd                       |
| members.certificateType             | 证件类型     | string   |                                  |
| members.certificate                 | 证件号       | string   |                                  |
| reports                             | 报告列表     | Object[] |                                  |
| reports.gmtCreate                   | 生成时间     | string   |                                  |
| reports.url                         | 报告链接     | string   |                                  |
| policies                            | 保单信息     | Object[] |                                  |
| policies.policyCode                 | 保单号       | string   |                                  |
| policies.company                    | 保险公司     | string   |                                  |
| policies.gmtCreate                  | 创建时间     | string   |                                  |
| policies.gmtModified                | 更新时间     | String   |                                  |
| policies.gmtProcessed               | 处理时间     | string   |                                  |
| policies.state                      | 处理状态     | string   |                                  |
| policies.effectDate                 | 保单生效日   | string   |                                  |
| policies.holdeName                  | 投保人       | string   |                                  |
| policies.benes                      | 受益人       | Object[] | 为空时表示法定受益人             |
| policies.benes.name                 | 受益人姓名   | String   |                                  |
| policies.benes.sex                  | 受益人性别   | String   | 男性 女性                        |
| policies.benes.birthday             | 受益人生日   | String   |                                  |
| policies.benes.ratio                | 受益比例     | String   |                                  |
| policies.benes.order                | 受益顺序     | String   | 1-第一顺位 2-第二顺位 3-第三顺位 |
| policies.products                   | 保单险种     | Object[] |                                  |
| policies.products.productName       | 险种名称     | String   |                                  |
| policies.products.main              | 主附险标记   | String   |                                  |
| policies.products.effectDate        | 险种生效日   | String   |                                  |
| policies.products.amount            | 保额         | String   |                                  |
| policies.products.coverageYear      | 保险期间     | String   |                                  |
| policies.products.chargeYear        | 缴费期间     | String   |                                  |
| policies.products.chargeMode        | 缴费方式     | String   |                                  |
| policies.products.prem              | 保费         | String   |                                  |
| policies.products.receiveAge        | 领取年龄     | String   |                                  |
| policies.products.deductible        | 免赔额       | String   |                                  |
| policies.products.productType       | 险种类型     | String   |                                  |
| policies.products.insureds          | 被保人       | Object[] |                                  |
| policies.products.insureds.name     | 被保人姓名   | String   |                                  |
| policies.products.insureds.sex      | 被保人性别   | String   | 男性 女性                        |
| policies.products.insureds.birthday | 被保人生日   | String   |                                  |

##### 8.1.1.3.1. HTTP响应示例

###### 8.1.1.3.1.1. 响应 200

```json
{
    "code":20000,
    "data":{
        "familyCode":"F0019293192",
        "familyTitle":"张三的家庭保单",
        "gmtCreate":"2019-08-05 22:33:43",
        "tenantUserCode":"123",
        "tenantUserName":"张三",
        "tenantUserMobile":"110",
        "members":[
            {
                "relationType":"本人",
                "name":"张三",
                "sex":"男性",
                "birthday":"1999-01-01",
                "certificateType":"身份证",
                "certificate":"110110199901010101"
            },
            {
                "relationType":"夫妻",
                "name":"张三",
                "sex":"男性",
                "birthday":"1999-01-01",
                "certificateType":"110110199901010101"
            }
        ],
        "reports":[
            {
                "gmtCreate":"2021-01-01",
                "url":"https://**.com"
            }
        ],
        "policies":[
            {
                "policyCode":"1111000",
                "company":"中国人寿",
                "gmtCreate":"2019-08-05 22:33:43",
                "gmtProcessed":"2019-08-05 22:33:43",
                "gmtModified":"2019-08-05 22:33:43",
                "state":"2",
                "effectDate":"2019-08-05",
                "holdeName":"张三",
                "benes":[
                    {
                        "name":"张三",
                        "sex":"男性",
                        "birthday":"1999-01-01",
                        "ratio":"100",
                        "order":"1"
                    }
                ],
                "products":[
                    {
                        "productName":"恒安标准臻爱倍护重大疾病保险（B款）",
                        "main":1,
                        "effectDate":"2019-08-05",
                        "amount":"150000",
                        "coverageYear":"终身",
                        "chargeYear":"20年",
                        "chargeMode":"年交",
                        "prem":"12321",
                        "receiveAge":"11",
                        "deductible":"123",
                        "productType":"年金",
                        "insureds":[
                            {
                                "name":"张三",
                                "sex":"男性",
                                "birthday":"1999-01-01"
                            }
                        ]
                    }
                ]
            },
            {
                "policyCode":"1111000",
                "company":"中国人寿",
                "gmtCreate":"2019-08-05 22:33:43",
                "gmtProcessed":"2019-08-05 22:33:43",
                "state":"2",
                "effectDate":"2019-08-05",
                "holderName":"张三",
                "products":[
                    {
                        "productName":"恒安标准臻爱倍护重大疾病保险（B款）",
                        "main":1,
                        "effectDate":"2019-08-05",
                        "amount":"150000",
                        "coverageYear":"终身",
                        "chargeYear":"20年",
                        "chargeMode":"年交",
                        "prem":"12321",
                        "receiveAge":"11",
                        "deductible":"123",
                        "productType":"年金",
                        "insured":[
                            {
                                "name":"张三",
                                "sex":"男性",
                                "birthday":"1999-01-01"
                            }
                        ]
                    }
                ]
            }
        ]
    },
    "msg":"成功",
    "success":true,
    "trace":"string"
}
```

### 8.1.2. 统计数据

```js
GET /data/report/statistics?buzDate=20210101
```

#### 8.1.2.1. 描述

> 获取保单托管统计数据

#### 8.1.2.2. request

| 请求类型  | 名称                    | 说明     | 数据类型 | 默认值 |
|-----------|-------------------------|----------|----------|--------|
| **query** | ** buzDate** <br>*必填* | 业务日期 | String   |        |

##### 8.1.2.2.1. HTTP请求示例

```js

```

#### 8.1.2.3. response

| 名称              | 说明           | 数据类型 | 备注 |
|-------------------|----------------|----------|------|
| h5view            | h5访问量       | String   |      |
| pdf               | pdf报告数量    | String   |      |
| excel             | Excel生成数量  | String   |      |
| details           | 代理人统计详情 | Object[] |      |
| details.agentCode | 代理人编码     | String   |      |
| details.h5view    | h5访问量       | String   |      |
| details.pdf       | pdf报告数量    | String   |      |
| details.excel     | Excel生成数量  | String   |      |

##### 8.1.2.3.1. HTTP响应示例

###### 8.1.2.3.1.1. 响应 200

```json
{
    "code":20000,
    "data":{
        "h5view":"123",
        "pdf":"123",
        "excel":"123",
        "details":[
            {
                "agentCode":"zhangsan",
                "h5view":"123",
                "pdf":"123",
                "excel":"123"
            }
        ]
    },
    "msg":"成功",
    "success":true,
    "trace":"string"
}
```

---

## 8.2. 产品对比

### 8.2.1. 明细数据

```js
GET /data/compare/details?buzDate=20210101
```

#### 8.2.1.1. 描述

> 获取产品对比明细数据

#### 8.2.1.2. request

| 请求类型  | 名称                    | 说明     | 数据类型 | 默认值 |
|-----------|-------------------------|----------|----------|--------|
| **query** | ** buzDate** <br>*必填* | 业务日期 | String   |        |

##### 8.2.1.2.1. HTTP请求示例

```js

```

#### 8.2.1.3. response

| 名称                 | 说明         | 数据类型 | 备注 |
|----------------------|--------------|----------|------|
| tenantUserCode       | 代理人编码   | String   |      |
| tenantUserName       | 代理人姓名   | String   |      |
| tenantUserMobile     | 代理人手机号 | String   |      |
| gmtCompare           | 对比时间     | String   |      |
| compares             | 对比详情     | Object[] |      |
| compares.productType | 产品类型     | string   |      |
| compares.productName | 产品名称     | string   |      |

##### 8.2.1.3.1. HTTP响应示例

###### 8.2.1.3.1.1. 响应 200

```json
{
    "code":20000,
    "data":[
        {
            "tenantUserCode":"123",
            "tenantUserName":"张三",
            "tenantUserMobile":"110",
            "gmtCompare":"2021-08-16 10:33:06",
            "compares":[
                {
                    "productType":"重疾",
                    "productName":"相伴一生年金保险"
                },
                {
                    "productType":"重疾",
                    "productName":"相伴一生年金保险"
                }
            ]
        }
    ],
    "msg":"成功",
    "success":true,
    "trace":"string"
}
```

### 8.2.2. 统计数据

```js
GET /data/compare/statistics?buzDate=20210101
```

#### 8.2.2.1. 描述

> 获取产品对比统计数据

#### 8.2.2.2. request

| 请求类型  | 名称                    | 说明     | 数据类型 | 默认值 |
|-----------|-------------------------|----------|----------|--------|
| **query** | ** buzDate** <br>*必填* | 业务日期 | String   |        |

##### 8.2.2.2.1. HTTP请求示例

```js

```

#### 8.2.2.3. response

| 名称              | 说明           | 数据类型 | 备注 |
|-------------------|----------------|----------|------|
| h5                | h5分享数量     | String   |      |
| h5view            | h5浏览数量     | String   |      |
| excel             | Excel生成数量  | String   |      |
| details           | 代理人统计详情 | Object[] |      |
| details.agentCode | 代理人编码     | String   |      |
| details.excel     | h5访问量       | String   |      |
| details.h5        | pdf报告数量    | String   |      |
| details.h5view    | Excel生成数量  | String   |      |

##### 8.2.2.3.1. HTTP响应示例

###### 8.2.2.3.1.1. 响应 200

```json
{
    "code":20000,
    "data":{
        "excel":"生成Excel数量",
        "h5":"12",
        "h5view":"110",
        "details":[
            {
                "agentCode":"zhangsan",
                "excel":"生成Excel数量",
                "h5":"12",
                "h5view":"110"
            }
        ]
    },
    "msg":"成功",
    "success":true,
    "trace":"string"
}
```

---

## 8.3. 单品计划书

### 8.3.1. 明细数据

```js
GET /data/singlePlan/details?buzDate=20210101
```

#### 8.3.1.1. 描述

> 获取单品计划书明细数据

#### 8.3.1.2. request

| 请求类型  | 名称                    | 说明     | 数据类型 | 默认值 |
|-----------|-------------------------|----------|----------|--------|
| **query** | ** buzDate** <br>*必填* | 业务日期 | String   |        |

##### 8.3.1.2.1. HTTP请求示例

```js

```

#### 8.3.1.3. response

| 名称                            | 说明           | 数据类型 | 备注      |
|---------------------------------|----------------|----------|-----------|
| planProgramCode                 | 单品计划书编码 | String   |           |
| tenantUserCode                  | 代理人编码     | String   |           |
| tenantUserName                  | 代理人姓名     | String   |           |
| tenantUserMobile                | 代理人手机号   | String   |           |
| gmtCreate                       | 创建时间       | String   |           |
| gmtModified                     | 更新时间       | String   |           |
| insured                         | 被保人信息     | Object   |           |
| insured.name                    | 姓名           | string   |           |
| insured.sex                     | 性别           | string   | 男性 女性 |
| insured.age                     | 年龄           | string   |           |
| portfilio                       | 组合信息       | Object[] |           |
| portfilio.portfilioName         | 组合名称       | string   |           |
| portfilio.products              | 保单险种       | Object[] |           |
| portfilio.products.productName  | 险种名称       | String   |           |
| portfilio.products.main         | 主附险标记     | String   |           |
| portfilio.products.amount       | 保额           | String   |           |
| portfilio.products.coverageYear | 保险期间       | String   |           |
| portfilio.products.chargeYear   | 缴费期间       | String   |           |
| portfilio.products.prem         | 保费           | String   |           |
| portfilio.products.productType  | 险种类型       | String   |           |

##### 8.3.1.3.1. HTTP响应示例

###### 8.3.1.3.1.1. 响应 200

```json
{
    "code":20000,
    "data":[
        {
            "planProgramCode":"PN405045817808781312",
            "tenantUserCode":"123",
            "tenantUserName":"张三",
            "tenantUserMobile":"110",
            "gmtCreate":"2021-01-01 22:22:22",
            "gmtModified":"2021-01-01 22:22:22",
            "insured":{
                "name":"张三",
                "sex":"男性",
                "age":"19"
            },
            "portfilio":{
                "portfilioName":"康健一生智尊保",
                "products":[
                    {
                        "productName":"恒安标准臻爱倍护重大疾病保险（B款）",
                        "main":1,
                        "amount":"150000",
                        "coverageYear":"终身",
                        "chargeYear":"20年",
                        "prem":"12321",
                        "productType":"年金"
                    }
                ]
            }
        }
    ],
    "msg":"成功",
    "success":true,
    "trace":"string"
}
```

### 8.3.2. 统计数据

```js
GET /data/singlePlan/statistics?buzDate=20210101
```

#### 8.3.2.1. 描述

> 获取单品计划书统计数据

#### 8.3.2.2. request

| 请求类型  | 名称                    | 说明     | 数据类型 | 默认值 |
|-----------|-------------------------|----------|----------|--------|
| **query** | ** buzDate** <br>*必填* | 业务日期 | String   |        |

##### 8.3.2.2.1. HTTP请求示例

```js

```

#### 8.3.2.3. response

| 名称           | 说明           | 数据类型 | 备注 |
|----------------|----------------|----------|------|
| h5view         | h5浏览数量     | String   |      |
| details        | 代理人统计详情 | Object[] |      |
| details.h5view | h5浏览数量     | String   |      |

##### 8.3.2.3.1. HTTP响应示例

###### 8.3.2.3.1.1. 响应 200

```json
{
    "code":20000,
    "data":[
        {
            "h5view":"110",
            "details":[
                {
                    "agentCode":"zhangsan",
                    "h5view":"110"
                }
            ]
        }
    ],
    "msg":"成功",
    "success":true,
    "trace":"string"
}
```

---

## 8.4. 家庭计划书

### 8.4.1. 明细数据

```js
GET /data/plan/details?buzDate=20210101
```

#### 8.4.1.1. 描述

> 获取家庭计划书明细数据

#### 8.4.1.2. request

| 请求类型  | 名称                    | 说明     | 数据类型 | 默认值 |
|-----------|-------------------------|----------|----------|--------|
| **query** | ** buzDate** <br>*必填* | 业务日期 | String   |        |

##### 8.4.1.2.1. HTTP请求示例

```js

```

#### 8.4.1.3. response

| 名称                                    | 说明         | 数据类型 | 备注      |
|-----------------------------------------|--------------|----------|-----------|
| tenantUserCode                          | 代理人编码   | String   |           |
| tenantUserName                          | 代理人姓名   | String   |           |
| tenantUserMobile                        | 代理人手机号 | String   |           |
| planProgramCode                         | 编码         | String   |           |
| planProgramTitle                        | 标题         | String   |           |
| gmtCreate                               | 创建时间     | String   |           |
| gmtModified                             | 更新时间     | String   |           |
| members                                 | 家庭成员     | Object[] |           |
| members.relationType                    | 关系         | string   |           |
| members.name                            | 姓名         | string   |           |
| members.sex                             | 性别         | string   | 男性 女性 |
| members.age                             | 年龄         | string   |           |
| members.portfilio                       | 组合信息     | Object[] |           |
| members.portfilio.portfilioName         | 组合名称     | string   |           |
| members.portfilio.products              | 保单险种     | Object[] |           |
| members.portfilio.products.productName  | 险种名称     | String   |           |
| members.portfilio.products.main         | 主附险标记   | String   |           |
| members.portfilio.products.amount       | 保额         | String   |           |
| members.portfilio.products.coverageYear | 保险期间     | String   |           |
| members.portfilio.products.chargeYear   | 缴费期间     | String   |           |
| members.portfilio.products.prem         | 保费         | String   |           |
| members.portfilio.products.productType  | 险种类型     | String   |           |

##### 8.4.1.3.1. HTTP响应示例

###### 8.4.1.3.1.1. 响应 200

```json
{
    "code":20000,
    "data":[
        {
            "tenantUserCode":"123",
            "tenantUserName":"张三",
            "tenantUserMobile":"110",
            "planProgramCode":"PN339143806295212032",
            "planProgramTitle":"张三123",
            "gmtCreate":"2019-08-05 22:33:43",
            "gmtModified":"2019-08-05 22:33:43",
            "members":[
                {
                    "relationType":"本人",
                    "name":"张三",
                    "sex":"男性",
                    "age":"19",
                    "portfilio":[
                        {
                            "portfilioName":"康健一生智尊保",
                            "products":[
                                {
                                    "productName":"恒安标准臻爱倍护重大疾病保险（B款）",
                                    "main":1,
                                    "amount":"150000",
                                    "coverageYear":"终身",
                                    "chargeYear":"20年",
                                    "prem":"12321",
                                    "productType":"险种类型"
                                }
                            ]
                        }
                    ]
                }
            ]
        }
    ],
    "msg":"成功",
    "success":true,
    "trace":"string"
}
```

### 8.4.2. 统计数据

```js
GET /data/plan/statistics?buzDate=20210101
```

#### 8.4.2.1. 描述

> 获取家庭计划书统计数据

#### 8.4.2.2. request

| 请求类型  | 名称                    | 说明     | 数据类型 | 默认值 |
|-----------|-------------------------|----------|----------|--------|
| **query** | ** buzDate** <br>*必填* | 业务日期 | String   |        |

##### 8.4.2.2.1. HTTP请求示例

```js

```

#### 8.4.2.3. response

| 名称            | 说明           | 数据类型 | 备注 |
|-----------------|----------------|----------|------|
| h5view          | h5浏览数量     | String   |      |
| pdf             | pdf生成数量    | String   |      |
| mindMap         | 脑图生成数量   | String   |      |
| details         | 代理人统计详情 | Object[] |      |
| details.h5view  | h5浏览数量     | String   |      |
| details.pdf     | pdf生成数量    | String   |      |
| details.mindMap | 脑图生成数量   | String   |      |

##### 8.4.2.3.1. HTTP响应示例

###### 8.4.2.3.1.1. 响应 200

```json
{
    "code":20000,
    "data":[
        {
            "h5view":"110",
            "pdf":"110",
            "mindMap":"110",
            "details":[
                {
                    "agentCode":"zhangsan",
                    "h5view":"110",
                    "pdf":"110",
                    "mindMap":"110"
                }
            ]
        }
    ],
    "msg":"成功",
    "success":true,
    "trace":"string"
}
```

---

## 8.5. 保单置换

### 8.5.1. 明细数据

```js
GET /data/exchange/details?buzDate=20210101
```

#### 8.5.1.1. 描述

> 获取保单置换明细数据

#### 8.5.1.2. request

| 请求类型  | 名称                    | 说明     | 数据类型 | 默认值 |
|-----------|-------------------------|----------|----------|--------|
| **query** | ** buzDate** <br>*必填* | 业务日期 | String   |        |

##### 8.5.1.2.1. HTTP请求示例

```js

```

#### 8.5.1.3. response

| 名称                              | 说明         | 数据类型 | 备注                             |
|-----------------------------------|--------------|----------|----------------------------------|
| tenantUserCode                    | 代理人编码   | String   |                                  |
| exchangeCode                      | 置换编码     | String   |                                  |
| tenantUserName                    | 代理人姓名   | String   |                                  |
| tenantUserMobile                  | 代理人手机号 | String   |                                  |
| gmtChanageCreate                  | 置换时间     | String   |                                  |
| policy                            | 保单信息     | Object   |                                  |
| policy.policyCode                 | 保单号       | string   |                                  |
| policy.company                    | 保险公司     | string   |                                  |
| policy.gmtCreate                  | 创建时间     | string   |                                  |
| policy.gmtProcessed               | 处理时间     | string   |                                  |
| policy.gmtModified                | 更新时间     | string   |                                  |
| policy.state                      | 处理状态     | string   |                                  |
| policy.effectDate                 | 保单生效日   | string   |                                  |
| policy.holdeName                  | 投保人       | string   |                                  |
| policy.benes                      | 受益人       | Object[] | 为空时表示法定受益人             |
| policy.benes.name                 | 受益人姓名   | String   |                                  |
| policy.benes.sex                  | 受益人性别   | String   | 男性 女性                        |
| policy.benes.birthday             | 受益人生日   | String   |                                  |
| policy.benes.ratio                | 受益比例     | String   |                                  |
| policy.benes.order                | 受益顺序     | String   | 1-第一顺位 2-第二顺位 3-第三顺位 |
| policy.products                   | 保单险种     | Object[] |                                  |
| policy.products.productName       | 险种名称     | String   |                                  |
| policy.products.main              | 主附险标记   | String   |                                  |
| policy.products.effectDate        | 险种生效日   | String   |                                  |
| policy.products.amount            | 保额         | String   |                                  |
| policy.products.coverageYear      | 保险期间     | String   |                                  |
| policy.products.chargeYear        | 缴费期间     | String   |                                  |
| policy.products.chargeMode        | 缴费方式     | String   |                                  |
| policy.products.prem              | 保费         | String   |                                  |
| policy.products.receiveAge        | 领取年龄     | String   |                                  |
| policy.products.deductible        | 免赔额       | String   |                                  |
| policy.products.productType       | 险种类型     | String   |                                  |
| policy.products.insureds          | 被保人       | Object[] |                                  |
| policy.products.insureds.name     | 被保人姓名   | String   |                                  |
| policy.products.insureds.sex      | 被保人性别   | String   | 男性 女性                        |
| policy.products.insureds.birthday | 被保人生日   | String   |                                  |
| portfilio                         | 组合信息     | Object   |                                  |
| portfilio.portfilioName           | 组合名称     | string   |                                  |
| portfilio.products                | 保单险种     | Object[] |                                  |
| portfilio.products.productName    | 险种名称     | String   |                                  |
| portfilio.products.main           | 主附险标记   | String   |                                  |
| portfilio.products.amount         | 保额         | String   |                                  |
| portfilio.products.coverageYear   | 保险期间     | String   |                                  |
| portfilio.products.chargeYear     | 缴费期间     | String   |                                  |
| portfilio.products.prem           | 保费         | String   |                                  |

##### 8.5.1.3.1. HTTP响应示例

###### 8.5.1.3.1.1. 响应 200

```json
{
    "code":20000,
    "data":{
        "tenantUserCode":"123",
        "tenantUserName":"张三",
        "tenantUserMobile":"110",
        "exchangeCode":"EC123213323",
        "gmtChanageCreate":"2021-01-01 22:22:22",
        "policy":{
            "policyCode":"1111000",
            "company":"中国人寿",
            "gmtCreate":"2019-08-05 22:33:43",
            "gmtProcessed":"2019-08-05 22:33:43",
            "gmtModified":"2019-08-05 22:33:43",
            "state":"2",
            "effectDate":"2019-08-05",
            "holdeName":"张三",
            "benes":[
                {
                    "name":"张三",
                    "sex":"男性",
                    "age":"19",
                    "ratio":"100",
                    "order":"1"
                }
            ],
            "products":[
                {
                    "productName":"恒安标准臻爱倍护重大疾病保险（B款）",
                    "main":1,
                    "effectDate":"2019-08-05",
                    "amount":"150000",
                    "coverageYear":"终身",
                    "chargeYear":"20年",
                    "chargeMode":"年交",
                    "prem":"12321",
                    "receiveAge":"11",
                    "deductible":"123",
                    "productType":"重疾",
                    "insureds":[
                        {
                            "name":"张三",
                            "sex":"男性",
                            "birthday":"1999-01-01"
                        }
                    ]
                }
            ]
        },
        "portfilio":{
            "portfilioName":"康健一生智尊保",
            "products":[
                {
                    "productName":"恒安标准臻爱倍护重大疾病保险（B款）",
                    "main":1,
                    "amount":"150000",
                    "coverageYear":"终身",
                    "chargeYear":"20年",
                    "prem":"12321"
                }
            ]
        }
    },
    "msg":"成功",
    "success":true,
    "trace":"string"
}
```

### 8.5.2. 统计数据

> 暂无

---

# 9. 相关字典

## 9.1. 家庭成员关系

> 本人<br>
> 配偶<br>
> 父母<br>
> 子女<br>
> 其他<br>

## 9.2. 证件类型

> 身份证<br>
> 临时身份证<br>
> 其他<br>
> 军官证<br>
> 出生证<br>
> 台湾居住证<br>
> 台湾通行证<br>
> 士兵证<br>
> 外国人永居身份证<br>
> 护照<br>
> 护照号<br>
> 港台护照<br>
> 港澳回乡证<br>
> 港澳通行证<br>
> 警官证<br>

## 9.3. 产品类型

> 医疗<br>
> 年金<br>
> 重疾<br>
> 意外<br>
> 两全<br>
> 终寿定寿<br>
> 终寿<br>
> 定寿<br>
> 增额终寿<br>
> 增额终身寿险<br>
> 增额定期寿险<br>
> 增额定寿<br>
> 减额定寿<br>
> 中高端医疗<br>
> 次中端医疗<br>
> 普通住院<br>
> 门诊医疗<br>
> 生育保险<br>
> 海外医疗<br>
> 意外医疗<br>
> 防癌医疗<br>
> 养老年金<br>
> 普通年金<br>
> 万能险<br>
> 储蓄险<br>
> 投连险<br>
> 短期意外<br>
> 长期意外<br>
> 普通重疾<br>
> 少儿重疾<br>
> 防癌保险<br>
> 男性防癌<br>
> 女性防癌<br>
> 老年防癌<br>
> 一年期重疾<br>
> 一年期防癌<br>
> 护理保险<br>
> 特定疾病<br>
> 投保人豁免<br>
> 被保人豁免<br>

## 9.4. 保单状态
> 0：未受理
> 1：暂存
> 2：成功
> -1：补充资料

&copy; **百保科技**
