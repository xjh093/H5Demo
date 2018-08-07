# H5Demo

H5混合开发 笔记

# 注意：

## Log2: 2018.8.7

- 1.JHURLParser+Goto.m
```
+ (void)gotoWithURL:(NSURL *)URL
             params:(NSDictionary *)dic
              forVC:(JHBaseH5VC *)vc
{
  [mdic setValue:URL.path forKey:@"url"]; // 修改 URL.path 为 url
  
   NSString *url = URL.path;
   if (URL.query) {
      url = [NSString stringWithFormat:@"%@?%@",url,URL.query];
   }
   [mdic setValue:url forKey:@"url"];
}
```


## Log1: 2018.8.3

- 1.JHURLParser.m

`+ (void)callback:(NSURL *)URL response:(id)responseObject forVC:(JHBaseH5VC *)vc`方法内要修改一处
```
@"apiResult('%@','%@')"
```

- 2.NSString+JHCategory.m

`+ (NSString *)jh_JSONStringFromDictionary:(NSDictionary *)dic` 方法内要修改一处

```
NSJSONWritingPrettyPrinted -> kNilOptions
```
