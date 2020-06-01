---
title: UserIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserIds
api_type:
- schema
ms.assetid: 78a09c3a-1646-4c55-95a2-1109fb11e1c6
description: UserIds 要素には、プリンシパルのメールボックスから取得または削除するデリゲートユーザーの配列が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: de4661226c154ef0d2d5ac55c57405e20c4d2aee
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459778"
---
# <a name="userids"></a>UserIds

**UserIds**要素には、プリンシパルのメールボックスから取得または削除するデリゲートユーザーの配列が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。 
  
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
|[UserId](userid.md) <br/> |プリンシパルのメールボックスから取得または削除する代理人を指定します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetDelegate](getdelegate.md) <br/> |メールボックスへの代理人に関する情報を取得する要求を定義します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[RemoveDelegate](removedelegate.md) <br/> |メールボックスから代理人を削除するための要求を定義します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetDelegate 操作](getdelegate-operation.md)
  
[RemoveDelegate 操作](removedelegate-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

