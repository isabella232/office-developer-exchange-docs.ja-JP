---
title: PhoneCallState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PhoneCallState
api_type:
- schema
ms.assetid: ac009eb3-6334-49ce-82be-48fe83577f9c
description: PhoneCallState 要素は、通話の現在の状態を指定します。
ms.openlocfilehash: d2088b9b2811befe80684188d49c8034c577cc55
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468531"
---
# <a name="phonecallstate"></a>PhoneCallState

**PhoneCallState**要素は、通話の現在の状態を指定します。 
  
```xml
<PhoneCallState>Idle or Connecting or Alerted or Connected or Disconnected or Incoming or Transferring or Forwarding</PhoneCallState>
```

 **PhoneCallStateType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[PhoneCallInformation](phonecallinformation.md) <br/> |通話の状態情報を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に、 **PhoneCallState**要素に指定できる値を示します。 
  
**PhoneCallState 要素の値**

|**値**|**説明**|
|:-----|:-----|
|アイドル  <br/> |最初の呼び出しの状態。  <br/> |
|接続中  <br/> |システムはこの通話にダイヤルしています。  <br/> |
|警告  <br/> |通話は警告状態にあります (電話は鳴っています)。  <br/> |
|Connected  <br/> |呼び出しは、接続状態です。  <br/> |
|Disconnected  <br/> |呼び出しは切断されます。  <br/> |
|読み込ま  <br/> |通話は受信です。  <br/> |
|渡す  <br/> |通話は別の宛先に転送されています。  <br/> |
|しよう  <br/> |通話は別の宛先に転送されています。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの/ews/ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

