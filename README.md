header.vim
==============

auto add header to your file when creating file with vim.
auto include the current directory as your project name

## Result
```
<?php
/***************************************************************************
 Copyright © 2020 rogerluo. All rights reserved.
 **************************************************************************/

/**
 * File: test.php
 * Author: rogerluo[tjrogertj@gmail.com]
 * Created At: 2020-04-29 22:42:39
 * desc:
 */
/* vim: set ts=4 sw=4 sts=4 tw=100 */

```
```
#!/bin/bash

###########################################################################
# Copyright © 2020 rogerluo. All rights reserved.
###########################################################################
# Author: rogerluo[tjrogertj@gmail.com]
# Created At: 2020-04-29 22:49:51
# File: test.sh
# desc:
# vim: set ts=4 sw=4 sts=4 tw=100

```

```
#!/usr/bin/env python3
# -*- coding: utf-8 -*-
###########################################################################
# Copyright © 2020 rogerluo. All rights reserved.
###########################################################################
# Author: rogerluo[tjrogertj@gmail.com]
# Created At: 2020-04-29 22:51:17
# File: test.py
# desc:
# vim: set ts=4 sw=4 sts=4 tw=100

```

## Installation

run command  
`$ curl -fsL -o ~/.vim/plugin/header.vim https://raw.githubusercontent.com/TJRoger/header.vim/master/header.vim`
