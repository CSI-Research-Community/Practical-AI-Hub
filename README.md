# Practical AI Hub

## Tips, Tricks and Hacks for your AI Research, and R&D Projects

<br>

## Free/Cheap GPU Environments

- [Google Colab], or directly use the [tensorflow with GPU notebook]
- [Kaggle Kernels GPU]
- [Free and cheap GPUs at Gradient by Paperspace]
- [Very cheap RTX 2080Ti]
- [Another Cheap GPU Provider]
- [One free GPU workspace at FlyodHub]
- [GCP Jupyter Notebooks with $300 credits on sign-up]
- Also, check out the ones that are supported by [Nvidia natively]

## Environment Setup

### CUDA

- **Installing and using Multiple CUDA versions on one system:**
One of the roadblocks to trying out all the SOTA and other past works of a DL domain is the differences in their requirement of Nvidia's CUDA library. Most modern Deep Learning applications and code bases can require CUDA versions ranging from 8.0 to whatever the latest one is. Now, probably the best solution to this is using docker containers with specifically made base image (more on this below). But for people looking for another solution (I use this often when I want to quickly test out some code and sometimes even for big projects) [this blog might be what you are looking for.]

<br>

- **Using GPU inside Docker:**
Check out [this tutorial on CUDA docker] or [this detailed blog] or if you're familiar with docker then go to the [Nvidia CUDA's dockerhub page.]

[Google Colab]: https://colab.research.google.com/
[tensorflow with GPU notebook]: https://colab.research.google.com/notebooks/gpu.ipynb
[Kaggle Kernels GPU]: https://www.kaggle.com/dansbecker/running-kaggle-kernels-with-a-gpu
[Free and cheap GPUs at Gradient by Paperspace]: https://gradient.paperspace.com/
[Very cheap RTX 2080Ti]: https://puzl.ee/gpu-cloud
[Another Cheap GPU Provider]: https://www.genesiscloud.com/pricing
[One free GPU workspace at FlyodHub]: https://www.floydhub.com/pricing
[Nvidia natively]: https://www.nvidia.com/en-in/data-center/gpu-cloud-computing/
[GCP Jupyter Notebooks with $300 credits on sign-up]: https://cloud.google.com/ai-platform-notebooks

[this blog might be what you are looking for.]: https://medium.com/@peterjussi/multicuda-multiple-versions-of-cuda-on-one-machine-4b6ccda6faae
[this tutorial on CUDA docker]: https://www.celantur.com/blog/run-cuda-in-docker-on-linux/
[this detailed blog]: https://towardsdatascience.com/how-to-properly-use-the-gpu-within-a-docker-container-4c699c78c6d1
[Nvidia CUDA's dockerhub page.]: https://hub.docker.com/r/nvidia/cuda