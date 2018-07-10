---
title: Exchange から自動検出を使用してユーザー設定を取得します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 6d90c305-4802-4e18-8d52-f60349feaa8d
description: 自動検出を使用して Exchange サーバーからユーザー構成設定を取得する方法について説明します。
ms.openlocfilehash: f37de55d6681bcdef381561b166adf209d3919a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758956"
---
# <a name="get-user-settings-from-exchange-by-using-autodiscover"></a><span data-ttu-id="80f26-103">Exchange から自動検出を使用してユーザー設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="80f26-103">Get user settings from Exchange by using Autodiscover</span></span>

<span data-ttu-id="80f26-104">自動検出を使用して Exchange サーバーからユーザー構成設定を取得する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="80f26-104">Learn how to get user configuration settings from an Exchange server by using Autodiscover.</span></span>
  
<span data-ttu-id="80f26-105">自動検出では、ユーザーの電子メール アドレスとパスワードだけを使用してユーザーの構成情報に簡単にアクセスを提供することによってアプリケーションの構成が簡略化されます。</span><span class="sxs-lookup"><span data-stu-id="80f26-105">Autodiscover simplifies application configuration by providing easy access to user configuration information using only the user's email address and password.</span></span> <span data-ttu-id="80f26-106">[ユーザーの構成設定の数](http://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx)は、自動検出では、ユーザーの表示名または外部の web サービスの URL などです。</span><span class="sxs-lookup"><span data-stu-id="80f26-106">A [number of user configuration settings](http://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) are available via Autodiscover, such as the user's display name or external web service URL.</span></span> 
  
<span data-ttu-id="80f26-107">自動検出サービスからユーザーの設定を取得するために、次の開発テクノロジのうちのいずれかを使用できます。</span><span class="sxs-lookup"><span data-stu-id="80f26-107">You can use one of the following development technologies to retrieve user settings from the Autodiscover service:</span></span>
  
- <span data-ttu-id="80f26-108">[EWS のマネージ API のクライアント アプリケーションを開始](get-started-with-ews-managed-api-client-applications.md)する</span><span class="sxs-lookup"><span data-stu-id="80f26-108">The [Get started with EWS Managed API client applications](get-started-with-ews-managed-api-client-applications.md)</span></span>
    
