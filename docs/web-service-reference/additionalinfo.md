---
title: AdditionalInfo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 50bebbab-2fef-4a27-a5a9-32d7200820b6
description: AdditionalInfo 要素は、メールボックスの保留中の状態に関する追加情報を指定します。
ms.openlocfilehash: 6fbe24d5d3e41f2ba9c81657b2c38240d10eefed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759289"
---
# <a name="additionalinfo"></a>AdditionalInfo

**AdditionalInfo**要素は、メールボックスの保留中の状態に関する追加情報を指定します。 
  
```XML
<AdditionalInfo></AdditionalInfo>
```

 **使用されています**
## <a name="attributes-and-elements"></a>属性および要素

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

AdditionalInfo 要素のテキスト値は、メールボックスの保留中の状態に関する追加情報です。
  
## <a name="remarks"></a>備考

この要素はオプションです。
  
この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型のスキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

