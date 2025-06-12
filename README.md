```bash
/** rofi -show drun -normal-window -config ~/.config/rofi/config.rasi
 * Rofi Configuration with Nordic Theme
 * For Arch Linux + i3wm
 */

configuration {
    modi: "drun,run,window";
    show-icons: true;
    icon-theme: "Nordic-Folder";
    display-drun: " ";
    display-run: "󰀄";
    display-window: "G";
    drun-display-format: "{name}";
    sidebar-mode: false;
    font: "Fira Code Nerd Font 12";
}

/* Nordic Color Palette */
* {
    /* Polar Night */
    nord0: #2E3440;
    nord1: #3B4252;
    nord2: #434C5E;
    nord3: #4C566A;
    
    /* Snow Storm */
    nord4: #D8DEE9;
    nord5: #E5E9F0;
    nord6: #ECEFF4;
    
    /* Frost */
    nord7: #8FBCBB;
    nord8: #88C0D0;
    nord9: #81A1C1;
    nord10: #5E81AC;
    
    /* Aurora */
    nord11: #BF616A;
    nord12: #D08770;
    nord13: #EBCB8B;
    nord14: #A3BE8C;
    nord15: #B48EAD;
    
    /* Application Colors */
    background: transparent;
    background-color: @nord0;
    foreground: @nord4;
    border-color: @nord8;
    selected-background: @nord8;
    selected-foreground: @nord0;
    active-background: @nord10;
    active-foreground: @nord4;
    urgent-background: @nord11;
    urgent-foreground: @nord6;
    
    /* Spacing */
    margin: 0;
    padding: 8px;
    spacing: 4px;
    border: 0px;
}

window {
    transparency: "real";
    background-color: @background-color;
    border-color: @border-color;
    border-radius: 1px;
    width: 40%;
    height: 800px;
    location: center;
    border: 2px;
}

inputbar {
    children: [prompt, entry];
    background-color: @nord1;
    border-radius: 4px;
    padding: 4px;
    border: 1px;
}

prompt {
    background-color: @nord8;
    padding: 4px 8px;
    border-radius: 1px;
    text-color: @nord0;
    margin: 0 4px 0 0;
    border: 1px;
}

entry {
    padding: 4px;
    text-color: @foreground;
    border: 1px;
}

listview {
    padding: 4px 0;
    dynamic: true;
    scrollbar: false;
    border: 0px;
}

element {
    padding: 4px;
    text-color: @foreground;
    border-radius: 1px;
    border: 0px;
}

element selected {
    background-color: @selected-background;
    text-color: #88C0D0;
    border-radius: 0px;
    border: 0;          /* Основна рамка */
    outline: 0;         /* Зовнішній контур */
    box-shadow: none;   /* Тіні */
    margin: 0;          /* Відступи */
}

element-text {
    text-color: inherit;
    border: 0px;
}

element-icon {
    size: 42px;
    padding: 0 8px 0 0;
    border: 0px;
}
```
