# Practical AI Hub

## Tips, Tricks and Hacks for your AI Research, and R&D Projects
<br><br>

## Environment Setup

### CUDA

- Installing and using Multiple CUDA versions on one system
<br>
One of the roadblocks to trying out all the SOTA and other past works of a DL domain is the differences in their requirement of Nvidia's CUDA library. Most modern Deep Learning applications and code bases can require CUDA versions ranging from 8.0 to whatever the latest one is. Now, probably the best solution to this is using docker containers with specifically made base image (more on this below). But for people looking for another solution (I use this often when I want to quickly test out some code and sometimes even for big projects) [this blog might be what you are looking for.]
- Using GPU inside Docker
Check out [this tutorial on CUDA docker] or [this detailed blog] or if you're familiar with docker then go to the [Nvidia CUDA's dockerhub page.]





[this blog might be what you are looking for.]: https://medium.com/@peterjussi/multicuda-multiple-versions-of-cuda-on-one-machine-4b6ccda6faae
[this tutorial on CUDA docker]: https://www.celantur.com/blog/run-cuda-in-docker-on-linux/
[this detailed blog]: https://towardsdatascience.com/how-to-properly-use-the-gpu-within-a-docker-container-4c699c78c6d1
[Nvidia CUDA's dockerhub page.]: https://hub.docker.com/r/nvidia/cuda