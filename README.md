### 我们的目的
一千个人眼中有一千个哈姆雷特，这是我们对Thinkphp的改动，我们团队根据我们自身的开发对Thinkphp所做的优化
* 去除低版本支持
* 更好的国际化
* 更优化的效率

### 修改记录
* 原__F__函数变更为__cache__，__cache__不在作为__S__别名，新增加**F**函数[_文件读写删除操作_]

```
F($file, $content = false, $mod = '');
```
* $this->error失败后也不自动退出，便于后续全局操作进行
* 控制器后缀更改为__Controller__，方法后缀追加__Action__,增加对应的自动加载规则
* **alias_import**的key不在区分大小写
* **D**函数自动对输入的__layer__进行__ucfirst__操作
* 优化 **I** 函数[_获取输入参数 支持过滤和默认值_] 

```
mixed I($name,$filter='int',$default='');
```
* 增加**regex**函数[*使用正则验证数据*]

```
boolen regex($value, $rule);
```
* and so on
