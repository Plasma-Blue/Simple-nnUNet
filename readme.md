# Simple-nnUNet

## Why Simple-nnUNet?
nnUNet has demonstrated exceptional performance across various segmentation tasks in real-world production. However, its codebase can be somewhat disorganized, which is why we need Simple-nnUNet. Is it really that simple? Yes.

## Refactoring Goals

### 1. Segmentation Performance First
This means retaining the critical training and inference processes of nnUNet while ensuring minimal performance differences after reimplementation.

### 2. Simplicity and Elegance
I have previously extracted and refactored the inference process of nnUNet, providing a simple and elegant interface. The goal is to achieve the same standard for the entire nnUNet codebase.

### 3. Speed
Inference should be as fast as possible. I have experience accelerating nnUNet's inference (up to 10 times faster than the original), so this won't be a major issue. Optimizing inference time can also slightly benefit the training process. For example, optimizing the previously inefficient resampling in nnUNet will improve efficiency for both inference and training.

### 4. Easy to Extend and Modify
The training framework should allow:

- Easy adjustment of training parameters
- Flexible modification of network structures
- Relatively easy customization of training workflows
- Relatively easy customization of inference workflows
- Clean component reuse with decoupled inference and training processes
- Easy reproducibility
- Visualization of training states
- Support for checkpoint mechanisms
- Easy fine-tuning
- Compatibility with 2D and 3D images and networks

Due to the balance between simplicity and functionality, not all features may be implemented or retained. Balancing is always challenging!

### 5. Educational Purpose
By examining simple, clear, and elegant code, interested individuals can understand the ultimate solutions in deep learning segmentation.

### 6. Consistent Usage
nnUNet requires only three command lines to start training. We aim to maintain consistent usage—unless we can make it even simpler!

## Is It Useful?
Yes. For learning, showcasing skills, having fun, preparing for future ventures, and as a gift to the world.

## Project Timeline
nnUNet has been maintained from v1 to v2 over five to six years. This is a long-term project, but we hope to achieve most goals within a year. Optimistically, it could be faster.

## Open Source?
Yes. Although I dislike how big tech companies exploit open-source projects without giving back to the community, great projects like FreeSurfer and nnUNet are open source. Respect. The project will use the AGPL V3 license to restrict unethical profit-making by such organizations in the future.
