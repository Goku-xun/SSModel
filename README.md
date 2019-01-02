# SSModel
a very simple BaseModel for us.
you can just create Model inherit ZRBaseModel,and the Model will have this ability
normal data analysis is enough.
```

/*
*Model 到字典   类似逆向的 setValuesForKeysWithDictionary
*/
- (NSDictionary *)properties_aps;
/*
*通过运行时获取当前对象的所有属性的名称，以数组的形式返回
*/
- (NSArray *) allPropertyNames;

+(NSMutableArray *)getDataWithArr:(NSArray *)arr;

/*
*缓存数据进文件夹
*/
-(void)ArchiverFileWithFileName:(NSString *)fileName;

+(instancetype)UnarchiverFileWithFileName:(NSString *)fileName;

```

To integrate SSModel into your Xcode project using CocoaPods, specify it in your Podfile:
```
source 'https://github.com/CocoaPods/Specs.git'
platform :ios, '8.0'

target 'TargetName' do
pod 'SSModel'
end
```
Then, run the following command:

```
pod install
```

