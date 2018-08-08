---
title: 自動検出のエラー メッセージを処理する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: e5939ec2-1100-4174-8a88-5a6e09b60b23
description: 自動検出の各種エラーと、そのエラーの対処法について説明します。
ms.openlocfilehash: fcafc799f4d35e92159d2913845474ecf7bc5657
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758898"
---
# <a name="handling-autodiscover-error-messages"></a>自動検出のエラー メッセージを処理する

自動検出の各種エラーと、そのエラーの対処法について説明します。
  
自動検出により、カスタムのアプリケーションは構成情報を自動的に取得できるようになり、最適に動作するようになります。ただし、物事は計画どおりに進まないこともあります。発生することがある一般的なエラーについて説明して、ユーザーに要求するクライアントの手動構成を最小限にするためのエラー処理の方法について説明します。
  
## <a name="http-status-errors"></a>HTTP 状態のエラー
<a name="bk_HttpErrors"> </a>

最初の種類のエラーは、自動検出の要求を送信するときに発生することがある HTTP 状態です。応答に含まれる HTTP 状態が 200 (OK) 以外の場合、求めている自動検出の応答は応答のペイロードに含まれていません。わかりやすくするために、200 以外の状態コードを 3 つのカテゴリに分類します。
  
**表 1. HTTP 状態コード**

