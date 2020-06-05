# API示例

## 历史轨迹API


**简要描述：** 

- 查询人员在一段时间内的历史轨迹

**请求URL：** 
- ` http://xx.com/track/list  `
  
**请求方式：**
- POST 

**参数：** 

|参数名|必选|类型|说明|
|:----    |:---|:----- |-----   |
|staff_id  |是  |int | 人员id |
|starttime     |是  |int | 开始时间 （时间戳） |
|endtime     |是  |int | 结束时间  |

**请求示例：**
- URL： http://xx.com/track/list 
- 参数： 

``` 
{
	staff_id: 1019，
	starttime: 1587603600，
	endtime: 1587604800，
}

```
- 数据返回：

```
{
  "code": 0,
  "msg": "操作成功",
  "result": [
    {
      "place_id": 232,
      "data": [
        {
          "name": "马静雯",
          "number": "1072856",
          "team": "PD",
          "staff_id": "1019",
          "x": "3844.0",
          "y": "2259.0",
          "region_id": null,
          "device_id": "1689",
          "mac": "12C4",
          "region_name": "未知区域",
          "type": "2",
          "status": "1",
          "time": "2020-04-23 09:01:16",
          "pick1x": null,
          "pick1y": null,
          "pick2x": null,
          "pick2y": null
        },
        {
          "name": "马静雯",
          "number": "1072856",
          "team": "PD",
          "staff_id": "1019",
          "x": "4425.0",
          "y": "2632.6",
          "region_id": null,
          "device_id": "1688",
          "mac": "12C4",
          "region_name": "未知区域",
          "type": "2",
          "status": "1",
          "time": "2020-04-23 09:02:00",
          "pick1x": null,
          "pick1y": null,
          "pick2x": null,
          "pick2y": null
        },
        {
          "name": "马静雯",
          "number": "1072856",
          "team": "PD",
          "staff_id": "1019",
          "x": "793.0",
          "y": "977.6",
          "region_id": null,
          "device_id": "1688",
          "mac": "12C4",
          "region_name": "未知区域",
          "type": "2",
          "status": "1",
          "time": "2020-04-23 09:02:26",
          "pick1x": null,
          "pick1y": null,
          "pick2x": null,
          "pick2y": null
        },
        {
          "name": "马静雯",
          "number": "1072856",
          "team": "PD",
          "staff_id": "1019",
          "x": "788.3",
          "y": "785.0",
          "region_id": null,
          "device_id": "1688",
          "mac": "12C4",
          "region_name": "未知区域",
          "type": "2",
          "status": "1",
          "time": "2020-04-23 09:07:36",
          "pick1x": null,
          "pick1y": null,
          "pick2x": null,
          "pick2y": null
        },
        {
          "name": "马静雯",
          "number": "1072856",
          "team": "PD",
          "staff_id": "1019",
          "x": "806.5",
          "y": "1555.3",
          "region_id": null,
          "device_id": "1689",
          "mac": "12C4",
          "region_name": "未知区域",
          "type": "2",
          "status": "1",
          "time": "2020-04-23 09:14:51",
          "pick1x": null,
          "pick1y": null,
          "pick2x": null,
          "pick2y": null
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
|pick1x |string   | 区域坐标x1 |
|pick1y |string   | 区域坐标y1 |
|pick2x |string   | 区域坐标x2 |
|pick2y |string   | 区域坐标y2 |


## 购买套件

如果您打算进行二次开发，而且需要“硬件”来发送数据至服务器，例如：

* 蓝牙定位标签
* 定位微基站
* LoRa网关

您可以[联系我们](./contact.md)购买和获取技术支持





