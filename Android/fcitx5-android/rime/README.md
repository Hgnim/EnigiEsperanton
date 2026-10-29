# fcitx5-android的rime插件

## 输入法与插件安装

前往其[开源仓库](https://github.com/fcitx5-android/fcitx5-android/releases)安装`app`与`plugin.rime`

## 部署配置文件

在输入法设置中，添加一个名为`中州韵`的输入法

将[epo.schema.yaml](./epo.schema.yaml)文件放入`[fcitx5-android配置目录]/data/rime/`目录中

编辑或新建`[fcitx5-android配置目录]/data/rime/default.custom.yaml`文件：
```yaml
#default.custom.yaml

#如果是编辑文件
#找到 schema_list 项后
#在其下添加 - schema: epo

#如果是新建文件
#直接将下列内容写入即可

patch:
  schema_list:
    - schema: epo
```

随后在输入法的菜单中（不是设置页面）找到重载配置相关的按钮点击后选择`世界语键盘`项即可