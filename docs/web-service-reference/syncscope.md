---
title: SyncScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SyncScope
api_type:
- schema
ms.assetid: e0ca231f-0374-4844-8d4c-ada8da167920
description: SyncScope 要素は、アイテムまたはアイテムとフォルダーに関連付けられた情報を同期応答で返すかどうかを指定します。
ms.openlocfilehash: 5e5d19809cea1f8f244444c09615ee888fea05be
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538899"
---
# <a name="syncscope"></a>SyncScope

**SyncScope 要素は**、アイテムまたはアイテムとフォルダーに関連付けられた情報を同期応答で返すかどうかを指定します。 
  
```xml
<SyncScope>NormalItems or NormalAndAssociatedItems</SyncScope>
```

 **SyncFolderItemsScopeType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[SyncFolderItems](syncfolderitems.md) <br/> |ストア フォルダー内のアイテムを同期する要求を定義Exchange要素。  <br/> 次に、この要素の XPath 式を示します。  <br/> /SyncFolderItems  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に **、SyncScope** 要素に使用できる値を示します。 
  
**SyncScope 要素の値**

|**値**|**説明**|
|:-----|:-----|
|NormalItems  <br/> |フォルダー内のアイテムのみを同期応答で返す方法を指定します。  <br/> |
|NormalAndAssociatedItems  <br/> |フォルダー内のアイテムとフォルダーに関連付けられた情報の両方を同期応答で返す方法を指定します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされているコンピューター Microsoft Exchange Server EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[SyncFolderItems 操作](syncfolderitems-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

