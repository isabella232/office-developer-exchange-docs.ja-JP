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
description: DelegateUser 要素は、メールボックスまたは代理人管理応答で返された代理人に対して追加または更新する単一の代理人を指定します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 40d9dacbd544436a3edf3213cf078cd33f961a74
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458804"
---
# <a name="delegateuser"></a>DelegateUser

**DelegateUser**要素は、メールボックスまたは代理人管理応答で返された代理人に対して追加または更新する単一の代理人を指定します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。 
  
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
|[UserId](userid.md) <br/> |代理人を識別します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[DelegatePermissions](delegatepermissions.md) <br/> |代理人のアクセス許可レベルの設定が含まれています。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[ReceiveCopiesOfMeetingMessages](receivecopiesofmeetingmessages.md) <br/> |代理人が、プリンシパルに宛てた会議関連のメッセージのコピーを受信するかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[ViewPrivateItems](viewprivateitems.md) <br/> |代理人が、プリンシパルのメールボックス内の個人の予定表アイテムを表示する権限を持っているかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DelegateUsers](delegateusers.md) <br/> |メールボックスで追加または更新する代理人の id が含まれます。  <br/> |
|[DelegateUserResponseMessageType](delegateuserresponsemessagetype.md) <br/> |代理人管理操作の応答メッセージを含みます。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [AddDelegate 操作](adddelegate-operation.md) 
- [UpdateDelegate 操作](updatedelegate-operation.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)
- [代理人の追加](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

