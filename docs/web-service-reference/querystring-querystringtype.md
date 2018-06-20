---
title: クエリ文字列 (QueryStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- QueryString
api_type:
- schema
ms.assetid: cadbf9a5-b87e-4d7f-b488-b76fb0ee7150
description: クエリ文字列要素には、ベースの高度なクエリ構文 (AQS) のメールボックスのクエリ文字列が含まれています。
ms.openlocfilehash: 410405638b3f8628dc589049873cfea1f153310c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832943"
---
# <a name="querystring-querystringtype"></a>クエリ文字列 (QueryStringType)

**クエリ文字列**要素には、ベースの高度なクエリ構文 (AQS) のメールボックスのクエリ文字列が含まれています。 
  
```XML
<QueryString/>
```

 **QueryStringType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ResetCache  <br/> |キャッシュをリセットする必要があることを示します。  <br/> |
|ReturnDeletedItems  <br/> |削除済みアイテムが返されることを示します。  <br/> |
|ReturnHighlightTerms  <br/> |強調表示されている用語が返されることを示します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |メールボックス内のアイテムを検索するための要求を定義します。  <br/> 次は、この要素の XPath 式:/FindItem。  <br/> |
   
## <a name="text-value"></a>テキスト値

**クエリ文字列**要素のテキスト値は、[高度なクエリ構文 (AQS)](http://msdn.microsoft.com/en-us/library/aa965711%28VS.85%29.aspx)のサブセットを使用して作成されるメールボックスのクエリを表します。 クエリ文字列の構文がサポートされているオプションの詳細については「解説」セクションを参照してください。
  
## <a name="remarks"></a>備考

Exchange Server 2010 では、この要素は、XML スキーマの文字列の種類をします。 バージョンの Exchange が Exchange Server 2013 で始まる、 **QueryStringType**は、Exchange オンライン、この要素の型を含みます。 3 つの新しいオプション属性を追加するため、この変更は既存のクライアントを中断しません。 
  
**クエリ文字列**要素は、EWS の制限の使用を除外します。 EWS で AQS の 3 種類の制限をサポートしています: word のフェーズの制限、日付範囲の制限、およびメッセージの種類の制限です。 次の表は、制限の種類ごとにサポートされている検索プロパティを一覧表示します。 
  
**Word フェーズの制限**

|**プロパティ**|**例**|**�֐�**|
|:-----|:-----|:-----|
|from  <br/> |: 学部長  <br/> :「Dean ハルステッド」  <br/> |Dean から送信されたアイテムを検索します。  <br/> Dean ハルステッドから送信されたアイテムを検索します。 送信者は、正確に「Dean ハルステッド」である必要があります。  <br/> |
|の行を  <br/> |: 学部長  <br/> |Dean に送信されたアイテムを検索します。  <br/> |
|cc  <br/> |Cc:Dean  <br/> |[Cc] 行の Dean でアイテムを検索します。  <br/> |
|bcc  <br/> |Bcc:Dean  <br/> |[Bcc] 行の Dean でアイテムを検索します。  <br/> |
|Participants  <br/> |参加者: 学部長  <br/> |フィールドを Dean でアイテムを [宛先] ボックス、[cc]、または [bcc] に検索します。  <br/> |
|件名  <br/> |件名: 商品  <br/> 件名:(product development)  <br/> 件名:「製品開発」  <br/> |件名に製品を持つアイテムを検索します。  <br/> 製品と開発の主題にアイテムを検索します。  <br/> |
|本文  <br/> コンテンツ  <br/> |本文: 進行状況  <br/> : 進行中のコンテンツ  <br/> |本文の中でアイテムを検索します。  <br/> |
|Attachment  <br/> |添付ファイル: レポート  <br/> |添付ファイルのファイル名またはファイルの本文にレポート アイテムを検索します。  <br/> |
|(プロパティが指定されていません)  <br/> |製品の開発  <br/> |製品と開発の両方で word のすべてのフェーズ プロパティを含む項目を検索します。  <br/> |
   
一致する単語の段階の制限は、常に大文字小文字を区別します。 Word フェーズの制限は、2 つの一致の種類をサポートしています: プレフィックスの一致または完全に一致します。 プレフィックスの一致は、マッチの既定の動作です。 正確に一致する場合は、二重引用符を使用します。 たとえば、件名:「製品」は、'製品' がない '' 内での生産、件名と一致します。 複数の単語を二重引用符では、word のフェーズとその順序の両方を制限します。 たとえば"win 製品"は、唯一の 'win 製品'、'win95 製品ではない' または '勝利の製品' と一致します。 アスタリスクを使用することができます (\*) 順で制限されているプレフィックスの一致を定義します。 たとえば、「win 製品」\* 'win95 製品'、' windows 生産ライン ' がない 'windows の新製品' または '勝利の製品' と一致します。 またはドメインから送信されたすべてのメッセージを検索することができます。 たとえば、from:"@hotmail.com"は、hotmail.com から送信されたすべてのメッセージを返します。
  
次の表では、日付の範囲の制限について説明します。
  
**日付範囲の制限**

|**プロパティ**|**例**|**�֐�**|
|:-----|:-----|:-----|
|Sent  <br/> |送信: 最後の週  <br/> 送信: 2001 年 01 月 01 日  <br/> Sent:01/01/2001..01/15/2001  <br/> |検索項目は、最後の週を送信します。  <br/> 2001 年 1 月 1 日に送信されたアイテムを検索します。  <br/> 2001 年 1 月 1 日と 2001 年 1 月 15 日の間で送信されたアイテムを検索します。  <br/> |
|Received  <br/> |受信しました: 今日  <br/> 受信: 2001 年 01 月 01 日  <br/> |今日受信したアイテムを検索します。  <br/> 2001 年 1 月 1 日に受信したアイテムを検索します。  <br/> |
   
2 つのドット (.) は、範囲演算子です。 開始日と終了日の範囲を定義して使用できます。 日付を指定するには、相対的な日付を使用できます。 次の相対日付がサポートされています。
  
- 相対日時: 今日、明日、昨日
    
- 語の相対日付: 今週、来月、先週、過去の月、または今後 1 年以内
    
- 曜日: 日曜日、月曜日、火曜日、水曜日、木曜日、金曜日、土曜日
    
- 年 1 月、2 月、3 月 4 月、可能性があります、6 月、7 月、8 月、9 月、10 月、11 月、年 12 月
    
次の表では、メッセージの種類の制限について説明します。 
  
**メッセージの種類の制限**

|**プロパティ**|**例**|**�֐�**|
|:-----|:-----|:-----|
|種類  <br/> |タスクの種類:  <br/> |すべての作業項目を検索します。  <br/> |
   
AQS EWS では、メッセージの種類を指定するのには**Kind**プロパティを使用します。 Kind プロパティは、次の項目の種類で使用できます。 
  
- email
    
- 会議
    
- tasks
    
- notes
    
- docs
    
- journals
    
- contacts
    
- im
    
論理コネクタをグループ化を次の表に示します。
  
**論理コネクタをグループ化**

|**コネクタ**|**例**|**�֐�**|
|:-----|:-----|:-----|
|AND  <br/> |件名: 製品および件名: 開発  <br/> 件名:(product AND development)  <br/> 件名:(product development)  <br/> |件名に製品と開発の両方を持つアイテムを検索します。  <br/> |
|OR  <br/> |本文: プロジェクトまたは本文: 提案  <br/> 本文:(project OR proposal)  <br/> |本文の製品や開発のいずれかの項目を検索します。  <br/> |
|NOT  <br/> |本文: 提案のないです。  <br/> 本文:(NOT proposal)  <br/> |提案なしのメッセージ本文の検索をします。  <br/> |
   
デフォルトのコネクタは、常にします。 など: プロジェクトの件名と本文: 提案は、プロジェクトの件名: 本文: 提案と同じ。 論理コネクタでは、大文字小文字を区別します。 本文の例では、:(project Or proposal) 'プロジェクト'、メッセージの検索 'または' と '' 'プロジェクト' または '提案' ではなく本文にします。 プラス記号 (+) のと同じです。 ハイフン記号 (-) は、NOT と同じです。 本文の例では、:(project-proposal)、本文に 'プロジェクト'、'提案' なしのメッセージを検索します。 
  
クエリ文字列は、検索用インデックス付けされていないプロパティを含めることもできます。 クエリ文字列にインデックス付けされていないプロパティが含まれている場合、検索は、インデックス付きのプロパティと、ストア、インデックス付けされていないプロパティの検索に Exchange 検索を実行する可能性があります。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="example"></a>例

件名に自動検出と、受信トレイでメッセージを検索するための要求の例を次に示します。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="1" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
      <m:QueryString>subject:Autodiscover</m:QueryString>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

要求に正常な応答の例を次に示します。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="20" 
                         Version="Exchange2010" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1" 
                        TotalItemsInView="5" 
                        IncludesLastItemInRange="false">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkADEzOTExYjJkLTYx" ChangeKey="CQAAABY" />
                <t:Subject>How to use Autodiscover</t:Subject>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目




  [FindItem 操作](finditem-operation.md)
  

  [FindConversation 操作](findconversation-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

