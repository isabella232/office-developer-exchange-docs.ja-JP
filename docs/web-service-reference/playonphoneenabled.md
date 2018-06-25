---
title: PlayOnPhoneEnabled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PlayOnPhoneEnabled
api_type:
- schema
ms.assetid: 6f800912-be4c-46f9-aa1e-dff0bbf877c5
description: PlayOnPhoneEnabled 要素は、電話での再生機能が有効になっているかどうかを示します。
ms.openlocfilehash: 1a6c5c41a4fe723f37d07ad0151dfbd6512cf4f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832829"
---
# <a name="playonphoneenabled"></a>PlayOnPhoneEnabled

**PlayOnPhoneEnabled**要素は、電話での再生機能が有効になっているかどうかを示します。 
  
```XML
<PlayOnPhoneEnabled>true | false</PlayOnPhoneEnabled>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[UnifiedMessagingConfiguration](unifiedmessagingconfiguration.md) <br/> |ユニファイド メッセージング サービスの構成情報が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

アカウントの電話での再生が有効になっている場合、 **PlayOnPhoneEnabled**要素が**true**の場合それ以外の場合、値が**false**にします。
  
## <a name="remarks"></a>備考

この要素は必須です。
  
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

