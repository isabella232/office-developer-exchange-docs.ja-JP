---
title: IsEncrypted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IsEncrypted
api_type:
- schema
ms.assetid: 68a30e92-c2b1-4af5-bb16-ba38afb80c43
description: IsEncrypted 要素は、条件または例外を適用するために受信メッセージを S/MIME 暗号化する必要があるかどうかを示します。
ms.openlocfilehash: 54e0be5262ab14bac72152028091fe56b37f90a3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509764"
---
# <a name="isencrypted"></a>IsEncrypted

**IsEncrypted 要素** は、条件または例外を適用するために受信メッセージを S/MIME 暗号化する必要があるかどうかを示します。 
  
```XML
<IsEncrypted>true | false</IsEncrypted>
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
|[条件](conditions.md) <br/> |満たされると、ルールのルール アクションをトリガーする条件を表します。  <br/> |
|[例外](exceptions.md) <br/> |受信トレイ ルールで使用可能なすべてのルール例外条件を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

true のテキスト **値は** 、条件または例外が適用されるには、メッセージが S/MIME 暗号化されている必要があります。 false の **値は** 、条件または例外が適用されるには、メッセージが S/MIME である必要がなかからない場合を示します。 
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

