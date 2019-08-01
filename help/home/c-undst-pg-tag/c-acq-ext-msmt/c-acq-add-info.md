---
description: Query string variables may be added to a JavaScript request to collect additional measurements when a request is made.
seo-description: Query string variables may be added to a JavaScript request to collect additional measurements when a request is made.
seo-title: Acquiring Additional Information
solution: Analytics
title: Acquiring Additional Information
topic: Data workbench
uuid: b70a8677-3516-4373-951d-9a7e9c9e8a34
index: y
internal: n
snippet: y
---

# Acquiring Additional Information{#acquiring-additional-information}

Query string variables may be added to a JavaScript request to collect additional measurements when a request is made.

 These variables may be added manually or by script in the page itself.

Additional information that can be acquired from a page may be added to the embedded object via script using the following code as an example:

```
<!-- BEGIN REFERENCE PAGE TAG--> 
<script language="javascript"> 
var vlc = "0" //Capture Link Click  1=TRUE, 0=FALSE 
var v = {}; 
v["_pn"] = "Application Form"; 
v["_1"] = “99.99”; 
v["_2"] = "visa"; 
</script> 
 
<script language="javascript" src=”http://www.myserver.com/path/to/zig.js" type="text/javascript"></script> 
<noscript> 
 
<img src="/path/to/zag.gif?Log=1&v_jd=1" border="0" width="1" height="1"/> 
</noscript> 
<!-- END REFERENCE PAGE TAG-->
```

In this example, the script variables for v_1 and v_2 can be derived from another function within your web page. The variables have been inserted as examples. In addition to the baseline measurements acquired with each request, the following extended measurements would be acquired with the request of the URL above:

|  Data Collected  | Explanation  | Example  |
|---|---|---|
|  v_pn=  | Value associated with the v_pn query string variable  | v_pn=Application Form  |
|  v_1=  | Value associated with the v_1 query string variable  | v_1=99.99  |
|  v_2=  | Value associated with the v_2 query string variable  | v_2=visa  |

