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
