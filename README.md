## 我们的目的
一千个人眼中有一千个哈姆雷特，这是我们对Thinkphp的改动，我们团队根据我们自身的开发对Thinkphp所做的优化
* 去除低版本支持
* 更好的国际化
* 更优化的效率

## 修改记录
* ThinkPHP原F函数变更为cache，cache不在作为S别名，新增加F函数做文件读写删除操作
``F($file, $content = false, $mod = '')``
* $this->error失败后也不自动退出，便于后续全局操作进行
* 控制器后缀更改为Controller，方法后缀追加Action
* 由于控制器默认为Controller，所以修改对应的自动加载规则
* alias_import的key不在区分大小写
* D函数自动对输入的layer进行ucfirst操作
* 优化I函数 增加regex函数（使用正则验证数据）
``mixed I($name,$filter='int',$default='')``
``boolen regex($value, $rule)``
`123`
