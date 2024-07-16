# ruby

> ruby info

```ruby
BasicObject
   |
   └── Object
        |  # Common methods: .class, .dup, .clone, .equal?, .freeze, .frozen?, .object_id, .send, .method, .is_a?
        ├── Module
        |    |  # Common methods: .include?, .name, .constants, .nesting, .ancestors, .class_variables, .instance_methods
        |    └── Class
        |         # Common methods: .new, .superclass, .allocate, .inherited, .attr_reader, .attr_writer, .attr_accessor
        |
        ├── Numeric
        |    |  # Common methods: .+, .-, .*, ./, .%, .**, .abs, .zero?, .nonzero?, .positive?, .negative?
        |    ├── Integer
        |    |    # Common methods: .odd?, .even?, .succ, .pred, .times, .chr, .digits, .next
        |    ├── Float
        |    |    # Common methods: .round, .ceil, .floor, .truncate, .finite?, .infinite?, .nan?
        |    ├── Rational
        |    |    # Common methods: .numerator, .denominator, .to_f, .to_i, .to_r
        |    └── Complex
        |         # Common methods: .real, .imaginary, .rectangular, .polar, .conjugate, .abs2, .arg
        |
        ├── String
        |    # Common methods: .length, .size, .empty?, .[], .slice, .split, .sub, .gsub, .chop, .chomp, .upcase, .downcase, .capitalize, .swapcase, .concat, .<<, .strip, .lstrip, .rstrip, .start_with?, .end_with?, .include?, .index, .rindex, .reverse, .to_sym, .intern, .hex, .oct, .tr, .tr_s, .delete, .squeeze, .count, .each_line, .each_byte, .each_char, .each_codepoint, .codepoints, .chars, .bytes
        |
        ├── Symbol
        |    # Common methods: .to_s, .id2name, .to_sym, .==, .eql?, .casecmp, .length, .empty?, .upcase, .downcase, .capitalize, .swapcase
        |
        ├── Array
        |    # Common methods: .length, .size, .empty?, .[], .at, .first, .last, .push, .pop, .shift, .unshift, .each, .map, .select, .reject, .compact, .flatten, .join, .reverse, .sort, .uniq, .zip, .transpose, .rotate, .shuffle, .sample, .index, .rindex
        |
        ├── Hash
        |    # Common methods: .length, .size, .empty?, .[], .[]=, .fetch, .store, .key?, .value?, .keys, .values, .each, .each_key, .each_value, .each_pair, .map, .select, .reject, .merge, .invert, .delete, .clear, .default, .default_proc
        |
        ├── Range
        |    # Common methods: .begin, .end, .first, .last, .each, .include?, .exclude_end?, .cover?, .to_a, .step, .size
        |
        ├── Regexp
        |    # Common methods: .match, .=~, .===, .source, .options, .casefold?, .to_s, .inspect, .freeze, .named_captures, .names
        |
        ├── Time
        |    # Common methods: .now, .at, .local, .utc, .mktime, .new, .year, .month, .day, .hour, .min, .sec, .usec, .nsec, .zone, .utc_offset, .isdst, .gmt?, .utc?, .localtime, .gmtime, .strftime, .to_i, .to_f, .to_r, .to_s
        |
        ├── Struct
        |    # Common methods: .new, .members, .each, .each_pair, .each_value, .length, .size, .[], .[]=, .to_h, .values, .values_at, .select, .reject
        |
        ├── IO
        |    |  # Common methods: .open, .foreach, .readlines, .popen, .sysopen, .sysread, .syswrite, .reopen, .close, .closed?, .gets, .read, .write, .seek, .tell, .eof?, .flush, .fileno, .fcntl, .isatty, .binmode, .sync, .sync=
        |    ├── File
        |    |    # Common methods: .open, .foreach, .readlines, .chmod, .chown, .delete, .rename, .umask, .exists?, .file?, .directory?, .readable?, .writable?, .executable?, .size, .zero?, .ctime, .mtime, .atime, .basename, .dirname, .extname
        |    └── Socket
        |         # Common methods: .open, .bind, .connect, .listen, .accept, .recv, .send, .shutdown, .getsockname, .getpeername, .setsockopt, .getsockopt
        |
        ├── Proc
        |    # Common methods: .new, .call, .lambda?, .arity, .parameters, .source_location, .binding, .to_proc, .yield, .curry, .===, .==, .eql?
        |
        ├── Method
        |    # Common methods: .call, .parameters, .owner, .name, .receiver, .unbind, .source_location, .to_proc, .==, .eql?
        |
        ├── Exception
        |    |  # Common methods: .new, .message, .backtrace, .cause, .inspect, .set_backtrace
        |    ├── StandardError
        |    |    # Common methods: .new, .message, .backtrace, .cause, .inspect, .set_backtrace
        |    |    ├── TypeError
        |    |    ├── ArgumentError
        |    |    ├── NameError
        |    |    |    └── NoMethodError
        |    |    ├── RuntimeError
        |    |    ├── IOError
        |    |    └── SystemCallError
        |    └── ScriptError
        |         # Common methods: .new, .message, .backtrace, .cause, .inspect, .set_backtrace
        |         ├── LoadError
        |         ├── NotImplementedError
        |         └── SyntaxError
        |
        ├── Fiber
        |    # Common methods: .new, .resume, .transfer, .alive?, .yield
        |
        └── Enumerable
             |  # Common methods: .each, .map, .collect, .select, .filter, .reject, .find, .detect, .find_all, .reduce, .inject, .all?, .any?, .none?, .one?, .count, .sum, .min, .max, .sort, .sort_by, .group_by, .partition, .first, .take, .drop, .each_with_index, .reverse_each, .zip, .cycle, .chunk, .slice_before
             └── Enumerator
                  # Common methods: .new, .each, .next, .peek, .rewind, .size, .with_index, .with_object, .lazy

```

