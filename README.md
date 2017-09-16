# Docker image for VASM

vasm is a portable and retargetable assembler to create linkable objects in
various formats or absolute code. Multiple CPU-, syntax and output-modules can
be selected.

Project homepage: http://sun.hasenbraten.de/vasm/

## Example usage

Assuming the current folder contain assembly sources:

```
docker run --rm -v $PWD:/data -w /data nguillaumin/vasm vasmm68k_mot -Ftos -devpac source.s
```

Make is also installed on the image:

```
docker run --rm -v $PWD:/data -w /data nguillaumin/vasm make
```
