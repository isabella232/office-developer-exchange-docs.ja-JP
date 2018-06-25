---
title: MailboxType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxType
api_type:
- schema
ms.assetid: 696e5fdb-d8c5-40f0-9e79-885eae65dfa4
description: MailboxType 要素は、電子メール アドレスで表されるメールボックスの種類を表します。
ms.openlocfilehash: d7232377951e8d9c8f191ac856058bc28467cadd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832305"
---
# <a name="mailboxtype"></a>MailboxType

**MailboxType**要素は、電子メール アドレスで表されるメールボックスの種類を表します。 
  
```XML
<MailboxType>Mailbox | PublicDL | PrivateDL | Contact | PublicFolder | Unknown | OneOff | GroupMailbox</MailboxType>
```

**MailboxTypeType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[メールボックス](mailbox.md) <br/> |完全に解決された電子メール アドレスを識別します。  <br/> |
|[RoomList](roomlist.md) <br/> |会議室の一覧を識別します。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表は、 **MailboxType**要素の値を一覧します。 
  
|**値**|**説明**|
|:-----|:-----|
|メールボックス  <br/> |メールが有効な Active Directory オブジェクトを表します。  <br/> |
|PublicDL  <br/> |パブリックな配布リストを表します。  <br/> |
|PrivateDL  <br/> |ユーザーのメールボックス内の個人用配布リストを表します。  <br/> |
|連絡先  <br/> |ユーザーのメールボックス内の連絡先を表します。  <br/> |
|パブリック フォルダー  <br/> |パブリック フォルダーを表します。  <br/> |
|Unknown  <br/> |メールボックスの不明な型を表します。  <br/> |
|OneOff  <br/> |個人用配布リストの 1 回限りのメンバーを表します。  <br/> |
|GroupMailbox  <br/> |グループのメールボックスを表します。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

