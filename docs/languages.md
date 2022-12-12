What if you could have the tooling for any programming language by flipping a toggle?

```nix title="devenv.nix"
{ pkgs, ... }:

{
  languages.python.enable = true;
  languages.typescript.enable = true;
}
```

``devenv`` will provide executables for both languages:

```shell-session
$ devenv shell
Building shell ...
Entering shell ...

Python 3.10.8
tsc --version
Version 4.8.4
(devenv) $ 
```

See the [supported-languages](https://github.com/cachix/devenv/blob/main/examples/supported-languages/devenv.nix) example for a list of currently supported languages.

!!! note 

    The latest versions of the tooling are currently provided.
    [In the future, package sets and pinning will be supported
    and documented](https://github.com/cachix/devenv/issues/16).
