# TDComfyUI
<a href="https://discord.com/invite/wNW8xkEjrf"><img src="https://discord.com/api/guilds/838923088997122100/widget.png?style=shield" alt="Discord Shield"/></a>

TouchDesigner interface for [ComfyUI](https://github.com/comfyanonymous/ComfyUI) API

![Screenshot_1](https://github.com/olegchomp/TDComfyUI/assets/11017531/fba8e8f2-42fb-486b-8cd4-839968f97601)

## Tutorial
* [How to connect everything to Stable Diffusion](https://youtu.be/62eARh_gRhE?si=gQmFEXY3P42woVya)
## Installation
1. Install [ComfyUI](https://github.com/ltdrdata/ComfyUI-Manager#installation)
2. Install [ComfyUI Nodes for External Tooling](https://github.com/Acly/comfyui-tooling-nodes)
3. Download latest [TDcomfyUI](https://github.com/olegchomp/TDComfyUI/releases) component
4. Add TDComfyUI.tox to TouchDesigner project.
5. Run "Re-init" in "Settings" page of TDComfyUI component.

## How to use:
1. Set "Enable Dev mode Options" in ComfyUI settings. 
2. Create workflow
3. Save workflow with "Save (API Format)"
5. Drop/Load created file in TouchDesigner project (TextDAT). Connect DAT to TDComfyUI input (InDAT)
6. Set parameters on Workflow page and run "Generate" on Settings page.

## Image send/recieve:
* **Send to ComfyUI** - "Load Image (Base64)" node should be used instead of default load image. In TouchDesigner set TOP operator in "ETN_LoadImageBase64 image" field on Workflow page.
* **Send to TouchDesigner** - "Send Image (WebSocket)" node should be used instead of preview, save image and etc. nodes.
  
Load [TouchDesigner_img2img.json](https://github.com/olegchomp/TDComfyUI/blob/main/TouchDesigner_img2img.json) in ComfyUI and TouchDesigner for Wokflow example.
