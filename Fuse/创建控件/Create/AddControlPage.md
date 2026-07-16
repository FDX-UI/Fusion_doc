# AddControlPage 函数
添加选项卡
```lua
function AddControlPage(
    Name,    -- 显示标签
    firsttag -- 属性表
)
```
## Name 参数 (必填)
唯一标识
## firsttag 参数
属性表决定选项卡的属性
### CT_Visible 可见性
```lua
CT_Visible = false
```
### CTID_DIB_ID 图标
```lua
CTID_DIB_ID = "Icons.Tools.Tabs.Color"
```
## 实例
```lua
function Create()
    self:AddControlPage("hi")
end
```