```ruby
Object
├── BasicObject
│   └── Kernel
│       ├── puts
│       ├── print
│       ├── p
│       ├── require
│       ├── load
│       ├── raise
│       ├── include
│       ├── extend
│       └── method_missing
├── Module
│   └── Class
│       ├── new
│       ├── superclass
│       └── allocate
├── NilClass
│   └── nil?
├── TrueClass
│   └── to_s
├── FalseClass
│   └── to_s
├── Numeric
│   ├── Integer
│   │   ├── +
│   │   ├── -
│   │   ├── *
│   │   ├── /
│   │   ├── %
│   │   ├── **
│   │   ├── to_i
│   │   ├── to_f
│   │   ├── even?
│   │   ├── odd?
│   │   └── zero?
│   └── Float
│       ├── +
│       ├── -
│       ├── *
│       ├── /
│       ├── %
│       ├── **
│       ├── to_i
│       ├── to_f
│       ├── ceil
│       ├── floor
│       └── round
├── String
│   ├── +
│   ├── *
│   ├── []
│   ├── length
│   ├── size
│   ├── empty?
│   ├── include?
│   ├── start_with?
│   ├── end_with?
│   ├── upcase
│   ├── downcase
│   ├── capitalize
│   ├── strip
│   ├── split
│   └── gsub
├── Array
│   ├── []
│   ├── length
│   ├── size
│   ├── empty?
│   ├── include?
│   ├── push
│   ├── pop
│   ├── shift
│   ├── unshift
│   ├── join
│   ├── map
│   ├── select
│   └── sort
├── Hash
│   ├── []
│   ├── length
│   ├── size
│   ├── empty?
│   ├── include?
│   ├── keys
│   ├── values
│   ├── each
│   ├── merge
│   └── delete
├── Range
│   ├── include?
│   ├── first
│   ├── last
│   └── each
├── Regexp
│   ├── =~
│   ├── match
│   └── scan
├── Symbol
│   ├── to_s
│   └── to_sym
├── Proc
│   ├── call
│   └── lambda?
├── Time
│   ├── now
│   ├── to_i
│   ├── to_f
│   ├── year
│   ├── month
│   ├── day
│   ├── hour
│   ├── min
│   ├── sec
│   └── strftime
├── IO
│   ├── File
│   │   ├── open
│   │   ├── read
│   │   ├── write
│   │   ├── exists?
│   │   └── delete
│   └── Dir
│       ├── []
│       ├── chdir
│       ├── mkdir
│       ├── rmdir
│       └── glob
├── Exception
│   ├── StandardError
│   │   ├── ArgumentError
│   │   ├── IndexError
│   │   ├── NameError
│   │   ├── NoMethodError
│   │   ├── RuntimeError
│   │   ├── TypeError
│   │   └── ZeroDivisionError
│   └── SystemExit
└── Thread
    └── ThreadGroup
```

