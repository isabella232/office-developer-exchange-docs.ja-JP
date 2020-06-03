---
title: Name (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Name
api_type:
- schema
ms.assetid: 98c58c53-9acc-4e89-9fcf-03f1b05abee1
description: Name 要素は、メールボックスユーザーの名前を表します。
ms.openlocfilehash: db6eb547b5c848dc31bbaa377692989b16771673
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466928"
---
# <a name="name-emailaddresstype"></a>Name (EmailAddressType)

**Name**要素は、メールボックスユーザーの名前を表します。 
  
```xml
<Name/>
```

**string**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[メールボックス](mailbox.md) <br/> |完全に解決された電子メールアドレスを識別します。  <br/> |
|[RoomList](roomlist.md) <br/> |会議室のリストを識別します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素を使用する場合は、文字列を表すテキスト値が必要です。
  
## <a name="remarks"></a>注釈

この要素は省略できます。 **Name**要素は、 **attachmenttype**、 **emailaddresstype**、および**EmailAddress**型に存在します。 **EmailAddress**型の**name**要素については、「 [name (EmailAddress)](name-emailaddress.md)要素のトピックを参照してください。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

