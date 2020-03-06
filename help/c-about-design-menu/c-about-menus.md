---
description: メニューを使用して、プレゼンテーションレイヤーをカスタマイズできます。
seo-description: メニューを使用して、プレゼンテーションレイヤーをカスタマイズできます。
seo-title: メニューについて
solution: Target
subtopic: Navigation
title: メニューについて
topic: Design,Site search and merchandising
uuid: 011050cd-21b6-4150-9503-18fa3f771626
translation-type: tm+mt
source-git-commit: ef818327e1cdaad79ac47575a8dfba1de3dc5c2e

---


# メニューについて{#about-menus}

メニューを使用して、プレゼンテーションレイヤーをカスタマイズできます。

## メニューの使用 {#concept_68123CE5CF4447B59217B5D721424E32}

検索内の設定にマップするメニューを追加します。 メニュー内の各項目は、メニューの設定の値を指定します。 メニューラベルをカスタマイズすることもできます。

プレゼンテーションテンプレートで、定義されたメニューを参照できます。 その後、必要な任意のHTMLコンポーネント（選択コントロールなど）に配置できます。 この組み合わせにより、ユーザは検索結果をカスタマイズできます。 次の3種類のメニューがサポートされています。並べ替え、カウント、ナビゲーション。

## Adding a new menu {#task_EE171532D3AE477FAFE8C2F4077A6D73}

検索結果内の設定にマップするメニューを追加できます。

<!-- 

t_adding_a_new_menu.xml

 -->

>[!NOTE]
>
>Webサイトに表示されるように、プレゼンテーションテンプレートでメニューを参照してください。

**新しいメニューを追加するには**

