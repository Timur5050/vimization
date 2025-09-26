```
" -----------------------------
" Disable arrow keys completely
" -----------------------------
" Normal + Visual modes
noremap <Up> <NOP>
noremap <Down> <NOP>
noremap <Left> <NOP>
noremap <Right> <NOP>

" Insert mode
inoremap <Up> <NOP>
inoremap <Down> <NOP>
inoremap <Left> <NOP>
inoremap <Right> <NOP>

" -----------------------------
" Line numbers
" -----------------------------
set number              " Показувати абсолютні номери рядків
set relativenumber      " Відносна нумерація для зручних переходів

" -----------------------------
" Line number highlight
" -----------------------------
highlight LineNr ctermfg=NONE guifg=NONE
highlight CursorLineNr ctermfg=NONE guifg=NONE

" -----------------------------
" Syntax highlighting
" -----------------------------
syntax on

" -----------------------------
" Scrolling
" -----------------------------
set scrolloff=5         " Мін. відступ від краю при прокрутці

" -----------------------------
" Tabs & indentation
" -----------------------------
set expandtab           " Табуляція = пробіли
set tabstop=4           " Відображати таб як 4 пробіли
set shiftwidth=4        " Зсув >> і << = 4 пробіли
set softtabstop=4       " Tab у режимі Insert = 4 пробіли
set smarttab            " Розумний Tab з урахуванням shiftwidth
set smartindent         " Авто відступи після {, if тощо

" -----------------------------
" General settings
" -----------------------------
set backspace=indent,eol,start  " Backspace видаляє все що логічно
set nowrap                      " Не переносити довгі рядки
set ruler                       " Показувати позицію курсора (рядок:стовпець)
set mouse=a                     " Увімкнути мишку

" -----------------------------
" Search
" -----------------------------
set hlsearch            " Підсвічувати всі збіги
set incsearch           " Пошук під час введення
set ignorecase          " Ігнорувати регістр
set smartcase           " Але враховувати великі літери в запиті
nnoremap <Esc> :nohlsearch<CR>  " <Esc> двічі — зняти підсвітку пошуку
```