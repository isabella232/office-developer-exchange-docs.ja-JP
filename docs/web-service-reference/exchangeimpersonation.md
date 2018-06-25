---
title: ExchangeImpersonation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExchangeImpersonation
api_type:
- schema
ms.assetid: d8cbac49-47d0-4745-a2a7-545d33f8da93
description: ExchangeImpersonation 要素は、要求の SOAP ヘッダーで使用されます。 この要素が存在する場合、呼び出し元が ExchangeImpersonation 要素内に含まれているアカウントを偽装するとしています。
ms.openlocfilehash: aedeff22cda865ce1eec80dab9760d49fdc178f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760357"
---
# <a name="exchangeimpersonation"></a>ExchangeImpersonation

**ExchangeImpersonation**要素は、要求の SOAP ヘッダーで使用されます。 この要素が存在する場合、呼び出し元が**ExchangeImpersonation**要素内に含まれているアカウントを偽装するとしています。 
  
[ExchangeImpersonation](exchangeimpersonation.md)
  
```xml
<ExchangeImpersonation>
   <ConnectingSID/>
</ExchangeImpersonation>
```

 **ExchangeImpersonationType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ConnectingSID](connectingsid.md) <br/> |ExchangeImpersonation SOAP ヘッダーを使用する際に偽装するアカウントを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

呼び出し元のアカウントが必要でクライアント アクセス サーバーと**ms-exch-MayImpersonate** **ms の偽装 exch**上か、偽装するメールボックスを含むメールボックス データベースまたは Active Directory ユーザーと連絡先オブジェクトです。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[EWS でのサーバーからサーバーへの承認](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

