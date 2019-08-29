<center><img src="media/eye.jpg" width=250 height=250 /></center>
<center><h1>EXIF-Finder</h1></center>

这是一个用于检索出相册中留存有GPS定位信息图像的工具，且用法很简单。只需要输入如下命令即可

```bash
python3 run.py -t [path]
```

如果您需要(-l 参数)或许定位地区的中文名称，您就需要提前到`restapi.amap.com`站点申请一个自己的`key`并填入`conf.py`中。


### 参数说明:

- `-t`: 指定相册地址【必要参数】
- `-s`: 指定图片存储文件夹名
- `-l`: 开启地理定位附近位置查询功能
- `-a`: 开启地图投影功能，默认添加图片存储地址为`image`
- `--dark`: 开启暗黑地图模式
- `--locus`: 开启标点轨迹【依据时间排布】


### 结果案例:

```json
[
    {
        "path": "../screen_shot/21012_1.png",
        "GPSAltitude": "距海平面25.05米",
        "Make": "Apple",
        "Model": "iPhone 4",
        "Software": "Adobe Photoshop CS5 Windows",
        "GPS": [
            31.224166666666665,
            121.49383333333333
        ],
        "Dates": "2013:10:11 10:33:18",
        "address": "上海市黄浦区豫园街道光启路74傅家街幼儿园(傅家街)"
    },
    {
        "path": "../screen_shot/21012_2.png",
        "GPSAltitude": "距海平面25.05米",
        "Make": "Apple",
        "Model": "iPhone 4",
        "Software": "Adobe Photoshop CS5 Windows",
        "GPS": [
            31.224166666666665,
            121.49383333333333
        ],
        "Dates": "2013:10:11 10:33:18",
        "address": "上海市黄浦区豫园街道光启路74傅家街幼儿园(傅家街)"
    },
    {
        "path": "../screen_shot/22323_0.png",
        "GPSAltitude": "距海平面14.61米",
        "Make": "Apple",
        "Model": "iPhone 6",
        "Software": "8.2",
        "GPS": [
            31.676894444444446,
            119.9347138888889
        ],
        "Dates": "2015:10:13 16:08:18",
        "address": "江苏省常州市武进区湖塘镇武宜中路98号"
    }
]

```

### 👯一次女装图集的分析结果

图集项目地址: [https://github.com/komeiji-satori/Dress](https://github.com/komeiji-satori/Dress)

![media/demo_map.png](media/demo_map.png)
