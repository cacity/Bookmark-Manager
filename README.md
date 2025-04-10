# Chrome书签管理插件

## 功能介绍
这是一个Chrome浏览器扩展，用于高效管理你的书签。它能够：

1. **自动分类**：根据网站内容自动将书签分类
2. **归档管理**：将不常用的书签归档，保持书签栏整洁
3. **批量操作**：支持批量删除、移动、归档等操作
4. **独立管理**：所有操作都在插件内完成，不会影响原始Chrome书签
5. **侧边栏界面**：在浏览器右侧显示管理界面，方便操作
6. **书签勾选**：每个书签前有勾选框，可选择多个书签进行批量操作

## 使用方法
1. 安装插件后，在Chrome浏览器右上角会出现一个书签图标
2. 插件安装后会自动导入并同步你的Chrome书签
3. 点击图标打开侧边栏管理界面
4. 在侧边栏中可以查看所有书签，并进行分类、归档、删除等操作
5. 插件会每小时自动同步一次书签，你也可以点击“立即同步”按钮手动同步
6. 所有操作都在插件内完成，不会影响原始Chrome书签

### 书签勾选与批量操作
1. **勾选书签**：每个书签前面都有一个勾选框，可以选择一个或多个书签
2. **分类操作**：勾选书签后，可以点击“移动到分类”按钮，选择目标分类将书签移动过去
3. **归档操作**：勾选书签后，点击“移动到归档”按钮，将书签移入归档
4. **删除操作**：勾选书签后，点击“删除”按钮，可以删除选中的书签
5. **搜索结果操作**：在搜索结果中也可以勾选书签，进行移动、归档或删除操作
6. **批量操作标签页**：在“批量操作”标签页中，可以根据时间自动归档书签，或批量删除重复/断链书签

## 技术实现
- 使用Chrome Extension API进行开发
- 使用HTML, CSS, JavaScript构建用户界面
- 使用Chrome Storage API存储书签数据
- 使用Chrome Bookmarks API获取原始书签数据
- 使用Chrome Alarms API实现定期自动同步
- 使用Chrome SidePanel API实现侧边栏功能

## 项目结构
```
chrome书签插件/
├── images/             # 插件图标和界面图片
├── manifest.json       # 插件配置文件
├── popup.html          # 弹出窗口HTML
├── popup.js            # 弹出窗口JavaScript
├── popup.css           # 弹出窗口样式
├── sidebar.html        # 侧边栏HTML
├── sidebar.js          # 侧边栏JavaScript
├── sidebar.css         # 侧边栏样式
├── background.js       # 后台脚本
├── fix_all_issues.js   # 修复问题的脚本
├── fix_category.js     # 修复分类功能的脚本
└── README.md           # 项目说明文档
```

## 开发进度
- [x] 项目基础结构搭建
- [x] 插件配置文件编写
- [x] 书签数据获取功能
- [x] 书签分类算法实现
- [x] 侧边栏界面设计与实现
- [x] 批量操作功能实现
- [x] 数据存储与同步功能
- [x] 自动导入与定期同步功能
- [x] 修复导出书签功能
- [x] 修复新创建分类的使用问题
- [x] 修复分类数量统计问题

## 安装方法
1. 在Chrome浏览器中打开 chrome://extensions/
2. 开启右上角的"开发者模式"
3. 点击"加载已解压的扩展程序"
4. 选择本项目文件夹
5. 安装完成后，在Chrome浏览器右上角会出现插件图标
