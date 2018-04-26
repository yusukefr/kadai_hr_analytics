## 課題内容
人事データから、退職の予測確率を計算して、csvで出力をおこなう。  

dataフォルダ内の以下２つのデータから予測確率を提出  

+ ファイル名
    + モデル用：./data/final_hr_analysis_train.csv
    + スコア用：./data/final_hr_analysis_test.csv

+ データ形式
    + 第1列：index（ID列）
    + 第2列：left（1：退職、0：非退職の正解ラベル）
    + 第3列以降：特徴量
    + カテゴリ変数名：sales, salary
    + ヘッダー項目（以下11項目、以下順番で構成）
        + index
        + left
        + satisfaction_level
        + last_evaluation
        + number_project
        + average_montly_hours
        + time_spend_company
        + Work_accident
        + promotion_last_5years
        + sales
        + salary

+ 出力形式は2カラムのCSV
     + 第1列:ID
     + 第2列:確率

**注意 : leftを予測する問題ですよ。出力結果は、確率でなくてはなりません**

## 検証環境

### OS
+ Linux 4.4.0-116-generic #140-Ubuntu SMP Mon Feb 12 21:23:04 UTC 2018 x86_64 x86_64 x86_64 GNU/Linux
+ GNU bash, バージョン 4.3.48(1)-release (x86_64-pc-linux-gnu)

### Python
+ Python Version: 3.6.4 |Anaconda custom (64-bit)| (default, Jan 16 2018, 18:10:19) 
[GCC 7.2.0]
+ pandas Version: 0.22.0
+ matplotlib Version: 2.2.0
+ Numpy Version: 1.14.1
+ sklearn Version: 0.19.1
+ ipywidgets Version: 7.1.2
