# 第2次隨堂-隨堂-QZ2
>
>學號：109111139
><br />
>姓名：繆昊廷 
><br />
>作業撰寫時間：20mins
><br />
>最後撰寫文件日期：2022/10/23
>

本份文件包含以下主題：(至少需下面兩項，若是有多者可以自行新增)
- [x]說明內容
- [x]個人認為完成作業須具備觀念

## 說明程式與內容

下段程式碼則為使用後結果：初始lb_Msg的Text顯示為Page_Load，當按鈕按下時，lb_Msg的Text顯示為btn_Event。

```csharp
protected void Page_Load(object sender, EventArgs e)
        {
            lb_Msg.Text = "Page_Load";
        }

        protected void btn_Submit_Click(object sender, EventArgs e)
        {
            lb_Msg.Text = "btn_Event";
        }
```


下段程式碼則為使用後結果：顯示id為lb_Msg的label和id為btn_Submit的按鈕，按鈕的文字為送出，高度和寬度為40px。

```html
<%@ Page Language="C#" AutoEventWireup="true" ...>

<!DOCTYPE html>

<html xmlns="http://www.w3.org/1999/xhtml">
<head runat="server">
<meta http-equiv="Content-Type" ...>
    <title></title>
</head>
<body>
    <form id="form1" runat="server">
        <div>
            <asp:Label ID="lb_Msg" runat="server"></asp:Label>
            <asp:Button ID="btn_Submit" runat="server" Text="送出" Width="40px" Height="40px" OnClick="btn_Submit_Click" />
        </div>
    </form>
</body>
</html>
```


## 個人認為完成作業須具備觀念

可以在右下角的屬性更改id或Text，程式執行時，會先執行Page_Load這段的程式，當按鈕按下時，會執行該按鈕按下的指令。

