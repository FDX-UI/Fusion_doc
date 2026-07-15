# FuRegisterClass 函数
注册插件函数
```lua
function FuRegisterClass(
    name,       -- string
    ClassType,  -- number
    attributes, -- table
)
```
## name 参数 (必填)
唯一标识
## ClassType 参数 (必填)
决定插件是什么类型的
```lua
CT_Tool          -- 标准图像处理工具
CT_Modifier      -- 修饰器
CT_SourceTool    -- 源工具
CT_ViewLUTPlugin -- 视图 LUT 插件
```
## attributes 参数 (必填)
属性表决定插件的属性
### REGS_Name 显示名称
```lua
REGS_Name = "Ex1_BrightContrast"
```
### REGS_Category 菜单位置
```lua
REGS_Category = "Fuses\\Examples"
```
### REGS_OpIconString 缩写
```lua
REGS_OpIconString = "E1BC"
```
### REGS_OpDescription 简短描述
```lua
REGS_OpDescription = "Example1, using the functions of Color Matrix"
```
### REGS_HelpTopic 帮助文档的链接、路径或标识符
```lua
REGS_HelpTopic = "Example Location of Help"
```
### REGS_URL 网站链接
```lua
REGS_URL = "www.blackmagicdesign.com"
```
### REGS_IconID 自定义图标
```lua
REGS_IconID = "Icons.Tools.Icons.Example"
```
### REG_OpNoMask 禁用效果遮罩
```lua
REG_OpNoMask = true
```
