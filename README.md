# Assembly Language Processing System

## Project Overview
This project is a complete system for processing, assembling, and linking assembly language programs. It efficiently handles symbol table generation, opcode translation, address assignment, and loader functionalities. The system is designed for structured input and output handling, ensuring smooth execution of assembly programs.

## Features
- **Assembly language processing:** Parses and processes assembly language instructions.
- **Symbol table generation:** Automatically assigns addresses to symbols and mnemonics.
- **Opcode translation:** Converts assembly instructions into machine-readable opcodes.
- **Loader functionality:** Generates a loader file for execution.
- **Structured file handling:** Organizes input, intermediate, and output files systematically.

---

## Project Structure

The following is the correct directory structure of the project:

```bash
.
├── .vscode/
│   ├── c_cpp_properties.json   # VSCode IntelliSense and compilation settings
│   ├── launch.json             # Debugging configurations
│   ├── settings.json           # User-defined settings for VSCode
│
├── addressed_file.txt          # Processed assembly instructions with addresses
├── intermediate.txt            # Intermediate processing data
├── loader.txt                  # Loader instructions for execution
├── main.c                      # Core source code for the assembler
├── new_input.txt               # Raw assembly input file
├── object_file.txt             # Final object file containing machine code
│
├── output/
│   ├── main.exe                # Final executable output
│   ├── intermediate.txt        # Intermediate processing data
│   ├── loader.txt              # Loader instructions for execution
│   ├── object_file.txt         # Object file containing machine code
│   ├── symtab.txt              # Symbol table reference
│
├── symtab.txt                  # Symbol table mapping labels to addresses
```

---

## How to Use

### **1. Compile the Program**
Use GCC to compile the assembler source code:
```sh
gcc main.c -o assembler
```

### **2. Run the Program**
Execute the assembler with an input file:
```sh
./assembler new_input.txt
```

### **3. Generated Output Files**
- `addressed_file.txt`: Processed assembly instructions with assigned addresses.
- `symtab.txt`: Symbol table containing memory addresses of symbols.
- `intermediate.txt`: Stores intermediate processing results.
- `object_file.txt`: Final object file containing machine code.
- `loader.txt`: Loader file for execution.
- `output/main.exe`: Final executable file.

---

## Requirements
- **GCC Compiler** (for compiling `main.c`)
- **Basic understanding of assembly language**

---

## Future Enhancements
- **Error Handling:** Improve validation for invalid mnemonics and syntax errors.
- **Performance Optimization:** Optimize memory allocation and symbol table lookup.
- **Extended Opcode Support:** Expand opcode set for additional assembly instructions.

---

## Contributors
- **Mahmoud Hany** - Lead Developer

For contributions and issues, please contact [Mahmoud Hany]((https://www.linkedin.com/in/mahmoud-hany-fathalla-6b1690219/)).

---

## License
This project is licensed under the MIT License.

