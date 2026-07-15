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
    scriptname, -- 内部名称
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
    scriptname, -- 内部名称
    attributes  -- 属性表
)
```
```lua
OutImage = self:AddOutput("Output", "Output", {
    LINKID_DataType = "Image",
    LINK_Main = 1,
})
```
