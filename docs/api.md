# 学习API（需要 {==刘兴平==} 提供内容）

## API


**简要描述：** 

- 人员历史轨迹查询

**请求URL：** 
- ` http://xx.com/track/list  `
  
**请求方式：**
- POST 

**参数：** 

|参数名|必选|类型|说明|
|:----    |:---|:----- |-----   |
|name     |否  |string | 人员姓名    |
|number     |否  |string | 工号  |
|staff_id  |否  |int | 人员id,name,number,staff_id至少有一个不为空  |
|starttime     |否  |int | 开始时间 （时间戳） |
|endtime     |否  |int | 结束时间  |

 **返回示例**
 

 ``` 
{
    "code": 0,
    "msg": "操作成功",
    "result": [
        {
            "place_id": 186,
            "data": [
                {
                    "name": "张三",
                    "number": "1076005",
                    "team": "PD",
                    "staff_id": "450",
                    "x": "34.4",
                    "y": "22.9",
                    "region_id": "441",
                    "device_id": "1115",
                    "mac": "12B5",
                    "region_name": "小会议室",
                    "type": "2",
                    "status": "1",
                    "time": "2019-11-07 07:20:38"
                }
            ]
        }
    ]
}

 ```

 **返回参数说明** 

|参数名|类型|说明|
|:-----  |:-----|-----|
|code |int   |0:操作成功；2：数据库操作失败 |
|mac |string   | 信标mac值 |
|time |string   | 时间 |
|staff_id |string   | 人员id |
|name |string   | 人员姓名 |
|number |string   | 工号 |
|region_id |string   | 区域id |
|region_name |string   | 区域名称 |
|place_id |string   | 车间id |
|team |string   | 班组名称 |
|status |string   | 状态 |
|type |string   | 区域类型，1工作区，2非工作区 |



{==刘兴平==}可以参考使用 [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) 的其他网站来设计PDC的API培训内容:

```console
https://interactive.davischallenge.org/docs/session/
```

```console
https://doc.botsquad.com/dev/rest/#/
```

## 购买套件

如果您打算进行二次开发，而且需要“硬件”来发送数据至服务器，例如：

* 蓝牙定位标签
* 定位微基站
* LoRa网关

您可以[联系我们](./contact.md)购买和获取技术支持





