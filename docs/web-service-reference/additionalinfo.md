---
title: AdditionalInfo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 50bebbab-2fef-4a27-a5a9-32d7200820b6
description: AdditionalInfo 要素は、メールボックスの保留状態に関する追加情報を指定します。
ms.openlocfilehash: d8b707fb04ffe91d5c7aa793c6b56c8bb048f160
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544319"
---
# <a name="additionalinfo"></a>AdditionalInfo

**AdditionalInfo** 要素は、メールボックスの保留状態に関する追加情報を指定します。 
  
```XML
<AdditionalInfo></AdditionalInfo>
```

 **xs:string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MailboxHoldStatus](mailboxholdstatus.md) <br/> |メールボックスの保留状態を指定します。  <br/> |
|[NonIndexableItemDetail](nonindexableitemdetail.md) <br/> |インデックスを作成できないアイテムの詳細を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

AdditionalInfo 要素のテキスト値は、メールボックスの保持状態に関する追加情報です。
  
## <a name="remarks"></a>注釈

この要素は省略できます。
  
この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にできる  <br/> ||
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

