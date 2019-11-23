# 学内勉強会第１回 <基本のコマンド操作を覚えよう>
stc{hoge}というflagを用意しているので、練習がてらに見つけてみましょう。  

## 1. 使用するディレクトリ/フォルダを準備しよう
ターミナルを開いてコマンドを実行しよう  
```
git clone https://github.com/kisqragi/study-group-1st.git
```
`ls`コマンドでディレクトリがあるか確認。(lsと打ってエンター) 
上手くいっていればstudy-group-1stというディレクトリができているはずです。  
## 2. ディレクトリを自由に行き来しよう
study-group-1stの中に移動してみましょう。  
`cd <ディレクトリ名>` で好きなディレクトリに移動することができます。  
今回は `cd study-group-1st` で実行  
移動できたら`pwd`と打ち込んで今の場所を確認。  
`ls`コマンドでstudy-group-1stディレクトリ内にどんなファイルがあるか確認してみよう。  
移動操作ができるようになったらstudy-group-1st内のwork-1に移動してflagを見つけよう。  
(flagはstc{hoge}という型式です。)  

## ファイルの中身をみよう
今度はファイルの中身を見てみましょう。  
ファイルの中身を見るコマンドはいくつかありますが、今回はcatとlessコマンドを使います。  
では、study-group-1st内のwork-2に移動しましょう...  
work-2なんてないよ、って人は `cd ..` もしくは `cd` のみを実行しましょう。  
`cd ..` では今いるディレクトリの一つ上の階層のディレクトリに移動できます。  
`cd` のみの実行ではターミナルを開いた時と同じディレクトリ(ホームディレクトリ)に移動します。  
study-group-1st内のwork-2に移動できたら中にcat_fileとless_fileがあるのでそのファイルの中身をみていきます。  
```
cat <ファイル名>  
less <ファイル名>
```
で中身を見ることができます。  
### <u>catコマンド</u>
catコマンドでまず `work-2/cat_file` の中身を見てみましょう。  
work-2に移動して以下のコマンドを実行します。  
```
cat cat_file
```
cat_fileの中身が見れたと思います。  

catコマンドはconCATenate(連結)の略なのでファイルの中身を連結して一度に見ることができます。  
連結用にcat_file-1, 2, 3 を用意したのでやってみましょう。  
```
cat cat_file-1 cat_file-2 cat_file-3
```
各行に表示されている文字がそれぞれのファイルの中身になります。  
それぞれのファイルの中身をcatコマンドで確認してみても良いかもしれません。  

### <u>lessコマンド</u>
次はlessコマンドです。  
このコマンドは最初に使うにしては難しいですが、便利なのでぜひ覚えておきましょう。  
とりあえずコマンドを実行します。  
```
less less_file
```
キー操作は慣れるまで難しいですがとても便利です。  
下の表を見ながら実践してみましょう。  

|キー|操作|
|:---:|:---:|
| j | 1行進む |
| k | 1行戻る |
| f or SPACE | 1画面進む |
| b | 1画面戻る |
| q | 終了 |
| / | 検索 |
| n | 次の検索結果へ移動 |
| N | 前の検索結果へ移動 |

### flagを探してみましょう！  

lessコマンドを終了する場合は `q` を押しましょう。  
元の画面に戻ったと思います。  