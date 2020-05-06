## 技术点
1. 样式、伪元素的使用
2. 逻辑处理
3. [css+vue实现流程图](https://www.cnblogs.com/scdisplay/p/12029074.html)

组件接受一个数组类型参数treeData
格式如下:
其中子节点可选的参数isLong,可以实现额外的样式

```javascript
  [{
      name:'节点1'
  },
  {
      name:'节点1',
      children:[
          {name:'节点2'}
      ]
  },
  {
      name:'节点1',
      children:[
          {name:'节点2',children:[{name:'节点3'}]}
      ]
  },
  {
      name:'节点1',
      children:[
          {name:'节点5'},
          {name:'节点5',isLong:true},
          {name:'节点26',children:[
              {name:'节点3'},
              {name:'节点3'},
              {name:'节点33',
                  children:[
                      {name:'节点3'},
                      {name:'节点3'},
                      {name:'节点3'}
                  ]
              }
          ]},
          {name:'节点3',children:[{name:'节点3'},{name:'节点3'}]},
          {name:'节点4',children:[{name:'节点3'}]},
          {name:'节点5',isLong:true},
      ]
  }]
  
```
