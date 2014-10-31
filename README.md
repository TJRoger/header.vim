vim-autoHeader
==============

auto add header to your file when creating file with vim.
auto include the current directory as your project name
##result
```
//
//  test.c
//  project name
//
//  Created by Roger (ExampleEmail@gmail.com) on 10/29/14.
//  Copyright (c) 2014 ExampleWebsite.com. All rights reserved.
//
//  Description: 
//
```
##code
add the code to your `~/.vimrc`
```
"copyright add authomatically
"add or update the header
autocmd BufNewFile *.c exec ":call AddHeader()"
autocmd BufNewFile *.h exec ":call AddHeader()"
autocmd BufNewFile *.m exec ":call AddHeader()"
autocmd BufNewFile *.js exec ":call AddHeader()"
map <F4> :call AddHeader()<cr>'s
function AddHeader()
    call append(0, "//")
    call append(1, "//  ".expand("%:t"))
    call append(2, "//  ".fnamemodify(getcwd(), ':t'))
    call append(3, "//")
    call append(4, "//  Created by Roger (ExampleEmail@gmail.com) on ".strftime("%m/%d/%y").".")
    call append(5, "//  Copyright (c) ".strftime("%Y")." ExampleWebsite.com. All rights reserved.")
    call append(6, "//")
    call append(7, "//  Description: ")
    call append(8, "//")
    echohl WarningMsg | echo "Succeeded in adding copyright." | echohl None
endfunction
```
