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

When PML Runner form opens, PML Runner runs a file `.init` in the directory `%userprofile%\.pmlrun`. If it doesn't exist, it is automatically created. Additionally, you can change the directory by setting your desired path to the `PMLRUN` environment variable.

### Form

- File List

  This list shows the files and subfolders in the same directory as the `.init` file. You can click a file with the extension `.mac` to run it.

- Args Textbox

  When PML Runner runs a macro file, it uses this box value as the arguments.

- Show All Checkbox

  If this box is selected, files and subfolders whose names begin with `.` appear in the list.
