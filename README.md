# stm32 template
Based on this guide: [https://stm32-base.org/guides/setup](https://stm32-base.org/guides/setup)

Directory structure of this project
```
─┬ stm32-template
 ├─ libraries
 ├─ projects
 └┬ tools
```

# GNU ARM Embedded Toolchain
Download the GNU ARM Embedded Toolchain and extract the archive to a directory, ie `~/dev/tool/iot/arm-gnu-embedded-toolchain`
This should result in this directory structure:
```
 ─┬ arm-gnu-embedded-toolchain
  ├┬ arm-none-eabi
  │└─ ...
  ├┬ bin
  │└─ ...
  ├┬ lib
  │└─ ...
  └┬ share
   └─ ...
```

# Test demo project
Open `Makefile` in `projects/stm32-f1-template` and change variable `TOOLCHAIN_PATH` to GNU ARM Embedded Toolchain folder
`TOOLCHAIN_PATH := ~/dev/tool/iot/arm-gnu-embedded-toolchain`

```
cd projects/stm32-f1-template
make
```
