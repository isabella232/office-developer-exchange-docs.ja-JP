---
title: 自動検出を使用して Exchange からユーザー設定を取得する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 6d90c305-4802-4e18-8d52-f60349feaa8d
description: 自動検出を使用して Exchange サーバーからユーザー構成設定を取得する方法について説明します。
localization_priority: Priority
ms.openlocfilehash: 5f7ea04e6b04f674d4cb481cf9243d46437d6950
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528000"
---
# <a name="get-user-settings-from-exchange-by-using-autodiscover"></a><span data-ttu-id="5dbd0-103">自動検出を使用して Exchange からユーザー設定を取得する</span><span class="sxs-lookup"><span data-stu-id="5dbd0-103">Get user settings from Exchange by using Autodiscover</span></span>

<span data-ttu-id="5dbd0-104">自動検出を使用して Exchange サーバーからユーザー構成設定を取得する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-104">Learn how to get user configuration settings from an Exchange server by using Autodiscover.</span></span>
  
<span data-ttu-id="5dbd0-105">自動検出では、ユーザーの電子メール アドレスとパスワードだけを使用して、ユーザーの構成情報に簡単にアクセスできるようにすることで、アプリケーションの構成が簡略化されます。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-105">Autodiscover simplifies application configuration by providing easy access to user configuration information using only the user's email address and password.</span></span> <span data-ttu-id="5dbd0-106">ユーザーの表示名や外部の Web サービスの URL など、[多くのユーザー構成設定](https://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx)が自動検出で利用できます。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-106">A [number of user configuration settings](https://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) are available via Autodiscover, such as the user's display name or external web service URL.</span></span> 
  
<span data-ttu-id="5dbd0-107">自動検出サービスからユーザーの設定を取得するために、次の開発テクノロジのうちのいずれかを使用できます。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-107">You can use one of the following development technologies to retrieve user settings from the Autodiscover service:</span></span>
  
- <span data-ttu-id="5dbd0-108">[EWS マネージ API クライアント アプリケーションの概要](get-started-with-ews-managed-api-client-applications.md)</span><span class="sxs-lookup"><span data-stu-id="5dbd0-108">The [Get started with EWS Managed API client applications](get-started-with-ews-managed-api-client-applications.md)</span></span>
    
- <span data-ttu-id="5dbd0-109">[SOAP 自動検出 Web サービス](https://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="5dbd0-109">The [SOAP Autodiscover web service](https://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx)</span></span>
    
- <span data-ttu-id="5dbd0-110">[POX 自動検出 Web サービス](https://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="5dbd0-110">The [POX Autodiscover web service](https://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx)</span></span>
    
<span data-ttu-id="5dbd0-111">EWS マネージ API は、ユーザー設定を取得するためのオブジェクト ベースのインターフェイスを提供します。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-111">The EWS Managed API provides an object-based interface for retrieving user settings.</span></span> <span data-ttu-id="5dbd0-112">クライアント アプリケーションがマネージ コードを使用する場合は、EWS マネージ API を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-112">If your client application uses managed code, we recommend that you use the EWS Managed API.</span></span> <span data-ttu-id="5dbd0-113">EWS マネージ API を使用している場合は、必要な設定が [Microsoft.Exchange.WebServices.Autodiscover.UserSettingName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.usersettingname%28v=EXCHG.80%29.aspx) 列挙型で利用可能かどうかを判別します。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-113">If you are using the EWS Managed API, determine whether the settings that you need are available in the [Microsoft.Exchange.WebServices.Autodiscover.UserSettingName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.usersettingname%28v=EXCHG.80%29.aspx) enumeration.</span></span> <span data-ttu-id="5dbd0-114">利用可能でない場合は、SOAP または POX の自動検出サービスの使用をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-114">If they aren't, you might want to use the SOAP or POX Autodiscover services.</span></span> 
  
<span data-ttu-id="5dbd0-115">Web サービスを使用している場合は、POX の自動検出サービスよりも豊富な機能をサポートしている SOAP の自動検出サービスの使用をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-115">If you are using a web service, we suggest that you use the SOAP Autodiscover service, because it supports a richer set of features than the POX Autodiscover service.</span></span> <span data-ttu-id="5dbd0-116">SOAP の自動検出サービスを使用できない場合、POX の自動検出サービスは代替として最適です。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-116">If the SOAP Autodiscover service isn't available, the POX Autodiscover service is a good alternative.</span></span>
  
## <a name="set-up-to-get-user-settings"></a><span data-ttu-id="5dbd0-117">ユーザー設定を取得するように設定する</span><span class="sxs-lookup"><span data-stu-id="5dbd0-117">Set up to get user settings</span></span>
<span data-ttu-id="5dbd0-118"><a name="bk_Prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="5dbd0-118"><a name="bk_Prereq"> </a></span></span>

<span data-ttu-id="5dbd0-119">自動検出サービスを使用してユーザー設定を取得する前に、次のものを使用しているか確認してください。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-119">Before you get user settings by using the Autodiscover service, make sure that you have access to the following:</span></span>
  
- <span data-ttu-id="5dbd0-120">EWS マネージ API または POX ベースの自動検出サービス、Exchange Online 、Office 365 の一部としての Exchange Online、または Exchange 2007 SP1 以降のバージョンの Exchange を実行しているサーバーを使用しているか。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-120">If you are using the EWS Managed API or the POX-based Autodiscover service, Exchange Online, Exchange Online as part of Office 365, or a server that is running a version of Exchange starting with Exchange 2007 SP1.</span></span> 
    
- <span data-ttu-id="5dbd0-121">SOAP ベースの自動検出サービス、Exchange Online、または Exchange 2010 以降のバージョンの Exchange を使用しているか。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-121">If you are using the SOAP-based Autodiscover service, Exchange Online or a version of Exchange starting with Exchange 2010.</span></span>
    
> [!NOTE]
> <span data-ttu-id="5dbd0-p104">EWS マネージ API を使用している場合は、状況によっては[証明書の検証コールバック メソッドを指定](how-to-validate-a-server-certificate-for-the-ews-managed-api.md)する必要があります。また、Visual Studio で作成されたものなど、生成されたいくつかのプロキシ ライブラリを使用した、証明書の検証コールバック メソッドが必要になる場合もあります。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-p104">If you are using the EWS Managed API, you will need to [provide a certificate validation callback method](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) in some circumstances. You might also need a certificate validation callback method with some generated proxy libraries, such as those created by Visual Studio.</span></span> 
  
## <a name="get-user-settings-by-using-the-ews-managed-api"></a><span data-ttu-id="5dbd0-124">EWS マネージ API を使用してユーザー設定を取得する</span><span class="sxs-lookup"><span data-stu-id="5dbd0-124">Get user settings by using the EWS Managed API</span></span>
<span data-ttu-id="5dbd0-125"><a name="bk_Managed"> </a></span><span class="sxs-lookup"><span data-stu-id="5dbd0-125"><a name="bk_Managed"> </a></span></span>

<span data-ttu-id="5dbd0-126">[GetUserSettings](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx) メソッドを使用して、次の例のように、ユーザーの構成情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-126">You can use the [GetUserSettings](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx) method to retrieve configuration information for a user, as shown in the following example.</span></span> <span data-ttu-id="5dbd0-127">この例では、([UserSettingName](https://msdn.microsoft.com/library/exchange/microsoft.exchange.webservices.autodiscover.usersettingname%28v=exchg.80%29.aspx) 列挙型で利用できるものから) 返されるユーザー設定の配列を指定でき、メソッドは Exchange サーバーからのリダイレクト応答に従います。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-127">In this example, you can specify an array of user settings to return (from those available in the [UserSettingName](https://msdn.microsoft.com/library/exchange/microsoft.exchange.webservices.autodiscover.usersettingname%28v=exchg.80%29.aspx) enumeration), and the method will follow redirection responses from the Exchange server.</span></span> 
  
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

<span data-ttu-id="5dbd0-p106">ユーザー設定の配列の各キー/値ペアにアクセスするために返されるコレクションを解析することができます。次の使用例は、返された各要素を解析し、各キー/値ペアの名前と値を表示する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-p106">You can parse the collection returned to access each key/value pair in the user settings array. The following example shows how to parse through each returned element and display the name and value of each key/value pair.</span></span>
  
```cs
// Display each retrieved value. The settings are part of a key/value pair.
// userresponse is a GetUserSettingsResonse object.
foreach (KeyValuePair<UserSettingName, Object> usersetting in userresponse.Settings)
{
    Console.WriteLine(usersetting.Key.ToString() + ": " + usersetting.Value);
}
```

<span data-ttu-id="5dbd0-130">または、特定の設定の値を取得できます。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-130">Alternatively, you can obtain the value of a specific setting.</span></span> <span data-ttu-id="5dbd0-131">次の例では、**UserDisplayName** の設定が表示されます。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-131">In the following example, the **UserDisplayName** setting is to be displayed.</span></span> 
  
```cs
// Display a specific setting, such as UserDisplayName.
Console.WriteLine(userresponse.Settings[UserSettingName.UserDisplayName]);
```

## <a name="get-user-settings-by-using-soap-autodiscover"></a><span data-ttu-id="5dbd0-132">SOAP 自動検出を使用してユーザー設定を取得する</span><span class="sxs-lookup"><span data-stu-id="5dbd0-132">Get user settings by using SOAP Autodiscover</span></span>
<span data-ttu-id="5dbd0-133"><a name="bk_SOAP"> </a></span><span class="sxs-lookup"><span data-stu-id="5dbd0-133"><a name="bk_SOAP"> </a></span></span>

<span data-ttu-id="5dbd0-p108">EWS マネージ API を使用していない場合は、SOAP の自動検出 Web サービスを使用することをお勧めします。SOAP の自動検出 Web サービスが失敗した、または利用できない場合にのみ、POX 自動検出 Web サービスを使用します。 </span><span class="sxs-lookup"><span data-stu-id="5dbd0-p108">If you're not using the EWS Managed API, we recommend that you use the SOAP Autodiscover web service. Only use the POX Autodiscover web service if the SOAP Autodiscover web service fails or is not available.</span></span> 
  
<span data-ttu-id="5dbd0-136">ユーザー設定を取得するには、[GetUserSettings 操作 (SOAP)](https://msdn.microsoft.com/library/758d965c-ef63-4de4-9120-e293abf14ff8%28Office.15%29.aspx) を使用します。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-136">To get user settings, use the [GetUserSettings operation (SOAP)](https://msdn.microsoft.com/library/758d965c-ef63-4de4-9120-e293abf14ff8%28Office.15%29.aspx).</span></span> <span data-ttu-id="5dbd0-137">指定された設定は [UserSetting 要素](https://msdn.microsoft.com/library/aac6dc31-edd2-49d7-b845-1df4d77da58c%28Office.15%29.aspx)として返されます。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-137">The requested settings are returned as [UserSetting elements](https://msdn.microsoft.com/library/aac6dc31-edd2-49d7-b845-1df4d77da58c%28Office.15%29.aspx).</span></span>
  
<span data-ttu-id="5dbd0-138">次の例では、サーバーからユーザー設定を取得する SOAP 自動検出要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-138">The following example shows a SOAP Autodiscover request to get user settings from the server.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://autodiscover.exchange.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover">
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

<span data-ttu-id="5dbd0-p110">次の例では、クライアントからの要求を解析した後に、サーバーによって返される SOAP 応答を示します。応答には、要求される設定のみが含まれます (存在する場合)。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-p110">The following example shows the SOAP response that is returned by the server after it parses the request from the client. The response contains only the settings that are requested, if they exist.</span></span>
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/" xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">https://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="https://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>15</h:MajorVersion>
      <h:MinorVersion>0</h:MinorVersion>
      <h:MajorBuildNumber>160</h:MajorBuildNumber>
      <h:MinorBuildNumber>4</h:MinorBuildNumber>
      <h:Version>Exchange2013</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover">
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

## <a name="get-user-settings-by-using-pox-autodiscover"></a><span data-ttu-id="5dbd0-141">POX 自動検出を使用してユーザー設定を取得する</span><span class="sxs-lookup"><span data-stu-id="5dbd0-141">Get user settings by using POX Autodiscover</span></span>
<span data-ttu-id="5dbd0-142"><a name="bk_POX"> </a></span><span class="sxs-lookup"><span data-stu-id="5dbd0-142"><a name="bk_POX"> </a></span></span>

<span data-ttu-id="5dbd0-143">SOAP の自動検出 Web サービスを使用することをお勧めしますが、POX の自動検出 Web サービスは、SOAP が使用できない場合のための適切なバックアップ オプションです。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-143">Although we recommend that you use the SOAP Autodiscover web service, the POX Autodiscover web service is a good backup option for those times when SOAP isn't available.</span></span> <span data-ttu-id="5dbd0-144">たとえば、Exchange 2007 は SOAP の自動検出 Web サービスをサポートしていないため、Exchange 2007 を対象としている場合は、POX の自動検出 Web サービスを利用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-144">For example, Exchange 2007 does not support the SOAP Autodiscover web service, so if you are targeting Exchange 2007, you have to use the POX Autodiscover web service.</span></span> <span data-ttu-id="5dbd0-145">SOAP の自動検出 Web サービスとは異なり、POX の自動検出サービスでは特定の設定を要求できません。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-145">Unlike the SOAP Autodiscover web service, the POX Autodiscover service does not allow you to request specific settings.</span></span> <span data-ttu-id="5dbd0-146">その代わりに、サーバーが [Protocol 要素](https://msdn.microsoft.com/library/f77e4d66-6fdd-4999-9339-f7d7f9c86f44%28Office.15%29.aspx)の子要素として、使用可能な設定の完全な一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-146">Instead, the server returns a full list of available settings as child elements of the [Protocol element](https://msdn.microsoft.com/library/f77e4d66-6fdd-4999-9339-f7d7f9c86f44%28Office.15%29.aspx).</span></span>
  
<span data-ttu-id="5dbd0-p112">次の例では、サーバーからユーザー設定を取得する SOAP の自動検出要求を示しています。次の XML は、HTTP POST 経由でサーバーに送信されます。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-p112">The following example shows a POX Autodiscover request to get user settings from the server. The following XML is sent to the server via an HTTP POST.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>mara@contoso.com</EMailAddress>
    <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

<span data-ttu-id="5dbd0-149">次の例は、サーバーに返される POX の応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-149">The following example shows the POX response that is returned by the server.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
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

## <a name="next-steps"></a><span data-ttu-id="5dbd0-150">次の手順</span><span class="sxs-lookup"><span data-stu-id="5dbd0-150">Next steps</span></span>
<span data-ttu-id="5dbd0-151"><a name="bk_Next"> </a></span><span class="sxs-lookup"><span data-stu-id="5dbd0-151"><a name="bk_Next"> </a></span></span>

<span data-ttu-id="5dbd0-152">サーバーからユーザーのために必要な構成の詳細を取得すると、アプリケーションで必要な処理を行うために Exchange と通信する準備ができたことになります。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-152">After you've retrieved the necessary configuration details for your user from the server, you are ready to communicate with Exchange to do the things your application needs to do.</span></span> <span data-ttu-id="5dbd0-153">次のステップは、Exchange と通信する方法や、行う内容によって異なります。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-153">What you do next depends on how you communicate with Exchange and what you want to accomplish.</span></span> <span data-ttu-id="5dbd0-154">いくらかインスピレーションが必要で、EWS を使用している場合は、アイデアを得るために、「[Exchange 101 のコード サンプル](https://code.msdn.microsoft.com/exchange/Exchange-2013-101-Code-3c38582c)」を確認することができます。</span><span class="sxs-lookup"><span data-stu-id="5dbd0-154">If you need some inspiration, and you're using EWS, you might explore the [Exchange 101 code samples](https://code.msdn.microsoft.com/exchange/Exchange-2013-101-Code-3c38582c) for some ideas.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="5dbd0-155">関連項目</span><span class="sxs-lookup"><span data-stu-id="5dbd0-155">See also</span></span>


- [<span data-ttu-id="5dbd0-156">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="5dbd0-156">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)
    
- [<span data-ttu-id="5dbd0-157">Exchange Web サービス (EWS) マネージ API</span><span class="sxs-lookup"><span data-stu-id="5dbd0-157">Exchange Web Services (EWS) Managed API</span></span>](https://msdn.microsoft.com/library/exchange/jj220535%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="5dbd0-158">Exchange 用 SOAP 自動検出 Web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="5dbd0-158">SOAP Autodiscover web service reference for Exchange</span></span>](https://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx)
    
- [<span data-ttu-id="5dbd0-159">Exchange 用 POX 自動検出 Web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="5dbd0-159">POX Autodiscover web service reference for Exchange</span></span>](https://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx)
    

