---
title: ExchangeImpersonation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ExchangeImpersonation
api_type:
- schema
ms.assetid: d8cbac49-47d0-4745-a2a7-545d33f8da93
description: ExchangeImpersonation 要素は、要求の SOAP ヘッダーで使用されます。 この要素が存在する場合、呼び出し元は ExchangeImpersonation 要素内に含まれるアカウントを偽装しようとしている。
ms.openlocfilehash: 88a0ae18a869c14b9ae3ef2eb3cdfc189c8c60ea
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530767"
---
# <a name="exchangeimpersonation"></a>ExchangeImpersonation

**ExchangeImpersonation** 要素は、要求の SOAP ヘッダーで使用されます。 この要素が存在する場合、呼び出し元は **ExchangeImpersonation** 要素内に含まれるアカウントを偽装しようとしている。 
  
[ExchangeImpersonation](exchangeimpersonation.md)
  
```xml
<ExchangeImpersonation>
   <ConnectingSID/>
</ExchangeImpersonation>
```

 **ExchangeImpersonationType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ConnectingSID](connectingsid.md) <br/> |ExchangeImpersonation SOAP ヘッダーを使用している場合に偽装するアカウントを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

呼び出し元アカウントには、クライアント アクセス サーバー上の **ms-exch** 偽装権限と、偽装するメールボックスを含むメールボックス データベースまたは Active Directory User/Contact オブジェクトの **ms-exch-MayImpersonate** 権限が必要です。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[EWS でのサーバー間認証](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

