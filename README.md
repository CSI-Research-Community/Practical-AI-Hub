# Practical AI Hub

## Tips, Tricks and Hacks for your AI Research, and R&D Projects

<br>

## Literature Survey

### Experimentation with Code

- [Papers with code] is probably the best resource on the internet for finding the SOTA papers that have code available with them
- You might also want to check out the [associated github repositories]
- Arxiv also has a [code tab] where you can found the source code used in the experiments of the corresponding if the author has made it public
- This is the one I've used the least but might just help you so check out [catalyzeX]

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

- **Using GPU inside Docker:**
Check out [this tutorial on CUDA docker] or [this detailed blog] or if you're familiar with docker then go to the [Nvidia CUDA's dockerhub page.]

## Referencing

- ipynb notebooks in github: When learning AI/ML a lot of us use ipynb files to code and upload them on GitHub for future references. The problem is that GitHub's backend that renders these notebooks is horrible. Sometimes it takes 3-4 tries to load the notebooks, sometimes not even 25+ tries make it work and rarely it will work on the first try. There are two popular solutions to this -

    1. If the repo is public then do this -
        1. Open this link - <https://nbviewer.jupyter.org/>
        2. Paste your notebook's link there.
    2. If the repo is private then make a colab badge by -
        1. Add this in some readme -

                [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/[your username]/[repository name]/blob/master[or the branch it is on]/[name of your ipynb file])

        2. Fill in the appropriate places in the above code and save the readme file. Run the notebook on colab by clicking on the colab badge and authorize the notebook usage through GitHub

## Random Tips

- When working with multiple environments in the same system (python specific):
  - Make sure you have disabled the other environments to avoid package version clashes
  - If there are still clashes then try to use commands that specify the environment or directory
    - For example, for installing packages to the environment you are currently in and not affecting anything outside you can use something like
        ```sh
            python -m pip ...
        ```
    - Or when working with Anaconda or Virtual Env if you cannot import packages from that venv then you can try something like
        ```sh
            <path-to-venv>/bin/python [what you want to execute]
        ```

### Suspiciously Specific :thinking:

- If you are having problems installing something (especially Deep Learning tools and frameworks) then sometimes just trying the different methods for installation can work for some reason

- Always go for the .deb file and avoid .run files if you're using ubuntu

- It is always a good idea NOT to use the '-y' flag and instead check everything that will be modified during an installation

- Sometimes you just have to install all the dependencies manually (or write a script full of try-catches and if-elses) when you have conflicts with previous installations or other packages


[Papers with code]: https://paperswithcode.com/
[associated github repositories]: https://github.com/paperswithcode
[code tab]: https://blog.arxiv.org/2020/10/08/new-arxivlabs-feature-provides-instant-access-to-code/
[catalyzeX]: https://www.catalyzex.com/

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
