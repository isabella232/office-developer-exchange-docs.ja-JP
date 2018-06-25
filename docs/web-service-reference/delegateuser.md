---
title: DelegateUser
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegateUser
api_type:
- schema
ms.assetid: aac4e74e-f69b-4c41-a0c9-489610330fbf
description: DelegateUser の要素が 1 つのデリゲートを追加するメールボックスの更新を識別または代理人の管理の応答で、デリゲートが返されます。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 72ddc313a5a76cd0345918cad63b7775ff85026b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759954"
---
# <a name="delegateuser"></a>DelegateUser

**DelegateUser**の要素が 1 つのデリゲートを追加するメールボックスの更新を識別または代理人の管理の応答で、デリゲートが返されます。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。 
  
```xml
<DelegateUser>
   <UserId/>
   <DelegatePermissions/>
   <ReceiveCopiesOfMeetingMessages/>
   <ViewPrivateItems/>
</DelegateUser>
```

**DelegateUserType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ユーザー Id](userid.md) <br/> |デリゲートを識別します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[DelegatePermissions](delegatepermissions.md) <br/> |デリゲートのアクセス許可レベルの設定が含まれています。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[ReceiveCopiesOfMeetingMessages](receivecopiesofmeetingmessages.md) <br/> |代理人が会議に関連するプリンシパルにアドレス指定されたメッセージのコピーを受け取るかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[ViewPrivateItems](viewprivateitems.md) <br/> |代理人が主体のメールボックスにプライベートの予定表アイテムを表示する権限を持つかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DelegateUsers](delegateusers.md) <br/> |追加または更新のメールボックスに代理人の id が含まれています。  <br/> |
|[DelegateUserResponseMessageType](delegateuserresponsemessagetype.md) <br/> |代理人の管理操作の応答メッセージが含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [AddDelegate 操作](adddelegate-operation.md) 
- [UpdateDelegate 操作](updatedelegate-operation.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)
- [デリゲートを追加します。](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

