# PML Runner

Provides one click shortcuts to run PML macro files.

## Installation

To install this macro, as follows:

1. Put `pmlrun.pmlfrm` in a directory specified by the `PMLLIB` environment variable.

2. Open an AVEVA product.

3. Enter the following command in the **Command Window**:

   ```pml
   pml rehash all
   ```

## Usage

### Open macro

To open PML Runner form, enter the following command in the **Command Window**:

```pml
show !!pmlrun
```

### Initialization

When PML Runner form opens, PML Runner runs files `.init` in directories specified by the `PMLRUN` environment variable. If the environment variable is not defined, the directory is `%userprofile%\.pmlrun`.

### Form Controls

- File List

  This list shows the files and subfolders in directories specified by the `PMLRUN` environment variable. You can click a file with the extension `.mac` to run it.

- Args Textbox

  When PML Runner runs a macro file, it uses this box value as the arguments.

- All Checkbox

  If this box is selected, files and subfolders whose names begin with `.` appear in the list.
