---
title: ManagerMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 70c324d5-2196-406d-a674-73323f8d8b92
description: ManagerMailbox 要素には、連絡先のマネージャーのメールボックスを識別する SMTP 情報が含まれる。
ms.openlocfilehash: c30a343ad7071e92c826925407f8447ae6baccae
ms.sourcegitcommit: 63e48eaf2891a6db1a718b55cd69e3a0433c4a9c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/01/2021
ms.locfileid: "58851115"
---
# <a name="managermailbox"></a>ManagerMailbox

**ManagerMailbox 要素** には、連絡先のマネージャーのメールボックスを識別する SMTP 情報が含まれる。 
  
```XML
<ManagerMailbox>
   <Mailbox/>
</ManagerMailbox>
```

 **SingleRecipientType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[メールボックス](mailbox.md) <br/> |送信者を識別するメールが有効な Active Directory オブジェクトを識別します。  <br/> |
  
### <a name="parent-elements"></a>親要素

|**要素名**|**説明**|
|:-----|:-----|
|[Contact](contact.md) <br/> |ストア内の連絡先アイテムExchangeします。  <br/> |

## <a name="remarks"></a>解説

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
この要素は Exchange Server 2010 Service Pack 2 (SP2) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)


[連絡先の作成 (Exchange Web サービス)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

