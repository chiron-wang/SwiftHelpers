# SwiftHelpers
此專案主要用來放置練習專案時，所使用的共用程式碼。

## 使用方式
* 下載 submodule
首先到專案資料夾內，專案必須包含git版控，接者使用指令下載此repo，

最後一個Helper為資料夾名稱，可以自訂

```
git submodule add https://github.com/chiron-wang/SwiftHelpers.git Helpers
```

* 刪除 submodule
```
git submodule deinit -f -- ./Helpers

rm -rf .git/modules/Helpers

git rm -f Helpers

// 如果沒有其他模組的話
git rm -f .gitmodules
```

* 更新 submodule
```
// 全部更新
git submodule foreach --recursive git pull origin master

// 單一更新
git pull
```
