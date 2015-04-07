# fis-command-release
## 优化说明
针对FIS的全局构建进行了一次优化，可以指定文件或者目录构建项目，减少构建时间。
```fis release -d ../ -p -o -m -P /android_htdocs/gift/gift.shtml```
    gift.shtml所依赖的静态资源文件都会被构建，其他文件则不会受影响。
## Usage

    Usage: release [options]
    
    Options:
    
        -h, --help          output usage information
        -d, --dest <names>  release output destination
        -r, --root <path>   set project root
        -w, --watch         monitor the changes of project
        -L, --live          automatically reload your browser
        -c, --clean         clean compile cache
        -m, --md5 [level]   md5 release option
        -D, --domains       add domain name
        -l, --lint          with lint
        -t, --test          with unit testing
        -o, --optimize      with optimizing
        -p, --pack          with package
        -u, --unique        use unique compile caching
        -P, --Path          指定文件构建
        -a --all            是否构建所有文件
        --verbose           enable verbose output
