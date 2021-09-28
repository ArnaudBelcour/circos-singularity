# Circos singularity

A singularity recipe for Circos (inspired by the one written by [https://github.com/J35P312/CircusCircos](https://github.com/J35P312/CircusCircos)). This install all of its dependencies. The image size is around ~212 Mb.

You can directly call `circos` inside of the image like:

```
singularity exec -c -B /shared/folder:/shared/folder circos.sif circos -conf /shared/folder/circos.conf -outputdir /shared/folder
```

The `-c` option isolates the container and the `-B` option give access to a folder outside the container for Singularity.

You can use the path associated to `-B` to give access to data path in the configuration file.