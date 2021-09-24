---
title: UserIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UserIds
api_type:
- schema
ms.assetid: 78a09c3a-1646-4c55-95a2-1109fb11e1c6
description: UserIds 要素には、プリンシパルのメールボックスから取得または削除する代理人ユーザーの配列が含まれる。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。
ms.openlocfilehash: c99c39a75060780974cb26546e3a9d2947a9dfb8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517359"
---
# <a name="userids"></a>UserIds

**UserIds 要素には**、プリンシパルのメールボックスから取得または削除する代理人ユーザーの配列が含まれる。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。 
  
```xml
<UserIds>
   <UserId/>
</UserIds>
```

 **ArrayOfUserIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[UserId](userid.md) <br/> |プリンシパルのメールボックスから取得または削除する代理人を識別します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetDelegate](getdelegate.md) <br/> |メールボックスへの代理人に関する情報を取得する要求を定義します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
|[RemoveDelegate](removedelegate.md) <br/> |メールボックスから代理人を削除する要求を定義します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetDelegate 操作](getdelegate-operation.md)
  
[RemoveDelegate 操作](removedelegate-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

