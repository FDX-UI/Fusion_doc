# FuRegisterClass 函数
注册插件函数
```lua
function FuRegisterClass(
    name,       -- string
    ClassType,  -- number
    attributes, -- table
)
```
## name 参数
唯一标识
## ClassType 参数
决定插件是什么类型的
```lua
CT_Tool          -- 标准图像处理工具
CT_Modifier      -- 修饰器
CT_SourceTool    -- 源工具
CT_ViewLUTPlugin -- 视图 LUT 插件
```
## attributes
属性表决定插件的属性
### REGS_Name 显示名称
```lua
REGS_Name = "Ex1_BrightContrast" -- string
```
### REGS_Category 菜单位置 (必填)
```lua
REGS_Category = "Fuses\\Examples" -- string
```
### REGS_OpIconString 缩写 (必填)
```lua
REGS_OpIconString = "E1BC" -- string
```
### REGS_OpDescription 简短描述 (必填)
```lua
REGS_OpDescription = "Example, showing the various Controls in Fusion" -- string
```
