# 大数据采集与处理实验

- 姓名：王永亮
- 学号：112404260117
- 班级：数据1241

## 仓库结构

```text
bigdata-collection-labs-112404260117/
├── README.md
├── .gitignore
└── lab01/
    ├── lab1_html_api.ipynb
    ├── REPORT.md
    ├── data/
    │   ├── companies.json
    │   └── devices.json
    └── images/
        ├── 01_device_api.png
        ├── 02_company_source.png
        ├── 03_company_next.png
        └── 04_validation.png
```

> `scripts/` 为本地辅助脚本，已通过 `.gitignore` 忽略，不随作业提交。

## Lab 1 实验一：静态页面与 API 数据采集

- 平台：SmartPark DataLab（https://115.159.159.82）
- 内容：
  - Device：动态加载 → 通过 `/api/devices` 分页采集全部 **5000** 台设备
  - Company：静态加载 → BeautifulSoup 解析 → "下一页"连续采集 **3 页共 60** 家企业
  - 结果验证：数量、主键唯一性、Company–Device 一致性（不一致企业数 = 0）
- 运行方式：在 `lab01/` 目录下打开 `lab1_html_api.ipynb`，`Restart Kernel → Run All`
