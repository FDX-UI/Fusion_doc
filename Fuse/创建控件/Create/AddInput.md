# AddInput 函数
添加输入
```lua
function AddInput(
    labelname,  -- string
    scriptname, -- string
    attributes  -- table
)
```
## labelname 参数
显示标签
## scriptname 参数
唯一标识
## attributes 参数
属性表决定输入的属性
### LINKID_DataType 数据类型
```lua
LINKID_DataType = "Number"
```
### INPID_InputControl 控件类型
```lua
INPID_InputControl = "SliderControl"
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