- <span data-ttu-id="80f26-109">[Web サービスの SOAP の自動検出](http://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="80f26-109">The [SOAP Autodiscover web service](http://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx)</span></span>
    
- <span data-ttu-id="80f26-110">[POX の自動検出 web サービス](http://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="80f26-110">The [POX Autodiscover web service](http://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx)</span></span>
    
<span data-ttu-id="80f26-111">EWS のマネージ API は、ユーザー設定を取得するためのオブジェクト ベースのインタ フェースを提供します。</span><span class="sxs-lookup"><span data-stu-id="80f26-111">The EWS Managed API provides an object-based interface for retrieving user settings.</span></span> <span data-ttu-id="80f26-112">クライアント アプリケーションは、マネージ コードを使用する場合は、EWS のマネージ API を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="80f26-112">If your client application uses managed code, we recommend that you use the EWS Managed API.</span></span> <span data-ttu-id="80f26-113">EWS のマネージ API を使用する場合は、必要な設定は[Microsoft.Exchange.WebServices.Autodiscover.UserSettingName](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.autodiscover.usersettingname%28v=EXCHG.80%29.aspx)列挙体で使用できるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="80f26-113">If you are using the EWS Managed API, determine whether the settings that you need are available in the [Microsoft.Exchange.WebServices.Autodiscover.UserSettingName](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.autodiscover.usersettingname%28v=EXCHG.80%29.aspx) enumeration.</span></span> <span data-ttu-id="80f26-114">、されていない場合は、SOAP または POX の自動検出サービスを使用します。</span><span class="sxs-lookup"><span data-stu-id="80f26-114">If they aren't, you might want to use the SOAP or POX Autodiscover services.</span></span> 
  
<span data-ttu-id="80f26-115">Web サービスを使用する場合お勧め、SOAP の自動検出サービスを使用すること POX の自動検出サービスよりも豊富な機能をサポートしているためです。</span><span class="sxs-lookup"><span data-stu-id="80f26-115">If you are using a web service, we suggest that you use the SOAP Autodiscover service, because it supports a richer set of features than the POX Autodiscover service.</span></span> <span data-ttu-id="80f26-116">SOAP の自動検出サービスを使用できない場合の代替として最適では POX の自動検出サービスです。</span><span class="sxs-lookup"><span data-stu-id="80f26-116">If the SOAP Autodiscover service isn't available, the POX Autodiscover service is a good alternative.</span></span>
  
## <a name="set-up-to-get-user-settings"></a><span data-ttu-id="80f26-117">ユーザー設定を取得するように設定する</span><span class="sxs-lookup"><span data-stu-id="80f26-117">Set up to get user settings</span></span>
<span data-ttu-id="80f26-118"><a name="bk_Prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="80f26-118"></span></span>

<span data-ttu-id="80f26-119">自動検出サービスを使用してユーザー設定を取得する前に、次のものを使用しているか確認してください。</span><span class="sxs-lookup"><span data-stu-id="80f26-119">Before you get user settings by using the Autodiscover service, make sure that you have access to the following:</span></span>
  
- <span data-ttu-id="80f26-120">EWS マネージ API または POX ベースの自動検出サービス、Exchange Online 、Office 365 の一部としての Exchange Online、または Exchange 2007 SP1 以降のバージョンの Exchange を実行しているサーバーを使用しているか。 </span><span class="sxs-lookup"><span data-stu-id="80f26-120">If you are using the EWS Managed API or the POX-based Autodiscover service, Exchange Online, Exchange Online as part of Office 365, or a server that is running a version of Exchange starting with Exchange 2007 SP1.</span></span> 
    
- <span data-ttu-id="80f26-121">SOAP ベースの自動検出サービス、Exchange Online、または Exchange 2010 以降のバージョンの Exchange を使用しているか。</span><span class="sxs-lookup"><span data-stu-id="80f26-121">If you are using the SOAP-based Autodiscover service, Exchange Online or a version of Exchange starting with Exchange 2010.</span></span>
    
> [!NOTE]
> <span data-ttu-id="80f26-122">EWS のマネージ API を使用する場合は、いくつかの状況での[証明書検証のコールバック メソッドを提供](how-to-validate-a-server-certificate-for-the-ews-managed-api.md)する必要があります。</span><span class="sxs-lookup"><span data-stu-id="80f26-122">If you are using the EWS Managed API, you will need to [provide a certificate validation callback method](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) in some circumstances.</span></span> <span data-ttu-id="80f26-123">証明書検証コールバック メソッドによって生成されたプロキシのライブラリ、Visual Studio によって作成されたものなどをする必要もあります。</span><span class="sxs-lookup"><span data-stu-id="80f26-123">You might also need a certificate validation callback method with some generated proxy libraries, such as those created by Visual Studio.</span></span> 
  
## <a name="get-user-settings-by-using-the-ews-managed-api"></a><span data-ttu-id="80f26-124">EWS マネージ API を使用してユーザー設定を取得する</span><span class="sxs-lookup"><span data-stu-id="80f26-124">Get user settings by using the EWS Managed API</span></span>
<span data-ttu-id="80f26-125"><a name="bk_Managed"> </a></span><span class="sxs-lookup"><span data-stu-id="80f26-125"></span></span>

<span data-ttu-id="80f26-126">次の例のように、ユーザーの構成情報を取得するために[GetUserSettings](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx)メソッドを使用できます。</span><span class="sxs-lookup"><span data-stu-id="80f26-126">You can use the [GetUserSettings](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx) method to retrieve configuration information for a user, as shown in the following example.</span></span> <span data-ttu-id="80f26-127">この例では、(から[UserSettingName](http://msdn.microsoft.com/ja-jp/library/exchange/microsoft.exchange.webservices.autodiscover.usersettingname%28v=exchg.80%29.aspx)列挙に含まれる) を取得するユーザー設定の配列を指定することができ、メソッドは、Exchange サーバーからリダイレクト応答に従います。</span><span class="sxs-lookup"><span data-stu-id="80f26-127">In this example, you can specify an array of user settings to return (from those available in the [UserSettingName](http://msdn.microsoft.com/ja-jp/library/exchange/microsoft.exchange.webservices.autodiscover.usersettingname%28v=exchg.80%29.aspx) enumeration), and the method will follow redirection responses from the Exchange server.</span></span> 
  
```cs
using System;
using System.Net;
using Microsoft.Exchange.WebServices.Autodiscover;
public static GetUserSettingsResponse GetUserSettings(
    AutodiscoverService service,
    string emailAddress,
    int maxHops,
    params UserSettingName[] settings)
{
    Uri url = null;
    GetUserSettingsResponse response = null;
    for (int attempt = 0; attempt < maxHops; attempt++)
    {
        service.Url = url;
        service.EnableScpLookup = (attempt < 2);
        response = service.GetUserSettings(emailAddress, settings);
        if (response.ErrorCode == AutodiscoverErrorCode.RedirectAddress)
        {
            url = new Uri(response.RedirectTarget);
        }
        else if (response.ErrorCode == AutodiscoverErrorCode.RedirectUrl)
        {
            url = new Uri(response.RedirectTarget);
        }
        else
        {
            return response;
        }
    }
    throw new Exception("No suitable Autodiscover endpoint was found.");
}
```

<span data-ttu-id="80f26-p106">ユーザー設定の配列の各キー/値ペアにアクセスするために返されるコレクションを解析することができます。次の使用例は、返された各要素を解析し、各キー/値ペアの名前と値を表示する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="80f26-p106">You can parse the collection returned to access each key/value pair in the user settings array. The following example shows how to parse through each returned element and display the name and value of each key/value pair.</span></span>
  
```cs
// Display each retrieved value. The settings are part of a key/value pair.
// userresponse is a GetUserSettingsResonse object.
foreach (KeyValuePair<UserSettingName, Object> usersetting in userresponse.Settings)
{
    Console.WriteLine(usersetting.Key.ToString() + ": " + usersetting.Value);
}
```

<span data-ttu-id="80f26-130">または、特定の設定の値を取得できます。</span><span class="sxs-lookup"><span data-stu-id="80f26-130">Alternatively, you can obtain the value of a specific setting.</span></span> <span data-ttu-id="80f26-131">次の例では、 **UserDisplayName**の設定、表示されます。</span><span class="sxs-lookup"><span data-stu-id="80f26-131">In the following example, the **UserDisplayName** setting is to be displayed.</span></span> 
  
```cs
// Display a specific setting, such as UserDisplayName.
Console.WriteLine(userresponse.Settings[UserSettingName.UserDisplayName]);
```

## <a name="get-user-settings-by-using-soap-autodiscover"></a><span data-ttu-id="80f26-132">SOAP 自動検出を使用してユーザー設定を取得する</span><span class="sxs-lookup"><span data-stu-id="80f26-132">Get user settings by using SOAP Autodiscover</span></span>
<span data-ttu-id="80f26-133"><a name="bk_SOAP"> </a></span><span class="sxs-lookup"><span data-stu-id="80f26-133"></span></span>

<span data-ttu-id="80f26-p108">EWS マネージ API を使用していない場合は、SOAP の自動検出 Web サービスを使用することをお勧めします。SOAP の自動検出 Web サービスが失敗した、または利用できない場合にのみ、POX 自動検出 Web サービスを使用します。 </span><span class="sxs-lookup"><span data-stu-id="80f26-p108">If you're not using the EWS Managed API, we recommend that you use the SOAP Autodiscover web service. Only use the POX Autodiscover web service if the SOAP Autodiscover web service fails or is not available.</span></span> 
  
<span data-ttu-id="80f26-136">ユーザー設定を取得するには、 [GetUserSettings 操作 (SOAP)](http://msdn.microsoft.com/library/758d965c-ef63-4de4-9120-e293abf14ff8%28Office.15%29.aspx)を使用します。</span><span class="sxs-lookup"><span data-stu-id="80f26-136">To get user settings, use the [GetUserSettings operation (SOAP)](http://msdn.microsoft.com/library/758d965c-ef63-4de4-9120-e293abf14ff8%28Office.15%29.aspx).</span></span> <span data-ttu-id="80f26-137">要求された設定は、 [UserSetting の要素](http://msdn.microsoft.com/library/aac6dc31-edd2-49d7-b845-1df4d77da58c%28Office.15%29.aspx)として返されます。</span><span class="sxs-lookup"><span data-stu-id="80f26-137">The requested settings are returned as [UserSetting elements](http://msdn.microsoft.com/library/aac6dc31-edd2-49d7-b845-1df4d77da58c%28Office.15%29.aspx).</span></span>
  
<span data-ttu-id="80f26-138">次の例では、サーバーからユーザー設定を取得する SOAP 自動検出要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="80f26-138">The following example shows a SOAP Autodiscover request to get user settings from the server.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://autodiscover.exchange.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>mara@contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>UserDisplayName</a:Setting>
          <a:Setting>UserDN</a:Setting>
          <a:Setting>UserDeploymentId</a:Setting>
          <a:Setting>InternalMailboxServer</a:Setting>
          <a:Setting>MailboxDN</a:Setting>
          <a:Setting>PublicFolderServer</a:Setting>
          <a:Setting>ActiveDirectoryServer</a:Setting>
          <a:Setting>ExternalMailboxServer</a:Setting>
          <a:Setting>EcpDeliveryReportUrlFragment</a:Setting>
          <a:Setting>EcpPublishingUrlFragment</a:Setting>
          <a:Setting>EcpTextMessagingUrlFragment</a:Setting>
          <a:Setting>ExternalEwsUrl</a:Setting>
          <a:Setting>CasVersion</a:Setting>
          <a:Setting>EwsSupportedSchemas</a:Setting>
          <a:Setting>GroupingInformation</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="80f26-p110">次の例では、クライアントからの要求を解析した後に、サーバーによって返される SOAP 応答を示します。応答には、要求される設定のみが含まれます (存在する場合)。</span><span class="sxs-lookup"><span data-stu-id="80f26-p110">The following example shows the SOAP response that is returned by the server after it parses the request from the client. The response contains only the settings that are requested, if they exist.</span></span>
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>15</h:MajorVersion>
      <h:MinorVersion>0</h:MinorVersion>
      <h:MajorBuildNumber>160</h:MajorBuildNumber>
      <h:MinorBuildNumber>4</h:MinorBuildNumber>
      <h:Version>Exchange2013</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <UserResponses>
          <UserResponse>
            <ErrorCode>NoError</ErrorCode>
            <ErrorMessage>No error.</ErrorMessage>
            <RedirectTarget i:nil="true" />
            <UserSettingErrors />
            <UserSettings>
              <UserSetting i:type="StringSetting">
                <Name>UserDisplayName</Name>
                <Value>Mara Whitley</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>UserDN</Name>
                <Value>/o=microsoft/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Recipients/cn=mara</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>UserDeploymentId</Name>
                <Value>649d50b8-a1ce-4bac-8ace-2321   e463f701</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>CasVersion</Name>
                <Value>15.01.0160.004</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>EwsSupportedSchemas</Name>
                <Value>Exchange2007, Exchange2007_SP1, Exchange2010, Exchange2010_SP1, Exchange2010_SP2, Exchange2013</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>InternalMailboxServer</Name>
                <Value>mail.contoso.com</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>ActiveDirectoryServer</Name>
                <Value>dc.contoso.com</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>MailboxDN</Name>
                <Value>/o=microsoft/ou=Exchange Administrative Group 
                  (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=mail.contoso.com/cn=Contoso Private MDB</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>PublicFolderServer</Name>
                <Value>public.contoso.com</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>EcpDeliveryReportUrlFragment</Name>
                <Value>PersonalSettings/DeliveryReport.aspx?exsvurl=1&amp;amp;IsOWA=&amp;lt;IsOWA&amp;gt;&amp;amp;MsgID=&amp;lt;MsgID&amp;gt;&amp;amp;Mbx=&amp;lt;Mbx&amp;gt;</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>EcpTextMessagingUrlFragment</Name>
                <Value>?p=sms/textmessaging.slab&amp;amp;exsvurl=1</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>EcpPublishingUrlFragment</Name>
                <Value>customize/calendarpublishing.slab?exsvurl=1&amp;amp;FldID=&amp;lt;FldID&amp;gt;</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>ExternalEwsUrl</Name>
                <Value>https://mail.contoso.com/EWS/Exchange.asmx</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>ExternalMailboxServer</Name>
                <Value>mail.contoso.com</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>GroupingInformation</Name>
                <Value>CONTOSO-1</Value>
              </UserSetting>
            </UserSettings>
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope
```

## <a name="get-user-settings-by-using-pox-autodiscover"></a><span data-ttu-id="80f26-141">POX 自動検出を使用してユーザー設定を取得する</span><span class="sxs-lookup"><span data-stu-id="80f26-141">Get user settings by using POX Autodiscover</span></span>
<span data-ttu-id="80f26-142"><a name="bk_POX"> </a></span><span class="sxs-lookup"><span data-stu-id="80f26-142"></span></span>

<span data-ttu-id="80f26-143">SOAP の自動検出 web サービスを使用することをお勧めします、POX の自動検出 web サービスは SOAP が使用できない場合のための適切なバックアップ オプション。</span><span class="sxs-lookup"><span data-stu-id="80f26-143">Although we recommend that you use the SOAP Autodiscover web service, the POX Autodiscover web service is a good backup option for those times when SOAP isn't available.</span></span> <span data-ttu-id="80f26-144">POX の自動検出 web サービスを使用する Exchange 2007 を対象とする場合があるので、2007 は、SOAP の自動検出 web サービスをサポートしていないを交換します。</span><span class="sxs-lookup"><span data-stu-id="80f26-144">For example, Exchange 2007 does not support the SOAP Autodiscover web service, so if you are targeting Exchange 2007, you have to use the POX Autodiscover web service.</span></span> <span data-ttu-id="80f26-145">SOAP の自動検出 web サービスとは異なり POX の自動検出サービスはできません固有の設定を要求します。</span><span class="sxs-lookup"><span data-stu-id="80f26-145">Unlike the SOAP Autodiscover web service, the POX Autodiscover service does not allow you to request specific settings.</span></span> <span data-ttu-id="80f26-146">代わりに、サーバーは、すべての[プロトコル要素](http://msdn.microsoft.com/library/f77e4d66-6fdd-4999-9339-f7d7f9c86f44%28Office.15%29.aspx)の子要素として使用可能な設定の一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="80f26-146">Instead, the server returns a full list of available settings as child elements of the [Protocol element](http://msdn.microsoft.com/library/f77e4d66-6fdd-4999-9339-f7d7f9c86f44%28Office.15%29.aspx).</span></span>
  
<span data-ttu-id="80f26-p112">次の例では、サーバーからユーザー設定を取得する SOAP の自動検出要求を示しています。次の XML は、HTTP POST 経由でサーバーに送信されます。</span><span class="sxs-lookup"><span data-stu-id="80f26-p112">The following example shows a POX Autodiscover request to get user settings from the server. The following XML is sent to the server via an HTTP POST.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>mara@contoso.com</EMailAddress>
    <AcceptableResponseSchema>http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

<span data-ttu-id="80f26-149">次の例は、サーバーに返される POX の応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="80f26-149">The following example shows the POX response that is returned by the server.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    <User>
      <DisplayName>Mara Whitley</DisplayName>
      <LegacyDN>/o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Recipients/cn=f5eeabead90d4b6fb51d6379474692cd-Mara</LegacyDN>
      <AutoDiscoverSMTPAddress>mara@contoso.com</AutoDiscoverSMTPAddress>
      <DeploymentId>50817eff-b925-4578-a0db-13bfc635e7a5</DeploymentId>
    </User>
    <Account>
      <AccountType>email</AccountType>
      <Action>settings</Action>
      <MicrosoftOnline>False</MicrosoftOnline>
      <Protocol>
        <Type>EXCH</Type>
        <Server>5f76be3c-9138-4f66-85e0-21bc23ca35f0@contoso.com</Server>
        <ServerDN>/o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=5f76be3c-9138-4f66-85e0-21bc23ca35f0@contoso.com</ServerDN>
        <ServerVersion>73C08204</ServerVersion>
        <MdbDN>/o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=5f76be3c-9138-4f66-85e0-21bc23ca35f0@contoso.com/cn=Microsoft Private MDB</MdbDN>
        <PublicFolderServer>public.contoso.com</PublicFolderServer>
        <AD>dc.contoso.com</AD>
        <ASUrl>https://mail.contoso.com/EWS/Exchange.asmx</ASUrl>
        <EwsUrl>https://mail.contoso.com/EWS/Exchange.asmx</EwsUrl>
        <EmwsUrl>https://mail.contoso.com/EWS/Exchange.asmx</EmwsUrl>
        <EcpUrl>https://mail.contoso.com/ecp/</EcpUrl>
        <EcpUrl-um>?rfr=olk&amp;amp;p=customize/voicemail.aspx&amp;amp;exsvurl=1&amp;amp;realm=contoso.com</EcpUrl-um>
        <EcpUrl-aggr>?rfr=olk&amp;amp;p=personalsettings/EmailSubscriptions.slab&amp;amp;exsvurl=1&amp;amp;realm=contoso.com</EcpUrl-aggr>
        <EcpUrl-mt>PersonalSettings/DeliveryReport.aspx?rfr=olk&amp;amp;exsvurl=1&amp;amp;IsOWA=&amp;lt;IsOWA&amp;gt;&amp;amp;MsgID=&amp;lt;MsgID&amp;gt;&amp;amp;Mbx=&amp;lt;Mbx&amp;gt;&amp;amp;realm=contoso.com</EcpUrl-mt>
        <EcpUrl-ret>?rfr=olk&amp;amp;p=organize/retentionpolicytags.slab&amp;amp;exsvurl=1&amp;amp;realm=contoso.com</EcpUrl-ret>
        <EcpUrl-sms>?rfr=olk&amp;amp;p=sms/textmessaging.slab&amp;amp;exsvurl=1&amp;amp;realm=contoso.com</EcpUrl-sms>
        <EcpUrl-publish>customize/calendarpublishing.slab?rfr=olk&amp;amp;exsvurl=1&amp;amp;FldID=&amp;lt;FldID&amp;gt;&amp;amp;realm=contoso.com</EcpUrl-publish>
        <EcpUrl-photo>PersonalSettings/EditAccount.aspx?rfr=olk&amp;amp;chgPhoto=1&amp;amp;exsvurl=1&amp;amp;realm=contoso.com</EcpUrl-photo>
        <EcpUrl-tm>?rfr=olk&amp;amp;ftr=TeamMailbox&amp;amp;exsvurl=1&amp;amp;realm=contoso.com</EcpUrl-tm>
        <EcpUrl-tmCreating>?rfr=olk&amp;amp;ftr=TeamMailboxCreating&amp;amp;SPUrl=&amp;lt;SPUrl&amp;gt;&amp;amp;Title=&amp;lt;Title&amp;gt;&amp;amp;SPTMAppUrl=&amp;lt;SPTMAppUrl&amp;gt;&amp;amp;exsvurl=1&amp;amp;realm=contoso.com</EcpUrl-tmCreating>
        <EcpUrl-tmEditing>?rfr=olk&amp;amp;ftr=TeamMailboxEditing&amp;amp;Id=&amp;lt;Id&amp;gt;&amp;amp;exsvurl=1&amp;amp;realm=contoso.com</EcpUrl-tmEditing>
        <EcpUrl-extinstall>Extension/InstalledExtensions.slab?rfr=olk&amp;amp;exsvurl=1&amp;amp;realm=contoso.com</EcpUrl-extinstall>
        <OOFUrl>https://mail.contoso.com/EWS/Exchange.asmx</OOFUrl>
        <UMUrl>https://mail.contoso.com/EWS/UM2007Legacy.asmx</UMUrl>
        <OABUrl>https://mail.contoso.com/OAB/c21c7bc2-53b3-4ddc-ad89-1219b486c37c/</OABUrl>
        <ServerExclusiveConnect>off</ServerExclusiveConnect>
      </Protocol>
      <Protocol>
        <Type>EXPR</Type>
        <Server>mail.contoso.com</Server>
        <SSL>Off</SSL>
        <AuthPackage>Ntlm</AuthPackage>
        <ServerExclusiveConnect>on</ServerExclusiveConnect>
        <CertPrincipalName>None</CertPrincipalName>
      </Protocol>
      <Protocol>
        <Type>WEB</Type>
        <Internal>
          <OWAUrl AuthenticationMethod="Basic, Fba">https://mail.contoso.com/owa/</OWAUrl>
          <Protocol>
            <Type>EXCH</Type>
            <ASUrl>https://mail.contoso.com/EWS/Exchange.asmx</ASUrl>
          </Protocol>
        </Internal>
      </Protocol>
    </Account>
  </Response>
</Autodiscover>
```

## <a name="next-steps"></a><span data-ttu-id="80f26-150">次の手順</span><span class="sxs-lookup"><span data-stu-id="80f26-150">Next steps</span></span>
<span data-ttu-id="80f26-151"><a name="bk_Next"> </a></span><span class="sxs-lookup"><span data-stu-id="80f26-151"></span></span>

<span data-ttu-id="80f26-152">サーバーからユーザーのために必要な構成の詳細を取得した後は、アプリケーションが必要な処理を実行する Exchange との通信ができています。</span><span class="sxs-lookup"><span data-stu-id="80f26-152">After you've retrieved the necessary configuration details for your user from the server, you are ready to communicate with Exchange to do the things your application needs to do.</span></span> <span data-ttu-id="80f26-153">次のステップは、Exchange と通信する方法と、実行する内容によって異なります。</span><span class="sxs-lookup"><span data-stu-id="80f26-153">What you do next depends on how you communicate with Exchange and what you want to accomplish.</span></span> <span data-ttu-id="80f26-154">によって、インスピレーションを提供する必要があり、EWS を使用している場合は、いくつかのアイデアの[交換 101 のコード サンプル](http://code.msdn.microsoft.com/exchange/Exchange-2013-101-Code-3c38582c)を表示する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="80f26-154">If you need some inspiration, and you're using EWS, you might explore the [Exchange 101 code samples](http://code.msdn.microsoft.com/exchange/Exchange-2013-101-Code-3c38582c) for some ideas.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="80f26-155">関連項目</span><span class="sxs-lookup"><span data-stu-id="80f26-155">See also</span></span>


- [<span data-ttu-id="80f26-156">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="80f26-156">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)
    
- [<span data-ttu-id="80f26-157">Exchange Web サービス (EWS) の管理の API</span><span class="sxs-lookup"><span data-stu-id="80f26-157">Exchange Web Services (EWS) Managed API</span></span>](http://msdn.microsoft.com/ja-jp/library/exchange/jj220535%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="80f26-158">Exchange の自動検出 web サービスの参照が SOAP します。</span><span class="sxs-lookup"><span data-stu-id="80f26-158">SOAP Autodiscover web service reference for Exchange</span></span>](http://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx)
    
- [<span data-ttu-id="80f26-159">Exchange の POX の自動検出 web サービスの参照</span><span class="sxs-lookup"><span data-stu-id="80f26-159">POX Autodiscover web service reference for Exchange</span></span>](http://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx)
    

