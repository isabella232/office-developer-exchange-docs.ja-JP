---
title: 名 (EmailAddressType)
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
description: Name 要素は、メールボックス ユーザーの名前を表します。
ms.openlocfilehash: b140fd46608a04f9aaba17f917cc4171c056dcf2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832504"
---
# <a name="name-emailaddresstype"></a>名 (EmailAddressType)

**Name**要素は、メールボックス ユーザーの名前を表します。 
  
```xml
<Name/>
```

**string**

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

文字列を表す文字列値は、この要素を使用する場合に必要です。
  
## <a name="remarks"></a>備考

この要素はオプションです。 **AttachmentType**、 **EmailAddressType**、および**EmailAddress**の種類の**名前**の要素が存在しています。 **EmailAddress**の型の**名前**の要素は、[名前 (EmailAddress)](name-emailaddress.md)要素のトピックで説明します。 
  
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

