
<div align="center">

<image src="http://m.qpic.cn/psc?/V51UyG6T2hLdbN0oEgHl3fEkH73KqJt7/TmEUgtj9EK6.7V8ajmQrEEsEylM*52lTktZHLze*PTbMCd2wg4o5kkEyKNVsVL9UM5xK4GLClF.TOL*ty*FnqAuxBQmobbAoJ.gYMo62EQY!/mnull&bo=wADAAAAAAAADByI!&rf=photolist&t=5" height="64"/>

# UCSF

通用的课程表格式

[**English**](../../README.md) | **中文简体**

</div>

## 简介

UCSF 是一种通用的课程表格式，用于描述课程表。它被设计为简单易用，可以轻松转换为其他格式，如 ClassIsland 格式。

## 特点

- **简单**: UCSF 被设计为简单易用。
- **通用**: UCSF 是一种通用格式，可以轻松转换为其他格式。
- **易用**: UCSF 易于使用，可以轻松被人类理解。

## 示例

```yaml
version: 1
subjects:
  - name: 数学
    simplified_name: 数 # 可选，适合中文科目名，ClassIsland 等紧凑课程表软件一般需要
    teacher: 李梅 # 可选
    room: 101 # 可选
  - name: 语文
    simplified_name: 语
    teacher: 王芳
    room: 102
  - name: 英语
    simplified_name: 英
    teacher: 张伟
    room: 103
  - name: 物理
    simplified_name: 物
    teacher: 赵军
    room: 104

schedules:
  - name: 星期一
    enable_day: mon
    weeks: all
    classes:
      - subject: 数学
        start_time: 8:00
        end_time: 9:00
      - subject: 语文
        start_time: 9:00
        end_time: 10:00
  - name: 星期二-单周
    enable_day: tue
    weeks: odd
    classes:
      - subject: 物理
        start_time: 8:00
        end_time: 9:00
      - subject: 英语
        start_time: 9:00
        end_time: 10:00
  - name: 星期二-双周
    enable_day: tue
    weeks: even
    classes:
      - subject: 物理
        start_time: 8:00
        end_time: 9:00
      - subject: 英语
        start_time: 9:00
        end_time: 10:00
```

## 协议

[MIT](./LICENSE)