```ruby
Object
├── BasicObject
│   └── Kernel
│       ├── puts: 输出字符串并换行
│       ├── print: 输出字符串
│       ├── p: 输出对象的调试信息
│       ├── require: 加载外部库
│       ├── load: 加载文件
│       ├── raise: 抛出异常
│       ├── include: 包含模块
│       ├── extend: 扩展模块
│       └── method_missing: 处理未定义方法的调用
├── Module
│   └── Class
│       ├── new: 创建新对象
│       ├── superclass: 获取父类
│       └── allocate: 分配内存
├── NilClass
│   └── nil?: 判断对象是否为nil
├── TrueClass
│   └── to_s: 转换为字符串
├── FalseClass
│   └── to_s: 转换为字符串
├── Numeric
│   ├── Integer
│   │   ├── +: 加法
│   │   ├── -: 减法
│   │   ├── *: 乘法
│   │   ├── /: 除法
│   │   ├── %: 取模
│   │   ├── **: 幂运算
│   │   ├── to_i: 转换为整数
│   │   ├── to_f: 转换为浮点数
│   │   ├── even?: 判断是否为偶数
│   │   ├── odd?: 判断是否为奇数
│   │   └── zero?: 判断是否为零
│   └── Float
│       ├── +: 加法
│       ├── -: 减法
│       ├── *: 乘法
│       ├── /: 除法
│       ├── %: 取模
│       ├── **: 幂运算
│       ├── to_i: 转换为整数
│       ├── to_f: 转换为浮点数
│       ├── ceil: 向上取整
│       ├── floor: 向下取整
│       └── round: 四舍五入
├── String
│   ├── +: 字符串连接
│   ├── *: 重复字符串
│   ├── []: 获取子字符串
│   ├── length: 获取长度
│   ├── size: 获取长度
│   ├── empty?: 判断是否为空
│   ├── include?: 判断是否包含子字符串
│   ├── start_with?: 判断是否以某子字符串开头
│   ├── end_with?: 判断是否以某子字符串结尾
│   ├── upcase: 转换为大写
│   ├── downcase: 转换为小写
│   ├── capitalize: 首字母大写
│   ├── strip: 去除首尾空白
│   ├── split: 分割字符串
│   └── gsub: 全局替换
├── Array
│   ├── []: 获取元素
│   ├── length: 获取长度
│   ├── size: 获取长度
│   ├── empty?: 判断是否为空
│   ├── include?: 判断是否包含元素
│   ├── push: 添加元素
│   ├── pop: 移除最后一个元素
│   ├── shift: 移除第一个元素
│   ├── unshift: 添加到第一个位置
│   ├── join: 连接元素为字符串
│   ├── map: 映射元素
│   ├── select: 选择元素
│   └── sort: 排序
├── Hash
│   ├── []: 获取值
│   ├── length: 获取长度
│   ├── size: 获取长度
│   ├── empty?: 判断是否为空
│   ├── include?: 判断是否包含键
│   ├── keys: 获取所有键
│   ├── values: 获取所有值
│   ├── each: 遍历
│   ├── merge: 合并哈希
│   └── delete: 删除键值对
├── Range
│   ├── include?: 判断是否包含值
│   ├── first: 获取第一个值
│   ├── last: 获取最后一个值
│   └── each: 遍历
├── Regexp
│   ├── =~: 匹配正则表达式
│   ├── match: 匹配正则表达式
│   └── scan: 扫描匹配
├── Symbol
│   ├── to_s: 转换为字符串
│   └── to_sym: 转换为符号
├── Proc
│   ├── call: 调用过程
│   └── lambda?: 判断是否为lambda
├── Time
│   ├── now: 获取当前时间
│   ├── to_i: 转换为整数时间戳
│   ├── to_f: 转换为浮点数时间戳
│   ├── year: 获取年份
│   ├── month: 获取月份
│   ├── day: 获取日期
│   ├── hour: 获取小时
│   ├── min: 获取分钟
│   ├── sec: 获取秒
│   └── strftime: 格式化时间
├── IO
│   ├── File
│   │   ├── open: 打开文件
│   │   ├── read: 读取文件
│   │   ├── write: 写入文件
│   │   ├── exists?: 判断文件是否存在
│   │   └── delete: 删除文件
│   └── Dir
│       ├── []: 获取目录内容
│       ├── chdir: 改变当前目录
│       ├── mkdir: 创建目录
│       ├── rmdir: 删除目录
│       └── glob: 匹配目录内容
├── Exception
│   ├── StandardError
│   │   ├── ArgumentError: 参数错误
│   │   ├── IndexError: 索引错误
│   │   ├── NameError: 名称错误
│   │   ├── NoMethodError: 方法未定义错误
│   │   ├── RuntimeError: 运行时错误
│   │   ├── TypeError: 类型错误
│   │   └── ZeroDivisionError: 除零错误
│   └── SystemExit: 系统退出
├── Method
│   ├── call: 调用方法
│   ├── owner: 获取方法的所有者
│   └── name: 获取方法的名称
├── Enumerable
│   ├── each: 遍历元素
│   ├── map: 映射元素
│   ├── select: 选择元素
│   ├── reject: 排除元素
│   ├── find: 查找元素
│   ├── sort: 排序元素
│   ├── count: 计数元素
│   ├── reduce: 归约元素
│   └── group_by: 分组元素
└── Thread
    └── ThreadGroup

标准库
├── Abbrev: 计算字符串的缩写
├── Base64: 提供Base64编码和解码功能
├── Benchmark: 提供测量代码执行时间的工具
├── BigDecimal: 提供任意精度的十进制数运算
├── CGI: 提供CGI脚本的支持
├── CSV: 提供CSV文件的读写支持
├── Date: 提供日期和时间的处理
├── Delegator: 提供将方法调用委托给另一个对象的功能
├── Digest: 提供消息摘要算法（如MD5、SHA1等）
├── DRb: 提供分布式Ruby（Distributed Ruby）支持
├── ERB: 提供嵌入式Ruby（Embedded Ruby）模板系统
├── FileUtils: 提供文件和目录操作的实用工具
├── Find: 提供递归查找文件的功能
├── Forwardable: 提供将方法调用转发到另一个对象的功能
├── GetoptLong: 提供命令行选项解析功能
├── IPAddr: 提供IP地址操作和转换功能
├── JSON: 提供JSON格式数据的解析和生成功能
├── Logger: 提供日志记录功能
├── Net
│   ├── FTP: 提供FTP客户端功能
│   ├── HTTP: 提供HTTP客户端功能
│   ├── SMTP: 提供SMTP客户端功能
│   └── URI: 提供URI解析和操作功能
├── Observable: 提供观察者模式实现
├── OpenURI: 提供方便的HTTP和FTP访问功能
├── OptionParser: 提供命令行选项解析功能
├── Pathname: 提供路径名操作功能
├── PP: 提供更美观的对象打印功能
├── PStore: 提供对象持久化存储功能
├── Psych: 提供YAML格式数据的解析和生成功能
├── RDoc: 提供文档生成功能
├── REXML: 提供XML文档处理功能
├── Resolv: 提供DNS查询功能
├── Rinda: 提供分布式对象系统（如TupleSpace）
├── RubyGems: 提供RubyGems包管理功能
├── Scanf: 提供格式化输入解析功能
├── Set: 提供集合操作功能
├── Shell: 提供类似Unix shell的操作功能
├── Singleton: 提供单例模式实现
├── Socket: 提供网络套接字操作功能
├── StringIO: 提供在内存中读写字符串的功能
├── Tempfile: 提供临时文件操作功能
├── Thread: 提供线程操作功能
├── Time: 提供时间操作功能
├── Timeout: 提供超时控制功能
├── Tmpdir: 提供临时目录操作功能
├── Tracer: 提供代码执行跟踪功能
├── TSort: 提供拓扑排序功能
├── UN: 提供Unix常用命令的包装功能
├── URI: 提供URI解析和操作功能
├── WeakRef: 提供弱引用功能
└── YAML: 提供YAML格式数据的解析和生成功能
```

