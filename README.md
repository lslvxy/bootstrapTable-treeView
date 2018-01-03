TreeView for [bootstrapTable](https://github.com/wenzhixin/bootstrap-table)


![demo.png](https://raw.githubusercontent.com/lslvxy/bootstrapTable-treeView/master/assets/demo.png)

## DEMO

[http://lise.io/bootstrapTable-treeView/](http://lise.io/bootstrapTable-treeView/)

## NOTICE

数据中必须包含`parentId`属性

Data must contain `parentId` properties


## USE

```
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
