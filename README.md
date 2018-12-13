替换golang的`tests`包的模板文件，自定义生成单元测试方法  
[gotests/internal/render/templates](https://github.com/cweill/gotests/tree/master/internal/render/templates)
## Usage

```
go get -u github.com/cweill/gotests/...

https://github.com/bbbht/gotests-custom-template.git /path/to/templates

gotests -template_dir /path/to/templates [options] PATH ...
```

## change log

1. 如果返回`error`类型，直接定义并比较`error`
默认为wantErr为`bool`类型，比较时不够具体