|**ステータス コード**|**エラーの種類**|**処理方法**|
|:-----|:-----|:-----|
|301 または 302  <br/> |リダイレクト エラー  <br/> |HTTP 応答ヘッダーの "Location" に格納されている URI に向けて要求を再送信します。 詳細については、「[リダイレクト エラーの処理](#bk_HandlingRedirects)」を参照してください。  <br/> |
|401  <br/> |未認証エラー  <br/> |[自動検出プロセス](autodiscover-for-exchange.md)では、複数の潜在的な URL を試してみることが必要になるため、このエラーはある URL のみで発生することがあります (その次の URL は資格情報を受け入れた状態になります)。 このため、単一の 401 エラーで資格情報が無効だと見なしてはいけません。 ただし、複数の URL から 401 エラーを受け取る場合は、ユーザーにパスワードの再入力を求めるプロンプトを表示します (可能な場合)。  <br/> |
|その他の 200 以外の状態  <br/> |無効な自動検出エンドポイントのエラー  <br/> |200 以外の状態コードを返す URL は無効であると見なして、一覧内で次に当たる URL の試行を続行します。  <br/> |
   
## <a name="autodiscover-errors"></a>自動検出のエラー
<a name="bk_AutodiscoverErrors"> </a>

自動検出要求の送信後に 200 (OK) の状態コードを得たとしても、必要としている情報がサーバーから送られたという意味にはなりません。200 の状態は自動検出の応答があったということだけを意味し、その応答のペイロードにはエラーが含まれていることもあります。SOAP 形式と POX 形式では、エラー情報の場所が異なります。
  
### <a name="soap-autodiscover-errors"></a>SOAP 自動検出のエラー

SOAP 自動検出の場合は、1 つ以上の [ErrorCode (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) 要素が応答の異なる場所に含まれていることがあります。 一般に、[Response (SOAP)](http://msdn.microsoft.com/library/4c2bcdeb-95ce-4ffa-bd83-118af53b534f%28Office.15%29.aspx) 要素の子要素として期待することや、応答内の各 [UserResponse (SOAP)](http://msdn.microsoft.com/library/5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd%28Office.15%29.aspx) 要素の子として期待することができます。 また、[UserSettingError (SOAP)](http://msdn.microsoft.com/library/abb175c5-4f38-4dcc-81e3-b511686862eb%28Office.15%29.aspx) 要素の子として出現することもあります (存在する場合)。 エラーのコンテキストは、次に示すように **ErrorCode** 要素の場所によって変化します。 
  
- **Response** 要素の子要素の場合、**ErrorCode** 要素は要求全体に当てはまるエラーを表します。 
    
- **UserResponse** 要素の子の場合は、特定のユーザーにのみ当てはまるエラーを表します。 
    
- **UserSettingError** 要素の子の場合は、要求された特定の設定に当てはまるエラーを表します。 
    
応答の例を調べてみましょう。 この例では、**Response** 要素の **ErrorCode** 要素に "NoError" という値が含まれています。この値は、全体的な成功を表します。 ただし、**UserResponse** 要素の **ErrorCode** 要素には "RedirectAddress" という値が含まれています。この値は、その特定のユーザーにエラーが発生したことを表します。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
    xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>14</h:MajorVersion>
      <h:MinorVersion>3</h:MinorVersion>
      <h:MajorBuildNumber>136</h:MajorBuildNumber>
      <h:MinorBuildNumber>1</h:MinorBuildNumber>
      <h:Version>Exchange2010_SP2</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <UserResponses>
          <UserResponse>
            <ErrorCode>RedirectAddress</ErrorCode>
            <ErrorMessage>Redirection address.</ErrorMessage>
            <RedirectTarget>elvin@mail.contoso.com</RedirectTarget>
            <UserSettingErrors />
            <UserSettings />
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope>
```

「[ErrorCode (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx)」の記事に、発生することがあるすべてのエラーの一覧が記載されています。 これらのほとんどは、回復不可能なエラーを表しますが、いくつかは特別な処理を認めるものがあります。 
  
**表 2. SOAP 自動検出の ErrorCode の値**

|**ErrorCode の値**|**処理方法**|
|:-----|:-----|
|RedirectAddress  <br/> |[RedirectTarget (SOAP)](http://msdn.microsoft.com/library/f8162724-cf9a-4543-a1ad-5846c8b10bfa%28Office.15%29.aspx) 要素の電子メール アドレスを使用して、[新しい電子メール アドレスで自動検出を再開](#bk_RestartAutodiscover)します。  <br/> |
|RedirectUrl  <br/> |**RedirectTarget** 要素の URL を[新しい URL として要求を再送信](#bk_ResendRequest)します。  <br/> |
|ServerBusy  <br/> |少し間をおいて、この URL を再試行します。一定時間待機するか、この URL を単に試行する URL の一覧の最後に移動します。このエラーを 1 つの URL から複数回受け取る場合は、その URL が無効であると見なす必要があります。  <br/> |
   
### <a name="pox-autodiscover-errors"></a>POX 自動検出のエラー

POX 自動検出サービスは、少し異なる方法でエラーを報告します。 回復不可能なエラーは、[Error (POX)](http://msdn.microsoft.com/library/91c63b62-ab68-4c32-a2f7-5a87c188335b%28Office.15%29.aspx) 要素に含まれています。 「[ErrorCode (POX)](http://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx)」の記事に、発生することがあるすべてのエラーの一覧が記載されています。 
  
リダイレクトのエラーは、[Action (POX)](http://msdn.microsoft.com/library/a3462c6b-453c-462a-830d-f29ee4a2babb%28Office.15%29.aspx) 要素に含まれています。 **Action** 要素の "settings" 以外の値は、どれもリダイレクト エラーを表します。 
  
**表 3. POX 自動検出の ErrorCode の値**

|**Action の値**|**処理方法**|
|:-----|:-----|
|redirectAddr  <br/> |[RedirectAddr (POX)](http://msdn.microsoft.com/library/0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4%28Office.15%29.aspx) 要素の電子メール アドレスを使用して、[新しい電子メール アドレスで自動検出を再開](#bk_RestartAutodiscover)します。  <br/> |
|redirectUrl  <br/> |[RedirectUrl (POX)](http://msdn.microsoft.com/library/c54f310f-8c99-4c37-8e73-ac87722b6229%28Office.15%29.aspx) 要素の URL を[新しい URL として要求を再送信](#bk_ResendRequest)します。  <br/> |
   
この例では、**Action** 要素には "redirectAddr" という値が含まれています。この値は、**RedirectAddr** 要素に含まれた新しい電子メール アドレスで新しい要求を送信する必要があることを示しています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    <Account>
      <Action>redirectAddr</Action>
      <RedirectAddr>elvin@mail.contoso.com</RedirectAddr>
    </Account>
  </Response>
</Autodiscover>
```

## <a name="handling-redirect-errors"></a>リダイレクト エラーの処理
<a name="bk_HandlingRedirects"> </a>

リダイレクト エラーのシナリオは 2 つの方法で処理できます。
  
- 新しい電子メール アドレスで自動検出を再開する。
    
- 新しい URL に要求を再送信する。
    
どちらのシナリオも続行する前に何らかの検証が必要になります。
  
### <a name="restarting-autodiscover-with-a-new-email-address"></a>新しい電子メール アドレスで自動検出を再開する
<a name="bk_RestartAutodiscover"> </a>

自動検出のリダイレクト応答で新しい電子メール アドレスを取得したときには、リダイレクト エラー応答で提示された新しい電子メール アドレスがエラーになった要求で送信されたアドレスと同じでないことを最初に確認します。同じになる場合は、自動検出を再開してはいけません。その代わりに、応答を生成した URL を無効と見なします。
  
新しい電子メール アドレスが異なる場合は、潜在的な自動検出エンドポイント URL の既存の一覧を破棄して、新しい電子メール アドレスに基づいた新しい一覧を生成します。
  
### <a name="resending-your-request-to-a-new-url"></a>新しい URL に要求を再送信する
<a name="bk_ResendRequest"> </a>

自動検出リダイレクト応答で新しい URL を取得したときには、まず、その URL を次のようにして検証する必要があります。
  
- URL が HTTPS URL であることを確認します。
    
- これまでに現在の電子メール アドレスで、この URL からエラーを受け取っていないことを確認します。
    
- カスタム アプリケーションに適用可能な場合は、ユーザーにリダイレクトについて知らせて、リダイレクトに従う許可を取ります。
    
- URL に要求を送信して、[サーバーが提示した SSL 証明書が有効であることを確認します](how-to-validate-a-server-certificate-for-the-ews-managed-api.md)。
    
URL が検証に合格した場合は、この新しい URL に要求を再送信します。
  
## <a name="see-also"></a>関連項目


- [Exchange の自動検出](autodiscover-for-exchange.md)
    
- [Exchange の SCP 参照を使用して自動検出エンドポイントを見つける](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [ErrorCode (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx)
    
- [ErrorCode (POX)](http://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx)
    

