# Firebase Project

## ローカルエミュレータ起動

エミュレータ起動前に、hostingアプリケーションとfunctionsのビルドをしておく。

```bash
# Vue app build
cd app
npm run build
```

```bash
# functions build
cd functions
npm run build
```

エミュレータの起動

```bash
firebase emulators:start
```

functions のURLは `/{project-name}/{location-name}/{function-name}` という形式になるので注意。

## デプロイ

* hosting

```bash
firebase deploy --only hosting
```

* functions

```bash

firebase deploy --only functions
```