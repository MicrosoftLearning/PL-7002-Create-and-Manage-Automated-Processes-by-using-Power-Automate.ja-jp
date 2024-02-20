---
lab:
  title: '課題 3:SharePoint'
  module: 'Module 3: Build approval flows with Power Automate'
---

# 実習ラボ 3 - SharePoint

このラボでは、SharePoint サイトとリストを作成します。

## 学習する内容

- SharePoint リストを作成する方法
- データをアップロードする方法

## ラボ手順の概要

- 営業案件の SharePoint リストを作成する
  
## 前提条件

- 以下を完了している必要があります: 「**ラボ 0: ラボ環境を検証する**」

## 詳細な手順

## 演習 1 - SharePoint リストを作成する

### タスク 1.1 SharePoint サイトを作成する

1. [Power Apps Maker ポータル](https://make.powerapps.com)で、ブラウザー ウィンドウの左上にある**アプリ起動ツール**を選び、**[OneDrive]** を選びます。

1. SharePoint で、**[+ サイトの作成]** を選びます。

1. **[チーム サイト]** を選び、**[Standard team]** テンプレートを選んで、**[テンプレートの使用]** を選びます。

1. **[サイト名]** に「`Power Automate`」と入力して、**[次へ]** を選びます。

1. **サイトの作成**を選択します。

1. **[完了]** を選びます。

### タスク 1.2 SharePoint リストを作成する

1. SharePoint サイトで、**[+ 新規]** を選び、**[リスト]** を選びます。

    ![新しい SharePoint リストのスクリーンショット。](../media/new-sharepoint-list.png)

1. **[空白のリスト]** を選びます

1. **[名前]** に「`Tasks`」と入力して、**[作成]** を選びます。

1. **[+ 列の追加]** を選び、**[複数行のテキスト]** を選び、**[次へ]** を選びます。

1. **[列の作成]** ペインで、次の値を入力するか選びます。

   1. 名前: `Description`
   1. データ型:**複数行のテキスト**

1. **[保存]** を選択します。

1. **[+ 列の追加]** を選び、**[テキスト]** を選び、**[次へ]** を選びます。

1. **[列の作成]** ペインで、次の値を入力するか選びます。

   1. 名前: `Owner Name`
   1. データ型:**1 行のテキスト**

1. **[保存]** を選択します。

1. **[+ 列の追加]** を選び、**[日付と時刻]** を選び、**[次へ]** を選びます。

1. **[列の作成]** ペインで、次の値を入力するか選びます。

   1. 名前: `Deadline`
   1. データ型:**日付と時刻**

1. **[保存]** を選択します。

1. **[+ 列の追加]** を選び、**[選択肢]** を選び、**[次へ]** を選びます。

1. **[列の作成]** ペインで、次の値を入力するか選びます。

   1. 名前: `Approval Status`
   1. データ型:**選択肢**
   1. 選択肢 1 = `New`
   1. 選択肢 2 = `Approved`
   1. 選択肢 3 = `Declined`

1. **[既定値]** に **[新規]** を選びます

    ![新しい SharePoint リストのスクリーンショット。](../media/add-choice-column.png)

1. **[保存]** を選択します。

1. SharePoint サイトの URL の最初の部分をコピーします (例: `https://m365x99999999.sharepoint.com/sites/PowerAutomate/`)

## 演習 2 - データの SharePoint リストを追加する

### タスク 2.1 - データを追加する

1. SharePoint サイトに移動し、**[タスク]** リストを選びます。

    ![[SharePoint タスク] リストのスクリーンショット。](../media/tasks-sharepoint-list.png)

1. **[+ 新規]** を選び、次のデータを入力して、**[保存]** を選びます。

   1. Title = `Contact Jon`
   1. Description = `Call or email`
   1. Owner Name = `MOD Administrator`
   1. Deadline = **Yesterday**
   1. Approval Status = **Declined**

1. **[+ 新規]** を選び、次のデータを入力して、**[保存]** を選びます。

   1. Title = `Create Quote`
   1. Description = `No discount`
   1. Owner Name = `MOD Administrator`
   1. Deadline = **Today**
   1. Approval Status = **Approved**

1. **[+ 新規]** を選び、次のデータを入力して、**[保存]** を選びます。

   1. Title = `Visit Jim`
   1. Description = `First visit`
   1. Owner Name = `MOD Administrator`
   1. Deadline = **Tomorrow**
   1. Approval Status = **New**

    ![[SharePoint タスク] データのスクリーンショット。](../media/tasks-data.png)
