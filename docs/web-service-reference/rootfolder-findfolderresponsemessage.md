---
title: RootFolder (FindFolderResponseMessage)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootFolder
api_type:
- schema
ms.assetid: 5089c815-663f-46be-bc59-aed9ee20f94a
description: RootFolder 要素には、FindFolder 操作中に単一のルート フォルダーの検索の結果が含まれています。
ms.openlocfilehash: 1cd79d5fa34318e7fe29606df84cbf0ef0520b93
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833253"
---
# <a name="rootfolder-findfolderresponsemessage"></a>RootFolder (FindFolderResponseMessage)

**RootFolder**要素には、 [FindFolder 操作](findfolder-operation.md)中に単一のルート フォルダーの検索の結果が含まれています。
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Folders/>
</RootFolder>
```

 **FindFolderParentType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|IndexedPagingOffset  <br/> |インデックス付きページング ビューを使用する場合、次の要求に使用する必要があります次のインデックスを表します。  <br/> |
|NumeratorOffset  <br/> |分数のページ ビューを使用する場合は、次の要求に使用する新しい分子の値を表します。  <br/> |
|AbsoluteDenominator  <br/> |分数形式のページングを実行する場合、次の要求に使用する分母を表します。  <br/> |
|IncludesLastItemInRange  <br/> |さらにページングが必要ないように、現在の結果が、クエリ内の最後のフォルダーを含めるかどうかを示します。  <br/> |
|TotalItemsInView  <br/> |制限を満たすフォルダーの総数を表します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[フォルダー](folders-ex15websvcsotherref.md) <br/> |[FindFolder 操作](findfolder-operation.md)を使用してフォルダーの配列が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |[FindFolder 操作](findfolder-operation.md)要求の結果ステータスを格納します。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目




  [FindFolder 操作](findfolder-operation.md)


[フォルダーを検索します。](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