1. 製品メニューで//をクリ **[!UICONTROL Design]** ックし **[!UICONTROL Navigation]** ます **[!UICONTROL Menus]**。
1. ページ上で、 [!DNL Menus] をクリックしま **[!UICONTROL Add New Menu]**&#x200B;す。
1. ページ [!DNL Add Menu] で、必要なオプションを設定します。

   これらの設定は、階層リンクの動作とデフォルト表示の両方に影響します。 これらの設定の一部は、プレゼンテーションテンプレートの設定を使用して上書きできます。

   メニューにつ [いてを参照してくださ](../c-about-design-menu/c-about-menus.md#concept_68123CE5CF4447B59217B5D721424E32)い。

   <!-- 
   r_add_menu_options.xml
   -->

   <table> 
    <thead> 
      <tr> 
      <th colname="col1" class="entry"> <p>オプション </p> </th> 
      <th colname="col2" class="entry"> <p>説明 </p> </th> 
      </tr> 
    </thead>
    <tbody> 
      <tr> 
      <td colname="col1"> <p>メニュー名 </p> </td> 
      <td colname="col2"> <p>メニューの名前。 </p> </td> 
      </tr> 
      <tr> 
      <td colname="col1"> <p>メニューの種類 </p> </td> 
      <td colname="col2"> <p>次の3種類のメニューのいずれかを設定します。 </p> <p> 
      <ul id="ul_7E66ACC1DA494B20BEC3B0B2CCAB103A"> 
      <li id="li_D81876660A8B48AFB70D3317063FBF6F"> <span class="uicontrol"> 並べ替え </span> <p>定義済みのメタデータタイプで検索を整理します。 </p> <p>例えば、次のメタデータタイプを使用して並べ替えメニューを定義できます。関連性の3項目可用性コードなどのカスタムメタデータフィールド価格 この3つの項目には、それぞれ「関連性順」、「可用性順」、「価格順」というラベルを付けることができます。 プレゼンテーションテンプレートにこれを含めると、顧客はこのコントロールを使用して検索結果を並べ替えることができます。 </p> </li> 
      <li id="li_63AE06B544B64DCAA8C55031B3DFFFF7"> <span class="uicontrol"> カウント数 </span> <p>表示する検索結果の数を定義します。 このメニュータイプは、cgiパラメータ <span class="varname"> sp_cに対応していま </span>す。 </p> <p>バックエンド <a href="../c-appendices/c-cgiparameters.md#reference_582E85C3886740C98FE88CA9DF7918E8" format="dita" scope="local"> 検索のCGIパラメーターを参照してくだ </a>さい。 </p> </li> 
      <li id="li_EEC810D420FF41498ECE49EBAAB33BE5"> <span class="uicontrol"> ナビゲーション </span> <p>メニュー項目に関連付けられた静的URLのセットを指定します。 通常、検索結果ページに最上位レベルのナビゲーションバーを作成するには、ナビゲーションメニューを使用します。 </p> <p>例えば、次のようなメニュー項目を持つ女性、男性、男性、女性を含むメニューを作成できます。 
      <userinput>
        /?q1=womens;x1=gender 
      </userinput>、 
      <userinput>
        /?q1=mens;x1=gender 
      </userinput> </p> </li> 
      </ul> </p> </td> 
      </tr> 
      <tr> 
      <td colname="col1"> <p>マーチャンダイジング </p> 
        <!--DONT' KNOW WHAT THIS DOES--> </td> 
      <td colname="col2"> <p>このオプションは、メニューの種類として「並べ替え」を選択した場合にのみ使用 <span class="uicontrol"> できます。 </span> </p> </td> 
      </tr> 
      <tr> 
      <td colname="col1"> <p>メニュー内の項目数 </p> </td> 
      <td colname="col2"> <p>メニュー内の項目数を指定します。 この設定を変更すると、フォームのフィールドが追加または削除されます。 </p> </td> 
      </tr> 
      <tr> 
      <td colname="col1"> <p>既定の項目 </p> </td> 
      <td colname="col2"> <p>デフォルトで表示するメニュー項目を選択できます。 </p> </td> 
      </tr> 
      <tr> 
      <td colname="col1"> <p>項目の値 </p> </td> 
      <td colname="col2"> <p>項目の値は、設定したメニューの種類によって異なります。 </p> 
        <ul id="ul_2F14E6AA673640578A2D5161FD9D13EF"> 
        <li id="li_5017EC6E4ACB4B8E99E0AA61CBAAFFAE"> 並べ替えメニューの種類 <p>メニューで選択した項目を並べ替える基準を指定します。 選択した項目には、並べ替え可能なメタデータフィールドが入力されます。 </p> <p>1つの項目に対して、3つのメタデータフィールドで並べ替えを行うことができます。 並べ替えは、指定された順序で行われます。 </p> </li> 
        <li id="li_CC6BAFBF969C4367A71B55F08E0758D1"> カウントメニューの種類 <p>顧客がこのメニュー項目を選択した場合に返す結果の数を指定できます。 </p> </li> 
        </ul> </td> 
      </tr> 
      <tr> 
      <td colname="col1"> <p>項目のラベル </p> </td> 
      <td colname="col2"> <p>項目のラベルは、設定したメニューの種類によって異なります。 </p> 
        <ul id="ul_957BF01235F84748B5EB7062D6AEAC41"> 
        <li id="li_03FB2E2C96134A2B8E08154F87F0CD55"> 並べ替えメニューの種類 <p>顧客がメニューでこの品目を表示する際に表示するカスタムラベルを指定します。 </p> </li> 
        <li id="li_C9FE2BC46D9443FB85FEB837C7CA45E1"> カウントメニューの種類 <p>このメニュー項目に表示するカスタムラベルを指定します。 </p> </li> 
        </ul> </td> 
      </tr> 
    </tbody> 
    </table>

1. クリック **[!UICONTROL Add]**.
1. （オプション）ページ [!DNL Menus] で、次のいずれかの操作を行います。

   * 変更を **[!UICONTROL History]** 元に戻すには、をクリックします。

      詳しくは、「 [履歴」オプションの使用を参照してくださ](../t-using-the-history-option.md#task_70DD3F87A67242BBBD2CB27156F43002)い。

   * クリック **[!UICONTROL Live]**.

      ライブ設 [定の表示を参照してください](../c-about-staging.md#task_401A0EBDB5DB4D4CA933CBA7BECDC10F)。

   * クリック **[!UICONTROL Push Live]**.

      詳しくは、ス [テージ設定をライブにプッシュするを参照してくださ](../c-about-staging.md#task_44306783B4C0408AAA58B471DAF2D9A4)い。

## メニューの編集 {#task_0770DBFD0C7046169097FB6F771B9114}

追加したメニューの設定は編集できます。

<!-- 

t_editing_a_menu.xml

 -->

>[!NOTE]
>
>Webサイトに表示されるように、プレゼンテーションテンプレートでメニューを参照してください。

**メニューを編集するには**

1. 製品メニューで//をクリ **[!UICONTROL Design]** ックし **[!UICONTROL Navigation]** ます **[!UICONTROL Menus]**。
1. ページ [!DNL Menus] で、メニュー名の **[!UICONTROL Edit]** 右端にあるをクリックします。
1. ページ [!DNL Edit Menu] で、必要なオプションを設定します。

   新しいメニューの追加のオプションの [表を参照してください](../c-about-design-menu/c-about-menus.md#task_EE171532D3AE477FAFE8C2F4077A6D73)。
1. クリック **[!UICONTROL Save Changes]**.
1. （オプション）ページ [!DNL Menus] で、次のいずれかの操作を行います。

   * 変更を **[!UICONTROL History]** 元に戻すには、をクリックします。

      詳しくは、「 [履歴」オプションの使用を参照してくださ](../t-using-the-history-option.md#task_70DD3F87A67242BBBD2CB27156F43002)い。

   * クリック **[!UICONTROL Live]**.

      ライブ設 [定の表示を参照してください](../c-about-staging.md#task_401A0EBDB5DB4D4CA933CBA7BECDC10F)。

   * クリック **[!UICONTROL Push Live]**.

      詳しくは、ス [テージ設定をライブにプッシュするを参照してくださ](../c-about-staging.md#task_44306783B4C0408AAA58B471DAF2D9A4)い。

## メニューの削除 {#task_645E212311A045CD8D9D906878165F47}

追加したメニューは削除できます。

<!-- 

t_deleting_a_menu.xml

 -->

**メニューを削除するには**

1. 製品メニューで、//をクリ **[!UICONTROL Design]** ックしま **[!UICONTROL Navigation]** す **[!UICONTROL Menus]**
1. ページ [!DNL Menus] で、メニュー名の **[!UICONTROL Delete]** 右端にあるをクリックします。
1. ダイアログボッ [!DNL Confirmation] クスで、をクリックしま **[!UICONTROL OK]**&#x200B;す。
1. （オプション）次のいずれかの操作を行います。

   * 変更を **[!UICONTROL History]** 元に戻すには、をクリックします。

      詳しくは、「 [履歴」オプションの使用を参照してくださ](../t-using-the-history-option.md#task_70DD3F87A67242BBBD2CB27156F43002)い。

   * クリック **[!UICONTROL Live]**.

      ライブ設 [定の表示を参照してください](../c-about-staging.md#task_401A0EBDB5DB4D4CA933CBA7BECDC10F)。

   * クリック **[!UICONTROL Push Live]**.

      詳しくは、ス [テージ設定をライブにプッシュするを参照してくださ](../c-about-staging.md#task_44306783B4C0408AAA58B471DAF2D9A4)い。
