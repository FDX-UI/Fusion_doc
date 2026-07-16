# AddControlPage 函数
添加选项卡
```lua
function AddControlPage(
    Name,    -- string
    firsttag -- table
)
```
## Name 参数
唯一标识
## firsttag 参数
属性表决定选项卡的属性
### CT_Visible 可见性
```lua
CT_Visible = false
```
### CTID_DIB_ID 图标
...\Fusion 版本\Skins<br>
用解压工具打开Fusion.fuskin
```lua
CTID_DIB_ID = "Icons.Tools.Tabs.Color"
```
## 实例
```lua
self:AddControlPage("Color Controls")
```
