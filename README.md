# ComfyUI InstantMesh

**ComfyUI InstantMesh** is custom nodes that running [TencentARC/InstantMesh](https://github.com/TencentARC/InstantMesh) into ComfyUI

![overall](docs/overall.png)

## Installation

1. Install [ComfyUI-3D-Pack](https://github.com/MrForExample/ComfyUI-3D-Pack) using comfyui manager
2. Don't forget to run the post_install ;)
3. Install this custom node using comfyui manager
4. Restart ComfyUI.

# Changes in this fork

1. Standard directory paths (platform agnostic, no extra "ComfyUI" directory)
2. Standard save location (excluding all temp file locations)

## How to use

Currently, this extension implements two custom nodes, `InstantMeshLoader` and `InstantMeshRun`

Regarding `InstantMeshLoader`, there are four configurations for checkpoints, please refer to [TencentARC/InstantMesh](https://github.com/TencentARC/InstantMesh) for more details.

A simple workflow looks like:
![simple-connection](docs/overall.png) 
And you can find it at [simple-workflow](instantMesh-workflow.json)  
After generated, you could find results, mesh or texture, under `ComfyUI/custom_nodes/ComfyUI-InstantMesh/output` folder.

## Credit
- [TencentARC/InstantMesh](https://github.com/TencentARC/InstantMesh) - Efficient 3D Mesh Generation from a Single Image with Sparse-view Large Reconstruction Models
- [ComfyUI](https://github.com/comfyanonymous/ComfyUI) - A powerful and modular stable diffusion GUI.
- [ComfyUI-3D-Pack](https://github.com/MrForExample/ComfyUI-3D-Pack) - An extensive node suite that enables ComfyUI to process 3D inputs (Mesh & UV Texture, etc) using cutting edge algorithms (3DGS, NeRF, etc.)

## My extensions for ComfyUI
- [ComfyUI-Workflow-Encrypt](https://github.com/jtydhr88/ComfyUI-Workflow-Encrypt) - Encrypt your comfyui workflow with key

## My extensions for stable diffusion webui
- [3D Model/pose loader](https://github.com/jtydhr88/sd-3dmodel-loader) A custom extension for AUTOMATIC1111/stable-diffusion-webui that allows you to load your local 3D model/animation inside webui, or edit pose as well, then send screenshot to txt2img or img2img as your ControlNet's reference image.
- [Canvas Editor](https://github.com/jtydhr88/sd-canvas-editor) A custom extension for AUTOMATIC1111/stable-diffusion-webui that integrated a full capability canvas editor which you can use layer, text, image, elements and so on, then send to ControlNet, basing on Polotno.
- [StableStudio Adapter](https://github.com/jtydhr88/sd-webui-StableStudio) A custom extension for AUTOMATIC1111/stable-diffusion-webui to extend rest APIs to do some local operations, using in StableStudio.
- [Txt/Img to 3D Model](https://github.com/jtydhr88/sd-webui-txt-img-to-3d-model) A custom extension for sd-webui that allow you to generate 3D model from txt or image, basing on OpenAI Shap-E.
- [3D Editor](https://github.com/jtydhr88/sd-webui-3d-editor) A custom extension for sd-webui that with 3D modeling features (add/edit basic elements, load your custom model, modify scene and so on), then send screenshot to txt2img or img2img as your ControlNet's reference image, basing on ThreeJS editor.
