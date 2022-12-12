To get started using [Codespaces](https://github.com/features/codespaces),
you flip a toggle:


```nix title="devenv.nix"
{ pkgs, ... }:

{
    devcontainer.enable = true;
}
```

Once you run ``devenv shell``, you should see an auto-generated `.devcontainer.json` file.


If you commit that file to the Git repository and push it, you're good to go.
