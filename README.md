# CompactCalendarView for AndroidX
## 概要
- CompacrCalendarViewのAndroidX環境対応版
  - 本家に提出されていた[AndroidXにMigrateするPR](https://github.com/SundeepK/CompactCalendarView/pull/356)を取り込むことでAndroidX環境で使用しても正常にビルドできるように
- Mavenリポジトリとして追加するだけで使用可能

## 使い方
- プロジェクトのsettings.gradleにPagesデプロイをリポジトリとして追加
  - ```gradle
    maven { // Example
      name = 'CompactCalendarView-GHPages'
      url = uri('https://r-ca.github.io/CompactCalendarView/')
    }
    ```
- モジュールのbuild.gradleにimplementationプロパティで追加
  - ```gradle
    implementation 'one.nem:compact-calendar-view:1.0.0'
    ```
<details>
  <summary>構成例</summary>

  ![image](https://github.com/r-ca/CompactCalendarView/assets/66072112/22a1bac6-734a-403e-a849-150ec61b996e)
</details>

## その他
一時的に必要になり急いで作成したことに加え, そもそもMaven, Gradle, Github Actions, Github Pagesなど主要技術自体への知識も多くないため、正しい動作をしている保証はありません。  
Issue/PRは歓迎です、可能な限り対応します。  

少しでもお役に立てば幸いです！

## Links
- サンプルプロジェクト
  - [r-ca/CompactCalendarViewDebug](https://github.com/r-ca/CompactCalendarViewDebug)
- オリジナルのREADME.md
  - [README.md](/ORIGINAL_README.md)
- フォーク元
  - [SundeepK/CompactCalendarView](https://github.com/SundeepK/CompactCalendarView)

## Thanks
- https://github.com/SundeepK
  - フォーク元ライブラリの作者
- https://github.com/Saharatt593
  - 引用したAndroidX対応コミットの作者
