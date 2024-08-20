# rvirt-gpu

Virtualization for `GPU` that allows you to run local `GPU` apps and the code is actually ran in the cloud.

Functionality:
- `vGPU` is a `virtualization` layer for a `GPU`
- your local app "runs" on local `vGPU`
- local app decrypts the actual local data and sends the (`CUDA`) instructions to the remote `GPU-Coortinator`
- `GPU-Coortinator` distribute the instructions to multiple real `GPU`s
- then it sends the results back to `vGPU` which sends them to the local app

**The advantage is your private data never leave your network in plain. Only data needed to run actual CUDA instructions are sent over the wire but also encrypted with TLS.**

# Wiki

[Wiki](https://github.com/radumarias/rgpu/wiki)

# Schema

[![schema](website/resources/schema2.png)](website/resources/schema2.png)
