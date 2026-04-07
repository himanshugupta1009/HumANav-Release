###Steps

Use Pyenv to get Python 3.6.9 for running this.
Install a virtual env and install packages from requirements.txt
Run `bash patches/apply_patches_3.sh` to apply a patch.

Ensure that the dataset has been downloaded. You need the Stanford 2D-3D-Semantics Dataset for this.

To unzip all the data files and to get the traversibles, follow the commands in sd3dis/README.md.

Once all of that is done, run this to generate the training data

`PYOPENGL_PLATFORM=egl PYTHONPATH=. .venv/bin/python examples/generate_vts_dataset_from_sampada.py`
