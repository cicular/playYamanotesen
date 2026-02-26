# 各ディレクトリの説明  
## .g8
  Play プロジェクト生成テンプレート（Giter8）の残骸。  
役割  
  プロジェクト作成時のテンプレート情報  
  普段の開発では基本触らない  
  Springで言えば「initializrの内部情報」みたいなもの。  
  
## app  
アプリケーションの本体です。  
Play は最初から Web アプリ前提のレイヤ構造を持っています。  
  
## build.sbt  
Mavenのpom.xml相当  
Spring BootがMaven/Gradleを選べるのに対し、Playはsbtが基本になります。
  
## conf  
設定とルーティングを管理します。  
中身の代表例：  
  application.conf（設定ファイル）  
  routes（URLマッピング定義）  
  
  ルーティングはコードではなく、routesファイルで宣言的に書く。  
  
## project  
sbtの内部管理ディレクトリ  
Spring Bootの.mvnディレクトリ的ポジション。  
  
## public  
静的リソース置き場  
CSS  
JS  
画像  
  
Spring Bootでいうsrc/main/resources/staticと同じ役割。  
  
# Playの構造の特徴
## routesがconfにある
Springと違い、ControllerのアノテーションでURLを定義しない  

## sbt前提
Mavenよりも設定記法が独特  
依存関係の解決も少し癖あり  

