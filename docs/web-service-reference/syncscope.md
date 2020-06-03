---
title: SyncScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncScope
api_type:
- schema
ms.assetid: e0ca231f-0374-4844-8d4c-ada8da167920
description: SyncScope 要素は、同期応答でアイテムまたはアイテムとフォルダーの関連情報のみを返すかどうかを指定します。
ms.openlocfilehash: 5ede26204c823a452189222075c784f24e98d188
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463035"
---
# <a name="syncscope"></a>SyncScope

**Syncscope**要素は、同期応答でアイテムまたはアイテムとフォルダーの関連情報のみを返すかどうかを指定します。 
  
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
|[SyncFolderItems](syncfolderitems.md) <br/> |Exchange ストアフォルダー内のアイテムを同期する要求を定義する要素。  <br/> この要素の XPath 式を次に示します。  <br/> /Syncfolderitems  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に、 **Syncscope**要素に指定できる値を示します。 
  
**SyncScope 要素の値**

|**値**|**説明**|
|:-----|:-----|
|NormalItems  <br/> |同期応答でフォルダー内のアイテムのみが返されるように指定します。  <br/> |
|NormalAndAssociatedItems  <br/> |フォルダーとフォルダーに関連付けられたアイテムの両方が同期応答で返されることを指定します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[SyncFolderItems 操作](syncfolderitems-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

