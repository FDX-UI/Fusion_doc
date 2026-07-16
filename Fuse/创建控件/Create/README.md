# Create 函数
创建控件函数
```lua
function Create()
```
## self 对象
### AddInput 添加输入
### AddOutput 添加输出
### AddControlPage 添加选项卡
### RemoveControlPage 删除选项卡
### BeginControlNest 开始控件嵌套组
### EndControlNest 结束控件嵌套组
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
