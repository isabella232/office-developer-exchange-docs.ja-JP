---
title: SourceIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SourceIds
api_type:
- schema
ms.assetid: 0043abd5-ba9c-4d67-8832-325f32bf7651
description: SourceIds 要素には、変換するソース識別子が含まれる。
ms.openlocfilehash: e6a0767de0928578fb6ae16996ff39908580d45c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521341"
---
# <a name="sourceids"></a>SourceIds

**SourceIds 要素には**、変換するソース識別子が含まれる。 
  
[ConvertId](convertid.md)
  
[SourceIds](sourceids.md)
  
```xml
<SourceIds>
   <AlternateId/>
   <AlternatePublicFolderId/>
   <AlternatePublicFolderItemId/>
</SourceIds>
```

 **NonEmptyArrayOfAlternateIdsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[AlternateId](alternateid.md) <br/> |変換するアイテムまたはフォルダーの識別子について説明します。  <br/> |
|[AlternatePublicFolderId](alternatepublicfolderid.md) <br/> |変換するパブリック フォルダー識別子について説明します。  <br/> |
|[AlternatePublicFolderItemId](alternatepublicfolderitemid.md) <br/> |変換するパブリック フォルダーアイテム識別子について説明します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ConvertId](convertid.md) <br/> |サポートされている形式間でアイテムとフォルダーの識別子を変換Exchange定義します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされているコンピューター Exchange Server EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[ConvertId 操作](convertid-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)


[識別子の変換](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

