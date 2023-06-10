# Rubbish(MaoGai|MaYuan|ShiGang)

自动根据测试结果生成厦大 course.xmu.edu.cn 的题库

> **Note**
> 只要是**清华大学**course系统，并且所在课程的在线测试结果有公布答案，都可以使用该脚本生成题库

## 题目收集进度

- 马原题库：收集 **3800** 题，去重后 **430** 题

- 毛概题库：收集 **3569** 题，去重后 **383** 题

- 史纲题库：收集 **5240** 题，去重后 **855** 题

## 如何提供题目?

1. 完成6次测试，不用做直接提交即可
1. 点击查看结果，进入含有答案的结果页面
3. Ctrl+S分别保存6个测试结果网页
4. 将网页结果打包发送至作者，或者按照项目结构放入 samples 文件夹内，并发起 pull request

## 如何使用题库?

### 在线版（推荐）
1. 直接访问 [Github Pages](https://f5soft.github.io/RubbishMaoGai/)，这是部署好的在线版本
2. `Ctrl+F` 全文搜索
3. **全文搜索时，由于标点符号全半角、空格数量不匹配等问题，不建议复制整个标题搜索，可能会找不到结果！建议仅搜索题目标题的连续文字内容。**
4. **有的题目前面内容相同，但是后缀不同，注意搜索结果有多个的情况，以免看错！**
5. 如果你想保存页面，点击具体科目页面右侧题目列表上的打印机按钮即可

### 离线版
1. 参照 [如何使用该脚本生成其他题库](#如何使用该脚本生成其他题库) 部分生成题库，然后用 Markdown 阅读器打开
2. `Ctrl+F` 全文搜索
3. **全文搜索时，由于标点符号全半角、空格数量不匹配等问题，不建议复制整个标题搜索，可能会找不到结果！建议仅搜索题目标题的连续文字内容。**
4. **有的题目前面内容相同，但是后缀不同，注意搜索结果有多个的情况，以免看错！**

## 如何使用该脚本生成其他题库?

1. 操作同上，保存网页后，按照本仓库下samples文件夹的的结构，将测试结果放入samples文件夹

2. 在Python版本大于等于3.6.8的环境下运行`tiku.py`

   ```bash
   python tiku.py mg # 生成毛概题库
   python tiku.py my # 生成马原题库
   python tiku.py sg # 生成史纲题库
   ```
   > Linux下请使用`python3`

3. 检查 `src/banks` 文件夹下的 `xx.md`

## 致谢

[![Contributors](https://contributors-img.web.app/image?repo=F5Soft/RubbishMaoGai)](https://github.com/F5Soft/RubbishMaoGai/graphs/contributors)