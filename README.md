# composite-shell-os

This repository gives an example of how a composite Action can run a script using `bash` or `pwsh` depending on the OS in use by the runner.

```pseudo
if: runner os = mac or linux
  shell = bash
else
  shell = pwsh
```

The simple logic above is used due to the fact that GitHub hosted runners are available in 3 operating system flavours:

MacOS and Linux both use `bash` and Windows uses `pwsh`: https://github.com/MosJef-Workflow-Examples/ShellDetection
