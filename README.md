# README

## セットアップ

サイト作成

```shell
hugo new site hugo-educenter
```

レポジトリ初期化

```shell
cd hugo-educenter
git init
echo '*~' >> .gitignore
echo '*.bak' >> .gitignore
echo '*.orig' >> .gitignore
echo '.env' >> .gitignore
echo 'public' >> .gitignore
echo 'resources' >> .gitignore
```

テーマ設定(submoduleはhttpsプロトコルで追加)

```shell
git submodule add https://github.com/themefisher/educenter-hugo.git themes/educenter
```

(参考)submoduleの削除

```shell
git submodule deinit -f themes/educenter
git rm themes/educenter
rm -fr .git/modules/educenter
```

サイト設定

```shell
cp -p themes/educenter/exampleSite/config.toml .
cp -pr themes/educenter/exampleSite/{content,static} .
```

## Link

* [Educenter Hugo \| Hugo Themes](https://themes.gohugo.io/educenter-hugo/)
