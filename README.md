# README

This repositoary exists to build and release precompiled pytorch3d wheels for
platforms where precompiled pytorch3d packages are not available.

To test build PyTorch3D with the provided Pixi configuration locally, adapt the
following snippets (refer the the GitHub action script) as appropriate:

    git clone https://github.com/facebookresearch/pytorch3d.git -b v0.7.6
    cp pixi.lock pixi.toml pytorch3d
    cd pytorch3d
    pixi install --locked
    pixi run build-wheels
