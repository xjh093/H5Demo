# H5Demo

H5混合开发 笔记

# 注意：

## Log1: 2018.8.3

- 1.`+ (void)callback:(NSURL *)URL response:(id)responseObject forVC:(JHBaseH5VC *)vc`方法内要修改一处
```
@"apiResult('%@','%@')"
```

- 2.`+ (NSString *)jh_JSONStringFromDictionary:(NSDictionary *)dic` 方法内要修改一处

```
NSJSONWritingPrettyPrinted -> kNilOptions
```
