---
description: Instructions for adding the visual_sciences.dll to the Tomcat java library path.
seo-description: Instructions for adding the visual_sciences.dll to the Tomcat java library path.
seo-title: Modify the Java Library Path
title: Modify the Java Library Path
uuid: 564fa4d9-75b8-469f-ac4e-d9e081167355
index: y
internal: n
snippet: y
---

# Modify the Java Library Path{#modify-the-java-library-path}

Instructions for adding the visual_sciences.dll to the Tomcat java library path.

1. On your Windows server, navigate to Tomcat installation directory. (Tomcat > bin) 
1. Under bin folder, run Tomcat9w.exe (common daemon service manager).

In the Java tab, under Java options, add a new line:

```
-Djava.library.path=C:\Sensor directory
```

Where C:\Sensor directory is the directory containing the visual_sciences.dll file. 
