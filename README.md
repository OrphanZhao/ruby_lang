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
