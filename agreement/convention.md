# PHP 编码规范
如果您是ecstore开发人员，请详细阅读以下规范，并严格遵守。这样在保证您代码可读性的同时还可以大大减少我们的工作量。

- [命名](#named-agreement)
- [PHP约定](#php-agreement)
- [ECStore开发约定](#ecstore-agreement)
- [注释](#comment-agreement)
- [代码布局](#code-topology-agreement)

<a name="named-agreement"></a>
## 命名
### 文件命名
> **Note:** 包含任何 PHP 代码的任何文件应扩展名应当为 ".php" 脚本除外。
ecos的文件命名的准则是，class名称与文件名关联。关联的方法是以包所在的目录为根目录，到类所在的文件，将目录分隔符改为下划线即为此类的名称。
ecos的app目录下存放的是我们的主要代码，类命名时app则不需要加上

- 控制器文件放在app下的controller文件夹下,类的命名时用'''ctl'''代替'''controller'''，如 ''app/b2c/controller/site/order.php'' 对应类名称 b2c_ctl_site_order
- 模型层文件放在app下的model文件夹下,类的命名时用'''mdl'''代替'''model'''，如 ''app/b2c/model/orders.php'' 对应类名称 b2c_mdl_orders
- 类库层文件放在app下的lib文件夹下,类的命名时用不用写'''lib'''，如 ''app/b2c/lib/order/delivery.php'' 对应类名称 b2c_order_delivery
- 数据库定义文件 放在app下的dbschema文件夹下,命名时内部数组索引的值与文件名同名，如 ''app/b2c/dbschema/cart.php'' 对应文件内数组名称为 $db['cart']=array (

### 类命名
使用骆驼加下划线法则，首字母小写。

    class b2c_ctl_site_order{
    }

### 类的成员变量声明
### 类的构造函数命名
### 函数(方法,接口)命名
### 变量命名
### 常量命名
<a name="php-agreement"></a>
## PHP约定
### 文件编码
### 缩进
### UNIX编码规范
### UNIX风格换行
### php标签
### 行的最大长度
### 行尾空格
### 大括号放置
### 空格使用
### 逗号放置
### 字符串文字
### 包含单引号（'）的字符串文字
### 变量替换
### 字符串连接
### 函数和方法的传址引用
### if/else/elseif语句
### switch 语句
<a name="ecstore-agreement"></a>
## ECStore开发约定
### dump方法的使用
### 数据库操作
### POST、GET请求
### model和lib代码
<a name="comment-agreement"></a>
## 注释
### 头部注释
### 引用文件和定义常量注释
### 类(接口)注释
### 函数(方法,接口)注释
### 程序行间注释
<a name="code-topology-agreement"></a>
## 代码布局
### 类布局
### 空行使用