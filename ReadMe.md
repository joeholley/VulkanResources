This is a list of resources related to learning Vulkan that I've come across.  

### For those who know nothing:

This links in this section help you understand the GPU in detail

[A Trip Through the Pipeline by Fabian Giesen ](https://fgiesen.wordpress.com/2011/07/09/a-trip-through-the-graphics-pipeline-2011-index/)

[Render Hell 2.0 by Simon Trümpler](https://simonschreibt.de/gat/renderhell/)

[Vulkan in 30 minutes](https://renderdoc.org/vulkan-in-30-minutes.html)

#### Definitions (from Above)
*  **Queue** : A queue onto which you submit commands that the GPU reads and executes (asynchronously).
*  **Semaphore** : A GPU-GPU synchronization object.
*  **Fence** : A GPU-CPU synchronization object.
*  **Buffer** : Linear data for use on the device.
*  **Image** : Texture data (including dimensions & format) for use on the device.
*  **Sampler** : A collection of state required for a shader to sample textures (format, filtering etc).
*  **Pipeline** : A compiled collection of GPU state setting commands, shaders and other such data. (Almost) everything the GPU needs to get ready for rendering/compute work.
*  **PipelineCache** : A cache used by the pipeline compilation process. It is used to avoid unnecessary recompilations and can be saved and restored to and from disk to speed up subsequent compilations (for instance, in subsequent runs of the application).
*  **Swapchain** : A "ring buffer" of images offered by the platform's presentation engine (desktop compositors etc) on which the application can render and then submit for presentation.
*  **Pool** : A fast memory allocator specifically designed for objects of some specific type (descriptors, command buffers etc).

Source: https://www.reddit.com/r/vulkan/comments/4aveyh/tutorial_request_for_newbies_explain_the_things/d14551a

### Vulkan API - Companion Guide by Harry Gould 
* [Book](https://www.gitbook.com/book/harrylovescode/vulkan-api/details)
* [GitHub](https://github.com/HarryLovesCode/Vulkan-API-Book)

### API Without Secrets: Introduction to Vulkan by Pawel Lapinski [Github](https://github.com/GameTechDev/IntroductionToVulkan)
* [Part 0](https://software.intel.com/en-us/articles/api-without-secrets-introduction-to-vulkan-preface)
* [Part 1](https://software.intel.com/en-us/api-without-secrets-introduction-to-vulkan-part-1)
* [Part 2](https://software.intel.com/en-us/api-without-secrets-introduction-to-vulkan-part-2)
* [Part 3](https://software.intel.com/en-us/api-without-secrets-introduction-to-vulkan-part-3)

### A Brief Overview of Vulkan API

https://www.toptal.com/api-developers/a-brief-overview-of-vulkan-api

### Vulkan API Overview by [ Henri Tuhola.](http://boxbase.org/entries/2014/jul/28/about-the-author/)

* [Clear the Screen](http://boxbase.org/entries/2016/feb/22/vulkan-api-overview/)
* [Draw Primitives](http://boxbase.org/entries/2016/feb/29/vulkan-api-overview-2/)
* [Pipeline Barriers](http://boxbase.org/entries/2016/mar/7/vulkan-api-overview-3/)

### Vulkan API Tutorial Video series by Niko Kauppi - Visual Studio/C++ [Github Repository](https://github.com/Niko40/Vulkan-API-Tutorials)
* [Play List](https://www.youtube.com/watch?v=wHt5wcxIPcE&list=PLUXvZMiAqNbK8jd7s52BIDtCbZnKNGp0P)
* [Getting started with vulkan code](https://www.youtube.com/watch?v=wHt5wcxIPcE)
* [New Project, Instance and Device](https://www.youtube.com/watch?v=YhQZYnpFX_0)
* [Debugging & Layers](https://www.youtube.com/watch?v=raXIWyWBv2I)
* [Recap and SDK](https://www.youtube.com/watch?v=OeERUoJaw9o)
* [Command Buffers and Syncrhonization](https://www.youtube.com/watch?v=Bu581jeyTL0)
* [Window](https://www.youtube.com/watch?v=J87M6HdcjS0)
* [Window Surface](https://www.youtube.com/watch?v=36Zj8fa3iyg)

### GDC 2016 Presentation Video

* [Vulkan Part 1](https://www.youtube.com/watch?v=HM8vYJQtHpA)
  * [Vulkan Design Philosiphy - Jeff Bolz - Nivida](https://youtu.be/HM8vYJQtHpA?t=15m2s)
  * [Memory Allocation - Grahm Sellers - AMD](https://youtu.be/HM8vYJQtHpA?t=35m51s)
  * [Command Buffers & Render Pass/Subpass - Bill Licea-Kane - Qualcomm](https://youtu.be/HM8vYJQtHpA?t=1h1m13s)
  * [Keeping your GPU fed - Tobias Hector - Imagination](https://youtu.be/HM8vYJQtHpA?t=1h29m14s)
* [Vulkan Part 2](https://www.youtube.com/watch?v=xXyZ4YaktyU)
  * [Vulkan WSI/Swapchains - Alon Or-bach - Samsung](https://youtu.be/EX1RKhlOYmY?t=10s) 
  * [LunarG SDK - Karan Ghavam - LunarG](https://youtu.be/EX1RKhlOYmY?t=17m53s)
  * [A Next Gen Engine Design - Dan Baker - Oxide Games](https://youtu.be/EX1RKhlOYmY?t=42m27s)
  * [Performance Lessons Porting Source 2 Engine to Vulkan - Dan Ginsberg - Valve](https://youtu.be/EX1RKhlOYmY?t=1h14m31s)
  * [Vulan does Retro - libRetro - Hans-Kristian Arntzen](https://youtu.be/EX1RKhlOYmY?t=1h41m13s)
  * [Porting Cinder to Vulkan- Hai Nguyen - Google - Art Copy and Code Project](https://youtu.be/EX1RKhlOYmY?t=1h49m54s)
  * [GFXBench 5- Gergely Juhasz - Kishonti](https://youtu.be/EX1RKhlOYmY?t=2h3m3s)
  * [Comparing Vulkan to OpenGL ES - Barthold Lichtenbelt - NVIDIA](https://youtu.be/EX1RKhlOYmY?t=2h9m20s)

### Articles
* [Using the Vulkan™ Validation Layers by Daniel Rakos ](http://gpuopen.com/using-the-vulkan-validation-layers/)

### Siggraph 2015 - An Overview of Next-Generation Graphics API

This is mainly filled with Powerpoint presentations :(.

http://nextgenapis.realtimerendering.com/

### Sample Code

* [C++ Examples ](https://github.com/SaschaWillems/Vulkan) by Sascha Willems
* [C++ Examples](https://github.com/LunarG/VulkanSamples) from LunarG
* [C++ Examples](https://github.com/Z80Fan/VulkanDemos) by Z80Fan
* NVidia Examples
  * ["Simple" Example](https://github.com/nvpro-samples/gl_vk_chopper)
  * [Rendering 3D With 'worker-threads'](https://github.com/nvpro-samples/gl_vk_bk3dthreaded)
  * [Vulkan sample showing a high quality super-sampled rendering](https://github.com/nvpro-samples/gl_vk_supersampled)
  * [Vulkan & OpenGL Threaded CAD Scene Sample ](https://developer.nvidia.com/vulkan-opengl-threaded-cad-scene-sample) (Blog Post)
* [Spinning Vulkan Cube in C](https://github.com/krh/vkcube) by Kristian Høgsberg
* [Vulkan-sxs](https://github.com/philiptaylor/vulkan-sxs)
* [Google Android Samples](https://github.com/googlesamples/android-vulkan-tutorials)
* [Google Samples](https://github.com/googlesamples/vulkan-basic-samples)  Currently just LunarG samples
* [VKTS Samples (C++)](https://github.com/McNopper/Vulkan) Vulkan examples using VulKan ToolS (VKTS)
* [The Stardust sample application](https://github.com/GameTechDev/stardust_vulkan)  The Stardust sample application uses the Vulkan graphics API to efficiently render a cloud of animated particles. 
* [C SDL2 Window](https://github.com/corngood/SDL_vulkan)
* [Android PowerVR](https://imgtec.com/tools/powervr-early-access-program/) - requires registration.
* [Vulkan Code to Clear the Screen](https://gist.github.com/Overv/7a9200b0ab666004efcbde451433b039)

### Language Bindings
* [C++](https://github.com/nvpro-pipeline/vkcpp)
* C#/F#/Visual Basic
  * [SharpVulkan](https://github.com/jwollen/SharpVulkan)
  * [Mono](https://github.com/mono/VulkanSharp)
* [Haskell](https://github.com/expipiplus1/vulkan)
* [D](https://github.com/ColonelThirtyTwo/dvulkan)
* [Common Lisp](https://github.com/3b/cl-vulkan)
* [Julia](https://github.com/JuliaGPU/Vulkan.jl)
* [Rust](https://github.com/tomaka/vulkano)
* [Go](https://github.com/vulkan-go/vulkan)
* [C++ GPGPU lib](https://github.com/alexhultman/libvc)

### More Resources
* [Vulkan Quickreference (PDF)](https://www.khronos.org/registry/vulkan/specs/1.0/refguide/Vulkan-1.0-web.pdf)
* [Vulkan Specification](https://www.khronos.org/registry/vulkan/specs/1.0-wsi_extensions/xhtml/vkspec.html)
* [Khronous.org Resources](https://github.com/KhronosGroup/Khronosdotorg/blob/master/api/vulkan/resources.md)
* [Vulkan on Stackoverflow](http://stackoverflow.com/questions/tagged/vulkan)
* [Vulkan on reddit](https://www.reddit.com/r/vulkan/)
* [Awsome Vulkan](https://github.com/vinjn/awesome-vulkan) (Lots of Links)

### Companies support Vulkan
* [NVidia](https://developer.nvidia.com/Vulkan)
* [AMD](http://www.amd.com/en-us/innovations/software-technologies/technologies-gaming/vulkan#)
* [Intel](https://software.intel.com/en-us/videos/vulkan-on-intel-graphics-at-gdc-2016)
* [Imagination/PowerVR](http://blog.imgtec.com/?s=Vulkan&submit=Search)

