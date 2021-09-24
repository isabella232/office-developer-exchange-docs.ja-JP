---
title: MailboxType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MailboxType
api_type:
- schema
ms.assetid: 696e5fdb-d8c5-40f0-9e79-885eae65dfa4
description: MailboxType 要素は、電子メール アドレスで表されるメールボックスの種類を表します。
ms.openlocfilehash: f7605bf0e90851352efaaabed09e878be0925581
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524050"
---
# <a name="mailboxtype"></a>MailboxType

**MailboxType** 要素は、電子メール アドレスで表されるメールボックスの種類を表します。 
  
```XML
<MailboxType>Mailbox | PublicDL | PrivateDL | Contact | PublicFolder | Unknown | OneOff | GroupMailbox</MailboxType>
```

**MailboxTypeType**

## <a name="attributes-and-elements"></a>属性と要素

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

次の表に **、MailboxType** 要素に使用できる値を示します。 
  
|**値**|**説明**|
|:-----|:-----|
|メールボックス  <br/> |メールが有効な Active Directory オブジェクトを表します。  <br/> |
|PublicDL  <br/> |パブリック配布リストを表します。  <br/> |
|PrivateDL  <br/> |ユーザーのメールボックス内のプライベート配布リストを表します。  <br/> |
|Contact  <br/> |ユーザーのメールボックス内の連絡先を表します。  <br/> |
|PublicFolder  <br/> |パブリック フォルダーを表します。  <br/> |
|不明  <br/> |不明な種類のメールボックスを表します。  <br/> |
|OneOff  <br/> |個人用配布リストの 1 回のメンバーを表します。  <br/> |
|GroupMailbox  <br/> |グループ メールボックスを表します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

