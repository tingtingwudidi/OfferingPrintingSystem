🏯  三宝佛光寺 · 供品准备打印系统
OfferingPrintingSystem
Lord Buddha Temple Singapore  ·  Offering Preparation & Print System

产品简介
本系统专为庙宇员工设计，应对善信批量预订供品时，能更快、更有效地完成前期准备工作。系统通过 SheetDB 直接连接 Google Sheet 数据源，自动按日期筛选供品记录，并生成可直接打印的标签页面。

使用流程
1.	自动载入 — 打开系统后自动连接 SheetDB 数据源，顶部显示所有可用日期按钮
2.	选择日期 — 点击绿色日期按钮，或手动输入日期后点「载入」
3.	查看清单 — 系统自动分类莲花烛 / 光明烛，显示完整供品清单
4.	打印标签 — 分别点击莲花烛或光明烛打印按钮，弹出打印预览页面

Google Sheet 栏位格式
⚠️  栏位标题须与以下完全一致，否则系统无法读取
栏位名称	说明	示例
准备供品日期	DD/M/YY 格式	19/4/26
祈福名称	善信名称（中英文均可）	陈一汕合家 / John Tan
备注栏	附加说明（填「无」视为空白）	Vesak Day
供品名称	含「莲花烛」或「光明烛」	莲花烛
佛祖名称	供奉对象	四面佛


🪷  莲花烛标签规格
标签纸型号：HERMA No.4270 — PREMIUM labels A4
参数	数值
标签尺寸	38.1 × 21.2 mm
Top margin	10.7 mm
Side margin	9.7 mm
Horizontal pitch	38.1 mm（无间隙）
Vertical pitch	21.2 mm（无间隙）
列数（Number across）	5 列
行数（Number down）	13 行
每页标签数	65 个

每格标签内容（4行）
•	第一行：祈福名称
•	第二行：备注栏
•	第三行：供奉日期（DD/MM/YY）
•	第四行：佛祖名称

打印功能
•	🔤 字体调整（＋ / － / 重置）
•	🔲 显示标签框 — 点击在每格显示粉色虚线对位框，方便对准标签纸
•	🖨️ 打印

打印设置（Chrome）
设置项	正确值	说明
纸张尺寸	A4 纵向	
边距	无 (None)	⚠️ 最关键，否则偏移
缩放比例	100%	不可选「适合页面」
页眉页脚	关闭	


🕯️  光明烛标签规格
纸张：普通 A4，每页 3 个矩形
参数	数值
每格尺寸	8.12 cm × 19.5 cm
每页格数	3 格
上下边距	10.5 mm
格间距	16.2 mm

字体规格
内容	条件	字体大小
祈福名称（中文）	≤ 3 字	100pt
祈福名称（中文）	> 3 字	80pt
祈福名称（英文）	< 10 字符	80pt
祈福名称（英文）	≥ 10 字符	60pt
喜敬 / 合家喜敬	—	45pt

第二行自动判断
•	名称含「合家」→ 显示「合家喜敬」
•	其他情况 → 显示「喜敬」

打印设置（Chrome）
设置项	正确值
纸张尺寸	A4 纵向
边距	无 (None)
缩放比例	100%
页眉页脚	关闭


日期格式
输入格式	示例	说明
DD/M/YY	19/4/26	主要格式
DD/MM/YYYY	19/04/2026	也支持
DD-MM-YYYY	19-04-2026	也支持


部署说明
⚠️  本系统需部署至网页服务器才能连接 SheetDB，不能直接双击本地文件运行。

推荐部署方式（Netlify Drop）
5.	下载 供品打印系统.html
6.	打开 app.netlify.com/drop
7.	将文件拖入页面
8.	获得网址后即可正常使用（如 https://xxx.netlify.app）
更新系统：重新拖入 Netlify Drop 即可覆盖原网址。

技术规格
•	纯 HTML 单文件，无需安装任何依赖
•	数据源：SheetDB API（连接 Google Sheet）
•	字体：Noto Serif SC / Noto Sans SC（Google Fonts）
•	兼容浏览器：Chrome（推荐）、Edge、Safari
https://sheetdb.io/api/v1/ayutqp5asrwb3
https://docs.google.com/spreadsheets/d/1Ar27XeIOvYDbMa5GMf1v63ODdjIZ04xlW7i00ZRd-qc/edit?gid=0#gid=0
