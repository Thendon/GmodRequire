
  Require

  How to use:
  - use: Require( <i>pathToFile</i> )
  - example: Require( "classes/core/printer")
  - note: 
      - do NOT add any prefixes like cl_, sv_, sh_ or the .lua file ending
      - 
      - Scince all files are included only one time it is recommended to save the return into alocal variable

  What it does:
  -   all found files get combined and included ONCE and table pointer is saved for following requires
  -   if the file was required before, the same pointer gets returned
  -   combined means sh_printer.lua & sv_printer.lua (in the example) will be returned (serverside) and sh_printer.lua & cl_printer.lua (clientside) as single table
  -   scans in lua and gamemode folder by default
  -   no prefix is handled like sh_

  How it works:
  -   meta-table magic
  
  Why I do this:
  -   worked a lot with javascript recently
