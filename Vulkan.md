This is a list of resources related to learning Vulkan that I've come across.  

### For those who know nothing:

[A Trip Through the Pipeline by 
Fabian Giesen](https://fgiesen.wordpress.com/2011/07/09/a-trip-through-the-graphics-pipeline-2011-index/)

[Render Hell 2.0 by Simon Trümpler](https://simonschreibt.de/gat/renderhell/)


*  *Queue* : A queue onto which you submit commands that the GPU reads and executes (asynchronously).
*  *Semaphore* : A GPU-GPU synchronization object.
*  *Fence* : A GPU-CPU synchronization object.
*  *Buffer& : Linear data for use on the device.
*  *Image* : Texture data (including dimensions & format) for use on the device.
*  *Sampler* : A collection of state required for a shader to sample textures (format, filtering etc).
*  *Pipeline* : A compiled collection of GPU state setting commands, shaders and other such data. (Almost) everything the GPU needs to get ready for rendering/compute work.
*  *PipelineCache* : A cache used by the pipeline compilation process. It is used to avoid unnecessary recompilations and can be saved and restored to and from disk to speed up subsequent compilations (for instance, in subsequent runs of the application).
*  *Swapchain* : A "ring buffer" of images offered by the platform's presentation engine (desktop compositors etc) on which the application can render and then submit for presentation.
*  *Pool* : A fast memory allocator specifically designed for objects of some specific type (descriptors, command buffers etc).

Source: https://www.reddit.com/r/vulkan/comments/4aveyh/tutorial_request_for_newbies_explain_the_things/d14551a
