# FuRegisterClass 函数
注册插件函数
```lua
function FuRegisterClass(
    name,       -- 唯一标识
    ClassType,  -- 类型
    attributes, -- 表格
)
```
## ClassType 参数
决定插件是什么类型的
```lua
CT_Tool          -- 标准图像处理工具
CT_Modifier      -- 修饰器
CT_SourceTool    -- 源工具
CT_ViewLUTPlugin -- 视图 LUT 插件
```
