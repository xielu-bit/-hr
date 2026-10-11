# 招聘复盘官 · AI 简历画像与标准反哺工具

> 让招聘标准从"凭手感"变成"有数据依据的闭环"。
> 历史简历（带筛选结果）→ AI 特征抽取 → 通过/未通过对比画像 → 反哺 JD 与筛选标准 → 回测验证。

## ⚡ 一键体验（无需任何配置）
应用内置 **60 份虚构简历** 及预抽取特征：
1. 点击「加载演示数据集」
2. 在「② 特征抽取」点「使用预抽取结果」
3. 依次查看画像对比 / 反哺 JD / 回测验证

## 🔑 实时 AI 模式
在左侧栏填入 DeepSeek API Key（platform.deepseek.com 申请，充值约 10-20 元可用很久），
即可体验 AI 实时抽取与生成。也可部署后在 Streamlit Cloud 的 Secrets 中配置 `DEEPSEEK_API_KEY`。

## ☁️ 部署到 Streamlit Cloud（免费，得到公开链接）
1. 注册 GitHub → 新建仓库（如 `recruit-review`）→ 上传本目录 4 个文件
   （app.py、demo_data.json、requirements.txt、README.md）
2. 打开 share.streamlit.io → 用 GitHub 登录 → 「New app」
3. 选择刚建的仓库，分支 main，主文件 app.py → Deploy
4. 约 2 分钟得到一个公开访问链接（可设置访问密码）

## 📁 文件说明
| 文件 | 说明 |
|---|---|
| app.py | 主程序（Streamlit 应用，含全部业务逻辑与提示词） |
| demo_data.json | 60 份虚构简历 + 预抽取特征 + 示例文案 |
| requirements.txt | Python 依赖 |

## ⚠️ 数据合规声明
演示数据全部为 AI 虚构：公司名、人名、电话、邮箱均为编造，不指向任何真实个人或企业。
工具设计上显式排除性别、年龄等敏感属性；AI 输出仅为辅助参考，最终招聘决策权在人。
