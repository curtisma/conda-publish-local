# conda-publish-local
A GitHub Action to publish to a local Conda channel.  It copies the file to the channel and 
then indexes the channel.

## Inputs

- package_path: Path to the Conda package tarball (*.tar.bz2) file (required)
- channel_path: Path to the local Conda channel (required)
- channel_subdir: The Conda channel subdirectory in which to release the package.  
  Common options include linux-64 (default), linux-32, win-64, win-32, osx-64 (optional)
- build_env_prefix: Path to the root of a build Conda env containing conda and conda build.  Defaults to 
  "./envs/build" (optional)
