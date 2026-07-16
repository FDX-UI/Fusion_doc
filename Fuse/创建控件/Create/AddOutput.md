# AddOutput 函数
添加输出
```lua
function AddOutput(
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
## 实例
```lua
OutImage = self:AddOutput("Output", "Output", {
    LINKID_DataType = "Image",
    LINK_Main       = 1,
})
```
