# 题目汇总

一个面向西医综合考研的开源刷题题库，支持多套独立试卷、单题作答、自动判题、错题/记录、收藏、编辑、新增和删除。

## 特点
- 多套试卷独立管理
- 生理 / 生化 / 病理 / 内科 / 外科 / 其他分类
- A型、B型、X型题
- 单题作答，提交后显示答案
- 本地保存做题记录与收藏
- 可编辑、新增、删除题目
- 可导出题库
- 纯前端，无需服务器和数据库
- 可直接部署到 GitHub Pages

## 本地运行
直接打开 `index.html` 即可使用。

## GitHub Pages
1. Fork 或上传本项目到 GitHub。
2. Settings → Pages。
3. 选择 `Deploy from a branch`。
4. Branch 选择 `main`，目录选择 `/root`。
5. 保存后等待部署。

## 如何添加新套卷
推荐将题目整理成 JSON 数据后，在 `index.html` 中接入新的题库数据。后续可以进一步将题库完全拆分到 `data/` 目录，实现无需修改核心代码即可导入。

## 题目数据格式
```json
{
  "id": "set-new-001",
  "setId": "set-new",
  "setName": "新套卷",
  "subject": "生理",
  "type": "A",
  "stem": "题干",
  "options": ["选项A", "选项B", "选项C", "选项D"],
  "answer": "B"
}
```

## 开源协议
MIT License
