<h1 align="center">  
 <img width="824" alt="HierarchyDecoratorNew" src="https://user-images.githubusercontent.com/31889435/226486126-009081e1-44de-465c-8ff7-5641870fdcae.png">
 
 Hierarchy Decorator (mgranddev fork)
</h1>

<h4 align="center"> Unity Editor plugin giving the Hierarchy a lick of paint.<br><br>
 
 Fully Customisable.<br>
 Toggle Everything.</h4>

<p align="center">
 <a href="https://unity3d.com/get-unity/download">
 <img src="https://img.shields.io/badge/unity-2018.4%2B-blue.svg" alt="Unity Download Link">
 <a href="https://github.com/mgranddev/hierarchy-decorator/blob/master/LICENSE.md">
 <img src="https://img.shields.io/badge/License-MIT-brightgreen.svg" alt="License MIT">
</p>
  

<p align="center">
  <a href="#about">About</a> •
  <a href="#installation">Installation</a> •
  <a href="#features">Features</a> •
  <a href="#support">Support</a> •
  <a href="#donate">Donate</a>
</p>

## About

> [!IMPORTANT]
> This is a separate fork. The original repository can be found here: https://github.com/WooshiiDev/HierarchyDecorator

Hierarchy Decorator is an extension for Unity 2018.4 and higher that extends Unity's hierarchy and takes it to the next level. With headers, component information and other features, it transforms the window into more than a plain list of objects. This can turn scene structures easier to read, understand and provide information on what is going on.

Everything is optional, and can be modified to the requirements of the project.

<p align="center">
<img width="372" alt="Unity_k2yhUSLugm" src="https://user-images.githubusercontent.com/31889435/226486583-8ad71e2b-1051-46b3-b00a-3880acffc413.png">
<img width="372" alt="Unity_myS52drEnl" src="https://user-images.githubusercontent.com/31889435/226486476-768a99ad-ae6f-4609-b8f8-8537c1f2393d.png">
</p>

## Installation

HierarchyDecorator can be installed directly through the git url
```
https://github.com/mgranddev/hierarchy-decorator.git?path=/package
```

You can also install this via git by adding the following to your **manifest.json**
```
"dev.mgrand.hierarchy-decorator" : "https://github.com/mgranddev/hierarchy-decorator.git?path=/package"
```

You can also install from the the GitHub Package Registry: https://github.com/mgranddev/hierarchy-decorator/pkgs/npm/dev.mgrand.hierarchy-decorator However, this is an advanced installation process.

For details on how to install a UPM package from the GitHub Package Registry, see this discussion: https://discussions.unity.com/t/using-github-packages-registry-with-unity-package-manager/784073 The relevant section starts at step #4.

## Features

| Feature                    | Hierarchy Decorator  | Other Hierarchy Extensions |
| -------------------------- | :----------------: | :-------------:   |
| Hierarchy Headers/Styles   |         ✔️         |        ✔️        |
| Tag/Layer Selector         |         ✔️         |        ✔️        |
| Breadcrumbs                |         ✔️         |        ✔️        |
| Component Icons            |         ✔️         |        ❌        |

For further details, including the original developer's planned features, please see the original repository: https://github.com/WooshiiDev/HierarchyDecorator

## Settings
  
<p align="center">
 <img align="center" width="929" alt="chrome_hzlst44Z1X" src="https://user-images.githubusercontent.com/31889435/226493547-3ec3db89-bcdf-4412-b000-c90aa9ee30b7.png">
</p>

There is a scriptable object that is required for hierarchy decorator to run. If it is deleted, another will be created in `Assets/HierarchyDecorator/`. These settings are also accessible from `Preferences`.

Setting design may change over time with development to support more features, or keep things looking consistent & clean.

### General
  
<details>
 <summary><b>Toggles</b></summary>
  
 <p align="center">
  <img width="915" alt="chrome_aClIcjH3wq" src="https://user-images.githubusercontent.com/31889435/226558578-78287342-711c-4b4b-acf3-18b316f3216b.gif">
  <img width="778" height="145" alt="Unity_GYpPOVFRrv" src="https://github.com/user-attachments/assets/fac34b54-684e-4499-b68b-a572d312bbd2" />
 </p>

  Toggles will simply display the state of the instance, can be clicked to toggle the instance active state.

  ```
  Show Active Toggles     Enable the toggles.
  Active Toggle Type      Choose between a checkbox or dot for the toggle icon.
  Active Swiping          Click and drag over check boxes to toggle them.
  Swipe Same State        Only toggle the instances with the same state as the first selected.
  Swipe Selection Only    If a selection exists, only toggle the selected instances.
  Depth Mode              The accepted criteria for selecting instances when swiping.
  ```
</details>

<details>
 <summary><b>Layers</b></summary>

<p align="center">
  <img width="913" alt="chrome_szO7gPHVZ4" src="https://user-images.githubusercontent.com/31889435/226493749-b30ebd4a-bf89-4841-bde8-b78159ec6068.png">
