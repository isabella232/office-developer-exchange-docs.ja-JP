---
title: Id (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Id
api_type:
- schema
ms.assetid: 3e1e37b5-5469-4447-ad1f-c2c6d4e0482f
description: Id 要素は、Exchange server 組織内の会議室を識別します。
ms.openlocfilehash: 5cd62f6f4e5912d2ecccda352be15c6a3b24e06c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831847"
---
# <a name="id-emailaddresstype"></a>Id (EmailAddressType)

**Id**要素は、Exchange server 組織内の会議室を識別します。 
  
[ルーム](room.md)
  
[Id (EmailAddressType)](id-emailaddresstype.md)
  
```xml
<Id>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Id>
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[名 (EmailAddressType)](name-emailaddresstype.md) <br/> |会議室の名前を定義します。 この要素はオプションです。  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |会議室の簡易メール転送プロトコル (SMTP) アドレスを定義します。 この要素はオプションです。  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |メールボックスに使用されるルーティングを定義します。 既定値は、SMTP です。 この要素はオプションです。  <br/> |
|[MailboxType](mailboxtype.md) <br/> |メールボックスのユーザーのメールボックスの種類を定義します。 この要素はオプションです。  <br/> |
|[ItemId](itemid.md) <br/> |ユーザーのアドレス帳フォルダーから受信者の連絡先または個人用配布リストの項目の識別子を定義します。 この要素はオプションです。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ルーム](room.md) <br/> |Exchange server 組織内の会議室を定義します。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、EWS のディレクトリにあるクライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターです。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetRooms 操作](getrooms-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

