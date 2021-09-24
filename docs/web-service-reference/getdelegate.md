---
title: GetDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetDelegate
api_type:
- schema
ms.assetid: 6d5efe59-596f-46f8-bdc6-ca9cded9bb8e
description: GetDelegate 要素は、メールボックスへの代理人に関する情報を取得する要求を定義します。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。
ms.openlocfilehash: 922a1d92856ba92abdc0fba717879b9a9e2687ef
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512969"
---
# <a name="getdelegate"></a>GetDelegate

**GetDelegate 要素** は、メールボックスへの代理人に関する情報を取得する要求を定義します。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。 
  
```xml
<GetDelegate IncludePermissions="">
      <Mailbox/>
   <UserIds/>
</GetDelegate>
```

 **GetDelegateType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**IncludePermissions** <br/> |応答に各代理人ユーザーのアクセス許可設定が含まれているかどうかを示します。  <br/> |
   
#### <a name="includepermissions-attribute-values"></a>IncludePermissions 属性値

|**値**|**説明**|
|:-----|:-----|
|**True** <br/> |UserId 要素で返される委任ユーザー情報に加えて、委任ユーザーのアクセス許可が [返](userid.md) されます。  <br/> |
|**False** <br/> |[UserId](userid.md) 情報が返されます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[メールボックス](mailbox.md) <br/> |プリンシパルのメールボックスを識別します。  <br/> |
|[UserIds](userids.md) <br/> |プリンシパルのメールボックスから取得する代理人ユーザーの配列を含む。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
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


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