```javascript
Object
├── Object
│   ├── create: 创建一个新对象，使用现有的对象来提供新创建的对象的__proto__
│   ├── assign: 将所有可枚举属性的值从一个或多个源对象复制到目标对象
│   ├── keys: 返回一个包含对象自身所有可枚举属性名称的数组
│   ├── values: 返回一个包含对象自身所有可枚举属性值的数组
│   ├── entries: 返回一个包含对象自身所有可枚举属性的键值对的数组
│   └── freeze: 冻结一个对象，冻结后不能添加新属性，不能删除已有属性，不能修改已有属性的值
├── Function
│   ├── call: 调用一个函数，其具有指定的this值和参数
│   ├── apply: 调用一个函数，其具有指定的this值，以及作为一个数组提供的参数
│   └── bind: 创建一个新的函数，在调用时设置this关键字为提供的值
├── Array
│   ├── length: 设置或返回数组中元素的数目
│   ├── push: 向数组的末尾添加一个或多个元素，并返回新的长度
│   ├── pop: 删除并返回数组的最后一个元素
│   ├── shift: 删除并返回数组的第一个元素
│   ├── unshift: 向数组的开头添加一个或多个元素，并返回新的长度
│   ├── concat: 连接两个或多个数组，并返回结果
│   ├── slice: 返回一个新的数组，包含从开始到结束（不包括结束）的元素
│   ├── splice: 从数组中添加/删除项目，然后返回被删除的项目
│   ├── forEach: 对数组的每个元素执行一次提供的函数
│   ├── map: 创建一个新数组，其结果是该数组中的每个元素都调用一个提供的函数后的返回值
│   ├── filter: 创建一个新数组, 其包含通过所提供函数实现的测试的所有元素
│   ├── reduce: 对累加器和数组中的每个元素（从左到右）应用一个函数，将其减少为单个值
│   └── sort: 对数组的元素进行排序
├── String
│   ├── length: 返回字符串的长度
│   ├── charAt: 返回指定位置的字符
│   ├── charCodeAt: 返回指定位置的字符的Unicode编码
│   ├── concat: 连接两个或多个字符串，并返回新的字符串
│   ├── indexOf: 返回某个指定的字符串值在字符串中首次出现的位置
│   ├── lastIndexOf: 返回一个指定的字符串值最后出现的位置，在一个字符串中的指定位置从后向前搜索
│   ├── slice: 提取字符串的某个部分，并以新的字符串返回被提取的部分
│   ├── substring: 提取字符串中两个指定的索引号之间的字符
│   ├── substr: 从起始索引号提取字符串中指定数目的字符
│   ├── replace: 替换与正则表达式匹配的子串
│   ├── toUpperCase: 把字符串转换为大写
│   ├── toLowerCase: 把字符串转换为小写
│   ├── trim: 去除字符串两端的空白字符
│   ├── split: 把字符串分割为字符串数组
│   └── match: 找到一个或多个正则表达式的匹配
├── Number
│   ├── toFixed: 把数字转换为字符串，结果的小数点后有指定位数的数字
│   ├── toPrecision: 把数字格式化为指定的长度
│   ├── toString: 把数字转换为字符串，使用指定的基数
│   └── valueOf: 返回一个Number对象的基本数字值
├── Math
│   ├── PI: 返回圆周率
│   ├── abs: 返回数的绝对值
│   ├── ceil: 对数进行上舍入
│   ├── floor: 对数进行下舍入
│   ├── max: 返回两个指定的数中带有较大的值的那个数
│   ├── min: 返回两个指定的数中带有较小的值的那个数
│   ├── pow: 返回x的y次幂的值
│   ├── random: 返回0到1之间的随机数
│   ├── round: 把数四舍五入为最接近的整数
│   └── sqrt: 返回数的平方根
├── Date
│   ├── now: 返回自1970年1月1日 00:00:00 UTC到当前时间的毫秒数
│   ├── parse: 解析一个表示日期的字符串，并返回从1970年1月1日 00:00:00 UTC到该日期的毫秒数
│   ├── UTC: 根据世界时返回1970年1月1日 00:00:00 UTC到指定日期的毫秒数
│   ├── getFullYear: 从Date对象以四位数字返回年份
│   ├── getMonth: 从Date对象返回月份 (0 ~ 11)
│   ├── getDate: 从Date对象返回一个月中的某一天 (1 ~ 31)
│   ├── getDay: 从Date对象返回一周中的某一天 (0 ~ 6)
│   ├── getHours: 返回Date对象的小时 (0 ~ 23)
│   ├── getMinutes: 返回Date对象的分钟 (0 ~ 59)
│   ├── getSeconds: 返回Date对象的秒数 (0 ~ 59)
│   ├── getMilliseconds: 返回Date对象的毫秒(0 ~ 999)
│   ├── setFullYear: 设置Date对象中的年份（四位数字）
│   ├── setMonth: 设置Date对象中的月份 (0 ~ 11)
│   ├── setDate: 设置Date对象中月的某一天 (1 ~ 31)
│   ├── setHours: 设置Date对象中的小时 (0 ~ 23)
│   ├── setMinutes: 设置Date对象中的分钟 (0 ~ 59)
│   ├── setSeconds: 设置Date对象中的秒钟 (0 ~ 59)
│   ├── setMilliseconds: 设置Date对象中的毫秒 (0 ~ 999)
│   ├── toDateString: 把Date对象的日期部分转换为字符串
│   ├── toTimeString: 把Date对象的时间部分转换为字符串
│   ├── toLocaleDateString: 根据本地时间格式，把Date对象的日期部分转换为字符串
│   ├── toLocaleTimeString: 根据本地时间格式，把Date对象的时间部分转换为字符串
│   └── toISOString: 使用ISO标准将Date对象转换为字符串
├── RegExp
│   ├── test: 检测一个字符串是否匹配某个模式
│   └── exec: 检索字符串中指定的值。返回找到的值，并确定其位置
├── JSON
│   ├── parse: 将一个JSON字符串转换为JavaScript对象
│   └── stringify: 将JavaScript值转换为JSON字符串
└── Error
    ├── name: 设置或返回一个错误名
    └── message: 设置或返回一个错误信息

Node.js核心模块
├── fs
│   ├── readFile: 异步读取文件的全部内容
│   ├── writeFile: 异步写入数据到文件，如果文件不存在则创建文件
│   ├── appendFile: 异步地将数据追加到文件，如果文件不存在则创建文件
│   ├── readdir: 读取目录的内容
│   ├── mkdir: 创建目录
│   ├── unlink: 删除文件
│   ├── rmdir: 删除目录
│   ├── stat: 获取文件信息
│   ├── rename: 重命名文件或目录
│   └── watch: 监视文件或目录的更改
├── http
│   ├── createServer: 创建HTTP服务器
│   ├── request: 发送HTTP请求到服务器
│   ├── get: 发送HTTP GET请求到服务器
│   └── ServerResponse: 表示HTTP服务器响应的对象
├── https
│   ├── createServer: 创建HTTPS服务器
│   ├── request: 发送HTTPS请求到服务器
│   └── get: 发送HTTPS GET请求到服务器
├── net
│   ├── createServer: 创建TCP服务器
│   ├── connect: 创建TCP客户端
│   └── Socket: 表示TCP或UNIX套接字连接的对象
├── path
│   ├── join: 使用平台特定的分隔符作为定界符将所有给定的路径段连接在一起，然后规范化生成的路径
│   ├── resolve: 将路径或路径段解析为绝对路径
│   ├── extname: 返回路径的扩展名
│   ├── basename: 返回路径的最后一部分
│   └── dirname: 返回路径的目录名
├── url
│   ├── parse: 解析URL字符串并返回URL对象
│   ├── format: 将URL对象转换为字符串
│   └── resolve: 解析一个目标URL相对于一个基础URL
├── querystring
│   ├── parse: 将查询字符串解析为对象
│   ├── stringify: 将对象序列化为查询字符串
│   └── escape: 对查询字符串中的特殊字符进行编码
├── stream
│   ├── Readable: 可读流
│   ├── Writable: 可写流
│   ├── Duplex: 双工流
│   └── Transform: 转换流
├── crypto
│   ├── createHash: 创建并返回一个哈希对象，该对象可用于生成哈希摘要
│   ├── createHmac: 创建并返回一个HMAC对象，该对象可用于生成HMAC摘要
│   ├── createCipher: 创建并返回一个Cipheriv对象，该对象可用于加密数据
│   ├── createDecipher: 创建并返回一个Decipheriv对象，该对象可用于解密数据
│   └── randomBytes: 生成加密强伪随机数据
├── events
│   ├── EventEmitter: 事件触发器类
│   ├── on: 添加一个监听器到事件的监听器数组的末尾
│   ├── once: 添加一个一次性监听器到事件的监听器数组
│   ├── emit: 触发事件
│   └── removeListener: 从事件的监听器数组中移除指定的监听器
├── child_process
│   ├── spawn: 启动一个新进程
│   ├── exec: 运行一个命令并缓冲输出
│   ├── execFile: 运行一个文件并缓冲输出
│   └── fork: 创建一个新的Node.js进程并使用建立的IPC通信通道调用指定的模块
└── util
    ├── promisify: 将回调函数转换为返回Promise的函数
    ├── inherits: 实现对象之间的原型继承
    └── inspect: 返回一个对象的字符串表示，主要用于调试
```
