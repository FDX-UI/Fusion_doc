# Create 函数
创建控件函数
```lua
function Create()
```
## self 对象
### AddInput 添加输入
```lua
function AddInput(
    labelname,  -- 显示标签
    scriptname, -- 脚本名称
    attributes  -- 属性表
)
```
```lua
InBright = self:AddInput("Brightness","Brightness", {
    LINKID_DataType    = "Number",
    INPID_InputControl = "SliderControl",
    INP_MaxScale       = 1.0,
    INP_MinScale       = -1.0,
    INP_Default        = 0.0,
})
...
InImage = self:AddInput("Input", "Input", {
    LINKID_DataType = "Image",
    LINK_Main       = 1,
})
```
### AddOutput 添加输出
```lua
function AddOutput(
    labelname,  -- 显示标签
    scriptname, -- 脚本名称
    attributes  -- 属性表
)
```
```lua
OutImage = self:AddOutput("Output", "Output", {
    LINKID_DataType = "Image",
    LINK_Main       = 1,
})
```
### AddControlPage 添加选项卡
```lua
self:AddControlPage("Color Controls")
```
### BeginControlNest 开始控件嵌套组
### EndControlNest 结束控件嵌套组
```lua
function BeginControlNest(
    name,   -- 显示标签
    _id,    -- 脚本名称
    expand  -- 展开状态
(
```
```lua
self:BeginControlNest("Color Picker", "ColorPicker", true)
 -- 控件
self:EndControlNest()
```
## 实例
```lua
function Create()
    InBright = self:AddInput("Brightness","Brightness", {
        LINKID_DataType    = "Number",
        INPID_InputControl = "SliderControl",
        INP_MaxScale       = 1.0,
        INP_MinScale       = -1.0,
        INP_Default        = 0.0,
    })

    nContrast = self:AddInput("Contrast", "Contrast", {
        LINKID_DataType    = "Number",
        INPID_InputControl = "SliderControl",
        INP_MaxScale       = 1.0,
        INP_MinScale       = -1.0,
        INP_Default        = 0.0,
    })

    nSaturation = self:AddInput("Saturation", "Saturation", {
        LINKID_DataType    = "Number",
        INPID_InputControl = "SliderControl",
        INP_MaxScale       = 5.0,
        INP_MinScale       = 0.0,
        INP_Default        = 1.0,
        ICD_Center         = 1,
    })

    nImage = self:AddInput("Input", "Input", {
        LINKID_DataType = "Image",
        LINK_Main       = 1,
    })

    utImage = self:AddOutput("Output", "Output", {
        LINKID_DataType = "Image",
        LINK_Main       = 1,
    })
end
```
