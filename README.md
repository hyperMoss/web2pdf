# web2pdf

use python transfer web doc to pdf

改写自[为了保存 VuePress 构建的网站为 PDF，我竟然。。。](https://xie.infoq.cn/article/dd1753a47d9b80c4a14fa7ef5)

## 使用方法

讲爬取和生成逻辑区分开来，一起执行的时候容易爬漏页面，或页面爬取结果不够理想
故将爬取html逻辑以及生成pdf逻辑区分开来

执行`test.py`，修改最后的要求参数，以及执行步骤即可
若爬取后，再想调整生成只需要，将`down.down_all_page_to_pdf()`注释即可

## 原理

- `bs4`抓取网页生成html
- `利用pdfkit` 生成pdf
