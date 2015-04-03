---
title: OnTableDestroying
page_title: OnTableDestroying | UI for ASP.NET AJAX Documentation
description: OnTableDestroying
slug: grid/client-side-programming/events/events/ontabledestroying
tags: ontabledestroying
published: True
position: 75
---

# OnTableDestroying



## 

Sys.EventArgs OnTableDestroying Property

>note To get or set property values for client API properties, you must call property accessor methods that are named with the get_ and set_ prefixes. For example, to get or set a value for a property such as[cancel](http://msdn.microsoft.com/en-us/library/bb310859.aspx), you call the get_cancel or set_cancel.
>


This event is fired when table object is destroyed.


|  __Fired by__  | RadGrid |
| ------ | ------ |
| __Arguments__ |N/A|
| __Can be canceled__ |No|

Example:

````ASPNET
	    <telerik:RadGrid ID="RadGrid1" runat="server">
	        <ClientSettings>
	            <ClientEvents OnTableDestroying="TableDestroying" />
	        </ClientSettings>
	    </telerik:RadGrid>
````



````JavaScript
	        function TableDestroying(sender, eventArgs) {
	            alert("Destroying DetailTable with ClientID: " + sender.get_id());
	        }
````

