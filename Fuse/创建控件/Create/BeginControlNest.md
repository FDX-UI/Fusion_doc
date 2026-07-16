# BeginControlNest 函数
开始控件嵌套组
```lua
function BeginControlNest(
    name,   -- string
    _id,    -- string
    expand  -- boolean
)
```
## name 参数
显示标签
## _id 参数
唯一标识
## expand 参数
展开状态
## 实例
```lua
self:BeginControlNest("Color Picker", "ColorPicker", true)
 -- 控件
self:EndControlNest()
```
