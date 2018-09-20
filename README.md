
Please Use [https://github.com/wenzhixin/bootstrap-table/tree/master/src/extensions/treegrid](https://github.com/wenzhixin/bootstrap-table/tree/master/src/extensions/treegrid)
-------------------------





TreeView for [bootstrapTable](https://github.com/wenzhixin/bootstrap-table)


![demo](https://raw.githubusercontent.com/lslvxy/bootstrapTable-treeView/master/assets/demo.png)

## DEMO

[http://imsense.site/bootstrapTable-treeView/](http://imsense.site/bootstrapTable-treeView/)

## NOTICE

数据中必须包含`parentId`属性,根节点`parentId=null`,子节点中根据配置的`parentId`==`options[treeId]`.

例如配置项中`treeId='id'`,那么子节点的`parentId`属性值为父节点的`id`

Data must contain `parentId` properties,

rootNode `parentId=null`

childNode `parentId=options[treeId]`

if options `treeId='id'`

childNode's `parentId` property value isparnetNode's `id` value


## USE

```
<script src="./src/bootstraptable-treeview.js"></script>
  
$('#tree_table').bootstrapTable({
    class: 'table table-hover table-bordered',
    data: data,
    pagination: false,//分页请设置为false
    treeView: true,//是否开启树视图
    treeId: "id",//id字段
    treeField: "name",//展示树的字段
    columns: [{
        field: 'name',
        title: '名称',
    },
    {
        field: 'desc',
        title: '详情',
    },
    ]
});
```
