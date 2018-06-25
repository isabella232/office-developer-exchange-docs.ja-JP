---
title: GetDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetDelegate
api_type:
- schema
ms.assetid: 6d5efe59-596f-46f8-bdc6-ca9cded9bb8e
description: GetDelegate 要素は、メールボックスへの代理人についての情報を取得する要求を定義します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: e31d6bd4f4387094beb467fcc4dff31ca7ec5d62
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760687"
---
# <a name="getdelegate"></a>GetDelegate

**GetDelegate**要素は、メールボックスへの代理人についての情報を取得する要求を定義します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。 
  
```xml
<GetDelegate IncludePermissions="">
      <Mailbox/>
   <UserIds/>
</GetDelegate>
```

 **GetDelegateType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**IncludePermissions** <br/> |代理人のユーザーごとにアクセス許可の設定が応答に含まれているかどうかを示します。  <br/> |
   
#### <a name="includepermissions-attribute-values"></a>IncludePermissions 属性の値

|**値**|**説明**|
|:-----|:-----|
|**True** <br/> |[ユーザー Id](userid.md)要素に返されるデリゲートのユーザー情報の他のアクセス許可が返されるユーザーに委任できます。  <br/> |
|**False** <br/> |[ユーザー Id](userid.md)情報が返されます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[メールボックス](mailbox.md) <br/> |主体のメールボックスを識別します。  <br/> |
|[ユーザー Id](userids.md) <br/> |代理人のユーザー主体のメールボックスから取得する配列が含まれています。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetDelegate 操作](getdelegate-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

