---
title: DelegateUser
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DelegateUser
api_type:
- schema
ms.assetid: aac4e74e-f69b-4c41-a0c9-489610330fbf
description: DelegateUser 要素は、メールボックスに追加または更新する単一の代理人、または代理人管理応答で返される代理人を識別します。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。
ms.openlocfilehash: 1963bef64e32ff536f0544a03f019e7785bae4d0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510258"
---
# <a name="delegateuser"></a>DelegateUser

**DelegateUser 要素は**、メールボックスに追加または更新する単一の代理人、または代理人管理応答で返される代理人を識別します。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。 
  
```xml
<DelegateUser>
   <UserId/>
   <DelegatePermissions/>
   <ReceiveCopiesOfMeetingMessages/>
   <ViewPrivateItems/>
</DelegateUser>
```

**DelegateUserType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[UserId](userid.md) <br/> |代理人を識別します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
|[DelegatePermissions](delegatepermissions.md) <br/> |代理人のアクセス許可レベルの設定が含まれる。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
|[ReceiveCopiesOfMeetingMessages](receivecopiesofmeetingmessages.md) <br/> |代理人が、プリンシパルにアドレス指定された会議関連メッセージのコピーを受信するかどうかを示します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
|[ViewPrivateItems](viewprivateitems.md) <br/> |代理人がプリンシパルのメールボックス内のプライベート予定表アイテムを表示するアクセス許可を持つかどうかを示します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DelegateUsers](delegateusers.md) <br/> |メールボックスに追加または更新する代理人の ID を格納します。  <br/> |
|[DelegateUserResponseMessageType](delegateuserresponsemessagetype.md) <br/> |代理人管理操作の応答メッセージが含まれます。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [AddDelegate 操作](adddelegate-operation.md) 
- [UpdateDelegate 操作](updatedelegate-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)
- [代理人の追加](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

