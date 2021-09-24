---
title: HasAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: de152be6-fc2f-48bc-a05d-1211935da20a
description: HasAttachment 要素は、アイテムに添付ファイルが含されているかどうかを示すブール値を指定します。
ms.openlocfilehash: c3d153e86a9d170c69e74bdc08a3bdedfa5e1220
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516798"
---
# <a name="hasattachment"></a>HasAttachment

**HasAttachment 要素は**、アイテムに添付ファイルが含されているかどうかを示すブール値を指定します。 
  
```XML
<HasAttachment> true | false </HasAttachment
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[SearchPreviewItem](searchpreviewitem.md) <br/> |アイテムを開かなくても、プレビュー用のメールボックス アイテムの最初の 256 文字を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**HasAttachment** 要素のテキスト値 **が true** の場合は、アイテムに添付ファイルが設定されています。 false の **値は** 、アイテムに添付ファイルが存在しないかどうかを示します。 
  
## <a name="remarks"></a>注釈

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

