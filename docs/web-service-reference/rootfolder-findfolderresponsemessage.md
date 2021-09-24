---
title: RootFolder (FindFolderResponseMessage)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RootFolder
api_type:
- schema
ms.assetid: 5089c815-663f-46be-bc59-aed9ee20f94a
description: RootFolder 要素には、FindFolder 操作中に 1 つのルート フォルダーを検索した結果が含まれる。
ms.openlocfilehash: 582d4642bb4ecd2816beba6df863eb274762f804
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512276"
---
# <a name="rootfolder-findfolderresponsemessage"></a>RootFolder (FindFolderResponseMessage)

**RootFolder 要素には、FindFolder** 操作中に 1 つのルート フォルダーを検索した [結果が含まれる。](findfolder-operation.md)
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Folders/>
</RootFolder>
```

 **FindFolderParentType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|IndexedPagingOffset  <br/> |インデックス付きページング ビューを使用するときに次の要求に使用する次のインデックスを表します。  <br/> |
|NumeratorOffset  <br/> |小数部のページ ビューを使用する場合に次の要求に使用する新しい分子値を表します。  <br/> |
|AbsoluteDenominator  <br/> |分数ページングを実行するときに次の要求に使用する次の分母を表します。  <br/> |
|IncludesLastItemInRange  <br/> |現在の結果にクエリ内の最後のフォルダーが含まれているかどうかを示します。この場合、それ以上のページングは不要です。  <br/> |
|TotalItemsInView  <br/> |制限に合格するフォルダーの総数を表します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[フォルダー](folders-ex15websvcsotherref.md) <br/> |FindFolder 操作を使用して見つかったフォルダーの [配列を格納します](findfolder-operation.md)。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |FindFolder 操作要求の状態と [結果を格納](findfolder-operation.md) します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[FindFolder 操作](findfolder-operation.md)


[フォルダーの検索](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

