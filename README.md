# gadgets-find

Find for the gadgets of [polpo](https://github.com/polpo-system/polpo): search a string in a set
of files and list the lines that contain it.

```
portia.Install gadgets-find
```

## Using

    Find.Domain {file} ~         the files to search
    Find.All ^                   search the selection in them, list the lines found
    Desktops.OpenDoc Find.Panel  the same with a panel

## What is here

    src/OLR.Find.Mod        Find
    share/Find.Panel        its panel
    tools/Find.Tool
    test/FindTest.Mod

The source comes from ETH Linux Oberon (OLR, 2017-06-18), converted from an Oberon text to plain
text; the first commit has it unchanged. It compiles unchanged with all five of polpo's compilers
(x86, ARM, ARMv7, RISC-V, MIPS).

## Tests

    FindTest.Run      2 checks: the module loaded, its panel opened; it needs the desktop's
                      display

The license is GPL-3 (`LICENSE`); the code comes from ETH Oberon, whose license (`LICENSE.ETH`)
asks to keep its copyright notice and conditions, which `LICENSE.ETH` does.
