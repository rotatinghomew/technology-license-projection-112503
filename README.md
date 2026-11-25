# 显示工艺许可预测与部分签约复核

仓库维护技术转移办公室围绕应用市场的机会与权利资料。日期为台账基准后的整数日，日期字段 day 与来源登记日期 known_at 具有不同含义。

资料为合成输入。各来源文件的单位、标识及关联见 [资料字典](资料字典.md)。

## 检查资料

使用 Python 3.11。NumPy 与 SciPy 版本在依赖清单中固定。已有环境可直接执行资料检查。首次在本地使用时可以建立虚拟环境并安装依赖。

```sh
python3 -m venv .venv
. .venv/bin/activate
python3 -m pip install -r requirements.txt
python3 -m unittest discover -s tests -v
```

检查只读原始 JSON，报告编号、记录引用、相互关联的原始资料及运行环境是否可用。