</p>
  
 Display the current layer the instance is assigned to.
  
  ```
  Show Layers             Enable the toggles.
  Click To Select Layer   Clicking the layer label will display a layer dropdown to update it.
  Apply Child Layers      Change the child gameobjects when updating the layer above.
  ```
</details>

<details>
 <summary><b>Breadcrumbs</b></summary>

<p align="center">
   <img width="922" alt="chrome_DtNbO5Mimi" src="https://user-images.githubusercontent.com/31889435/226493794-e45fbb59-ec38-430a-a3ba-2cd137251f46.png">
</p>
  
  Breadcrumbs will show line trails in the hierarchy, between objects to help visualise the tree. 
  
  _Instance_ settings are related to breadcrumbs drwan for the instance and it's siblings.<br>
 _Hierarchy_ settings will modify how breadcrumbs are displayed for higher depths.
  
  ```
  Show                    Show the breadcrumbs.
  Color                   The colour of the drawn lines.
  Style                   The line style - Solid, Dash, Dotted.
  Display Horizontal      Draw a horizontal line, from left to right, towards the instance.
  ```
</details>
 
### Visual

<details>
 <summary><b>Background</b></summary>
 
<p align="center">
 <img width="612" alt="chrome_Y3lak6Q0Dm" src="https://user-images.githubusercontent.com/31889435/226495114-e578f1c4-60d4-473e-8b42-b2c09c0fdeb1.png">
</p>

  The background can be enabled to alternate background colour between each hierarchy row. 

  ```
  Alternate Background    Show the breadcrumbs.
  Color One               The first colour for the theme.
  Color Two               The second colour for the theme.
  ```
</details>

<details>
 <summary><b>Styles</b></summary>
   
  The Style tab controls the design of the headers and seperators for the hierarchy. Colours are individual for light and dark mode providing accessibility. The **prefix** is the string to specify at the start of an instance name to apply the style.
  
  Layers and icons can be specifically disables on styles instances to remove clutter and information that is not required.

 <p align="center">
  <img width="510" height="450" alt="image" src="https://github.com/user-attachments/assets/1d727086-ea26-4ea9-ad66-26873b39d6b2" alt="Style Settings"/>
 </p>
</details>

  ### Icons

 Icons can be displayed that represent components that exist on gameobjects. This tab will provide the flexibility to specify what components can and cannot be displayed, and also allow you to automatically show all. 

<p align="center">
 <img width="132" height="327" alt="Unity_emGzaT8YHM" src="https://user-images.githubusercontent.com/31889435/226554415-8bd0be96-6eb2-4217-8d56-e39d23dd7ffd.png"><img width="627" alt="Unity_iWzNrNwYKa" src="https://user-images.githubusercontent.com/31889435/226494920-6b78be6e-686d-42ac-a11f-629f270cb5bc.png">
</p>

<details>
 <summary><b>Settings</b></summary>
 
 - Enable Icons: Will toggle the icons on.
 - Stack Mono Behaviours - If there are any MonoBehaviour derived components, show only one script icon on the instance.
 - Show Missing Script Warning - Show an indicator if there's an invalid script or "missing" script that cannot find the source file.

</details>

<details>
 <summary><b>Icon Panel</b></summary>
 
**Show All**

Below show all are two labels - Unity & Custom. Both of these can be enabled to automatically show the respective components automatically on all instances.
Unity components refer to built in types, while custom are custom MonoBehaviour's outside of Unity's code base.

**Groups**

Unity components have been categorized into related groups to make it easier to filter through all of them that exist. The search can be used to extend this further.

Any component toggled on in Excluded will disable them completely even if show all Unity components is enabled. This is primarily to make it easier to remove types not required when **Show All** is on.

**Custom**

Custom components are for scripts created in the project, that are not a part of Unity's engine. Here scripts can be grouped together and enabled if **Show All** for custom components is not on. 

Scripts can also be dragged in from the project view and will be added to the group highlighted for easy organisation.

<p align="center">
 <img width="40%" alt="Unity_emGzaT8YHM" src="https://user-images.githubusercontent.com/31889435/226555645-85954060-c25e-4ae8-bf5b-c7313d1188ee.gif">
 <img width="40%" alt="Unity_emGzaT8YHM" src="https://user-images.githubusercontent.com/31889435/226556916-73888fe0-b8fa-4365-88ab-18d786aa7c37.gif">
</p>

</details>

## Support

Functional changes to this fork will be minimal. Patches and new features will be merged from the original repository.

If you are encountering an issue, please verify whether the issue exists in the original repository: https://github.com/WooshiiDev/HierarchyDecorator

If the issue exists only in this fork, please create an issue here: https://github.com/mgranddev/hierarchy-decorator/issues

## Donate

This is a fork of HierarchyDecorator, originally created by Damian Slocombe ([@WooshiiDev](https://github.com/WooshiiDev)). If you find this tool useful, please consider supporting the original author: https://github.com/WooshiiDev/HierarchyDecorator/blob/master/README.md#support

Copyright (c) 2020-2025 Damian Slocombe
