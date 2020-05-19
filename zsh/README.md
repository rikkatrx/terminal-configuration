# mac

# linux

windows terminal + wsl(ubuntu)

## config windows terminal

### install

    > https://github.com/microsoft/terminal

### font

- download and install on windows

    > https://github.com/tonsky/FiraCode

- edit windows terminal profile in setting.json

    ``` json
    {
        "profiles":{
        "list":[
            {
                "guid":"...",
                "name":"...",
                "fontFace":"Fira Code Retina"
            }
        ]
    }
    }
    ```

    "Fira Code Retina" could be found in Windows Fonts Setting

### color schema

- download iterm2 color schema

    > https://github.com/mbadolato/iTerm2-Color-Schemes

- find schema json in ./windowsterminal**

    Dracula.json
    ``` json  
      {
            "name": "Dracula",
            "black": "#000000",
            "red": "#ff5555",
            "green": "#50fa7b",
            "yellow": "#f1fa8c",
            "blue": "#bd93f9",
            "purple": "#ff79c6",
            "cyan": "#8be9fd",
            "white": "#bbbbbb",
            "brightBlack": "#555555",
            "brightRed": "#ff5555",
            "brightGreen": "#50fa7b",
            "brightYellow": "#f1fa8c",
            "brightBlue": "#bd93f9",
            "brightPurple": "#ff79c6",
            "brightCyan": "#8be9fd",
            "brightWhite": "#ffffff",
            "background": "#1e1f29",
            "foreground": "#f8f8f2"
      }
    ```

- copy this json to setting.json

    ``` json
    {
        "schemes":[
            {
                "name":"Dracula",
                "black:"#000000",
                "....":"...."
            }        
        ]
    }
    ```

- active schema

    ``` json
    {
        "profiles":{
            "list":[
                {
                    "name":"....",
                    "fontFace":"....",
                    "colorSchema":"Dracula"
                }
            ]
        }
    }
    ```

## config wsl

### set dircolors

example: use dircolors.ansi-dark

> https://github.com/seebi/dircolors-solarized

- dowload

    > curl https://raw.githubusercontent.com/seebi/dircolors-solarized/master/dircolors.ansi-dark --output ~/.dircolors

- active

    copy this to .zshrc

    > eval `dircolors ~/.dircolors`


