# architecture

on-brand experience 强化品牌体验。


- Basil’s brand and app are designed to be approachable, direct, and delightfully surprising.
- Crane’s brand is refined and expressive, with an attention to visual and motion details that create an experience that feels tailor-made to the user.
-

| product   | Basil  | Crane  | Fortnightly| Owl     | Rally   |  Reply   | Shrine   |
| :-------- | :----- |:------ |:---------- |:------- |:------- | :------- |:-------- |
| what for  | recipe(食谱) | travel(订票/餐/房子) | news | educational (设计，艺术，建筑和时尚)|  理财 | email | retail(零售) |
| 特征  | 1. 平易近人，直接和令人愉快的惊喜 2. 时髦而实用的美学, 3. 大胆排版和颜色搭配简单的内容方法, 4. 令人兴奋的探索，易于理解| 1. 兼具功能性和信息丰富性 2. 精致而富有表现力，注重视觉和动作细节，创造出为用户量身定制的体验 3. 灵活美观 | 1. 内容突出 | 1. 充满活力和吸引力 2. energy，大胆的审美和有趣 3. 使用空缺来激励用户通过学习补充他们 | 1. 数据驱动，直接， 主次分明 2. 大量密集组织的信息，侧重于查看，调查和理解数据 3. 优质的风格 4. 主体突出（仪表盘）, 数据多但组织有序, 清晰 | 1. 提高清晰度，易读性，直观性和易用性 2. 友好, competence, and a hint of quirkiness. 2. 功能美学， 强调沟通 3. 功能突出，易用|  1. 时尚，优雅，精致。2. 极简主义审美
| 如何表达品牌 | 大胆的排版和颜色搭配简单的内容，创造一个令人兴奋的探索和易于理解的应用程序。 | 1. 自定义的交互性过路器提高交互体验, 交互性突出，更改的过滤器会立即在内容呈现上响应 | 1. 独特的图标，字体系统和突出的二级色（紫色应用程序的二级颜色）2. 通过颜色或排版引人注目 3. 灰度色调使摄影脱颖而出 4.从报纸中汲取灵感，并使用字体排版，标题加粗，长文本以便易于阅读。| 1. 大胆的颜色，形状和排版 2. 空缺和激励的文案 | 1. 深灰色UI, 明亮的强调色展示数据。 2. 数据与背景颜色之间的高对比度使其易于阅读其图形和图表。 3、 排版，颜色和形状来强调和组织数据。 | 应用的的品牌强调沟通。因此，应用程序的设计优先考虑功能质量，将易用性放在没有功能目的的设计元素上。 | 1. 视觉主题，边角削割, 强化突出品牌特色 2. 层叠效果
| 结构 | 四个顶层目录->分层数据->对等的两个tab页面。导航抽屉经常用于目录结构，Basil 使用了一种新颖的抽屉结构导航。| 程序使用流式结构。流结构是基于任务的结构，需要以连续顺序访问屏幕。三个顶级分类->过路器入口 + 结果呈现 | 目录结构 顶层分类 —> 结构预览数据（主部分 + 非主要部分，类似于报纸的头版和侧版） —> 详细页面 。使用标准的抽屉作为导航。目录结构允许用户快速导航到感兴趣的区域。| 分成三个部分，每个部分都有自己的主题和交互结构。 应用使用中心和轮辐（ hub and spoke）结构。各种子节点和教学形式为轮辐提供给用户。选择一个课并且用户进入Learn部分后，该课将成为一个中心，该课的每个部分都成为一个辐条。 | 分级结构。 内容按照相关性分块显示。永久显示导航栏方便快速的切换到不同的模块。 | 包含新消息和存档消息的收件箱，以及围绕这些消息相关的组织和执行操作构建的UI。主要的操作时生成和阅读消息。因此屏幕主要空间用于这些内容。在平板和手机上使用不同的导航,以确保空间足够。| 目录结构 分类目录 -> 页面浏览。 不同平台使用不同的导航方式。 |
| 布局 | Basil uses a responsive grid system, which has flexible columns and padding |
| 布局 | 视差和不透明度代替阴影来表示层次。运动视差来区分层，使用不透明度来表现高度差异（当文本在图像上方滚动时，双色调图像处理可确保文本保持清晰。）|  使用颜色代替阴影来表示层次。相同颜色的，使用阴影。 | 阴影层次 |  颜色和导航阴影 | 颜色和蒙层表达层次 | 颜色：由于Reply有时会显示密集内容，因此删除阴影会降低视觉复杂性。它还允许项目之间具有较小的填充，从而为内容留出更多空间。 | 颜色和 tab 阴影 |
| color | 0. 颜色使用要根据功能业务选择，不能看心情，靠喜好。例如，阅读类app 偏纸色，设计类 app 色彩浓重。 年轻女性消费着app 偏粉色。1, 设计中的主色，和 android theme 的 primaryColor 并不是对应的，设计中的主色是只应用最多的颜色。应该进行变换应用的项目中。 2. 主色的次要色并不一定只有一种，根据需要可能会有几种，但是要有规律，不能随意使用颜色。并且要统一， 主色用于分主题，分功能模块，不能页面随便变换颜色。 次要色使用也应该根据规律，没有规律可寻的颜色设置显得杂乱。 3. 字体色也是颜色的重要部分，如果字体使用除白色和黑色衍生色之外的颜色，字体色也要算作主题色中。|