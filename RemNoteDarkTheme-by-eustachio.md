- # RemNote Dark Theme by eustachio 
- Created by eustachio
- The dark theme and light theme will be merged soon.
- This is something I do for fun as I like simple and modern UI's. I wanted to make RemNote look awesome!!!
- Version 2.0 - Worrks with RemNote new app v1.4.
- Release date: 07 November 2021
- Please consider donate, it will help me to keep myself motivated to maintain the theme, fix bugs and introduce new ideas. I will appreciate it.
- [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=22TRCSWF3MZM6)

```markdown
- [ ] **RemNote Dark Theme by eustachio v1.3**
  - Designed, created and maintained by Eustachio (I do not work for RemNote)
  - Please consider donate, it will help me to keep myself motivated to maintain the theme, fix bugs and introduce new ideas. I will appreciate it.
  - This theme has been created to work with the `Dark Mode ON`
  - This is something I do for fun as I like simple and modern UI's. I wanted to make RemNote look awesome!!!
  - Version 2.0 - Released date: 07 November 2021
    - Updated to work with new RemNote App v.1.4
    - Redesigned portals
    - New darker theme option
    - Light theme (coming soon)
    - PDF and Image occlusion (coming soon)
    - Mobile version (coming soon)
    - Branches work but they are not perfect yet.
    - Css files are now hosted on Github, so it will be easier for future updates.
  - Version 1.3 - Released date: 25 August 2021
    - Branches have been fixed
    - Showing the hamburger (the 3 dots) this makes the 3 dots visible when in multiple windows, default and full width modes and when windows pane lab feature is ON and OFF.
    - Windowed pane has been retouched
    - The theme now works on mobile apps (BETA)
    - Quote spacing has been fixed 🤞
    - The todo tag has been removed from the markdown file that creates the theme to avoid some theme blocks to appear on your todo list (sorry about that)
  - Version 1.2 - Released date: 28 June 2021
    - Optional dark (inverted) PDF
    - Optional dark (inverted) Image Occlusion
    - Fixed some right-click menus and 'Quick Add' white backgrounds
  - Version 1.11 - Released date: 11 June 2021
    - More visible scrollbars
    - No Quote text jumps
    - Help menu hover now matches the dark theme
    - Highlight text color margin/padding improvements
    - Show proper card types on bottom bar
    - No white background on bottom bar
    - No white top border on narrowed bottom bar
    - New Windowed panes code block - Thanks to Henrik. This fixes the white body background when this lab feature Windowed Panes is ON.
    - Fixed dark background on popups windows
    - Fixed Latex dark background
  - Tested on MacOS (Big Sur) and Linux.
  - https://github.com/eustachi0/RemNoteThemes/blob/main/RemNoteDarkTheme-by-eustachio.md
  - For bugs and suggestions, please drop me an email to: `eustachio.dipaola@gmail.com` with some screenshots if possible.
  - For future updates, I recommend that you create a CSS code block at the bottom after this theme for your custom lines of code, things that you would like your way. So when an update, you can delete this theme and paste the new updated version without losing your customizations.
  - [ ] **0 Variable**
    - [ ] Dark Theme
      - [ ] Dark Theme - Original
        ```css
        @import url("https://eustachi0.github.io/RemNoteThemes/CSS/00_Dark-Theme_Original.css");
        ```
      - [x] Dark Theme - Darker
        ```css
        @import url("https://eustachi0.github.io/RemNoteThemes/CSS/00_Dark-Theme_Darker.css");
        ```
    - [ ] Light Theme
      ```css
      @import url("https://eustachi0.github.io/RemNoteThemes/CSS/00_Light-Theme_Original.css");
      ```
    - [ ] General Customizations
      ```css
      :root {
      /*body*/
          --font-name: "my font";
          --rem-margin-left: -16px;
          --rem-padding-left: 16px;

          --focused-bullet-border-color: rgb(193, 177, 255, 0.3);
          --collapse-bullet-border-color: rgb(177, 209, 255, 0.3);
          --collapse-bullet-icon-border-color: rgb(185, 209, 255, 0.1);
          --link-text-color: var(--accent-color);
          --pdf-highlight-text-color: var(--accent-color);
          --focused-link-text-color: var(--focused-accent-color);
          --cloze-cards-lines: var(--accent-color);
          --focused-cloze-cards-lines: var(--focused-accent-color);
          --quote-background: transparent;
          --focused-quote-background: transparent;
          --todo-finished-text-color: var(--accent-color);
          --latex-text-color: var(--accent-color);
          --focused-latex-text-color: var(--focused-accent-color);
          --breadcrumbs-text-color: var(--accent-color);
          --search-box-background-color: rgb(28, 30, 30);
          --search-box-text-color: var(--body-text-color);
      /*sidebar*/
          --sidebar-top-background-color: rgb(30, 32, 32);
          --sidebar-text-color: #BFBFBF;
          --sidebar-hover-background-color: rgb(39, 41, 41);
          --sidebar-hover-text-color: #D8D8D8;
          --nodocuments-text-color: rgb(88, 90, 90);
          --queue-indicator-icon-color: orange;
          --sidebar-focused-background-color: rgb(48, 50, 50);
          --sidebar-focused-left-border-color: rgb(48, 50, 50);
          --sidebar-focused-left-border-width: 0px;
          --sidebar-focused-text-color: white;
          --bars-border-width: 1px;
          --bars-border-radius: 7px;
      /* icons */
          --icons-color: #797E7F; /*#6F7E95*/
          --icons-filter: invert(51%) sepia(6%) saturate(227%) hue-rotate(142deg) brightness(95%) contrast(83%);
      /* modified 05 Jun 2021*/
          --popup-selected-background-color: rgb(56, 58, 58); /*added 04 Jun 2021*/
          --popup-hover-text-color: var(--body-text-color);
          --popup-border-radius: 6px;
          --popup-border-color: rgb(50, 52, 52);
          --popup-border-width: 1px;
          --popup-keycode-color: var(--accent-color);
      /* queue */
          --queue-fill-in-the-blank-color: #6060CA;/*modified 04 Jun 2021*/
      /* toggle checkbox*/   
          --toggle-background-color: rgb(28, 30, 30);/*mod 08 Jun 2021*/
          --toggle-color: #CECECE;
      /* knowledge base page*/
          --knowledgebasepage-background-color: rgb(40, 42, 42);
          --knowledgebasepage-title-background-color: rgb(48, 50, 50);
      /*portals*/
          --portal-text-color: #C4C4C4;
          --embeddedsearch-background-color: rgb(35, 38, 38);
          --portal-inside-portal-border-color: rgb(52, 54, 54);
          --portal-inside-portal-left-margin: 11px;
          --searchkeywordhighlight-color: #8E9664;
          --searchkeywordhighlight-text-color: white;
      /*borders radius*/
          --portal-border-radius: 16px; /* up to 15px*/
          --portal-inverted-radius: 12px; /* up to 15px*/
          --border-radius: 10px;
      /* code block */
          --code-block-text-color: #B6B6B6;
          --code-block-background-color: rgb(28, 30, 30);
          --code-block-focused-background-color: rgb(22, 24, 24);
          --code-block-border-color: #49525B;
          --code-block-border-width: 2px;
      /* settings buttons color */
          --button-color: #435371;
          --highlightcolor-border-radius: 20px;
          --highlightcolor-tags-border-radius: 10px;
      }
        ```
    - [x] Bright highlight colors
      ```css
      /*Bright highlight colors*/
      :root {
          /*red*/
          --highlight-red: rgb(203, 29, 73, 80%);
          --highlight-red-focused: rgb(218, 30, 77, 90%);
          /*orange*/
          --highlight-orange: rgb(202, 125, 27, 80%);
          --highlight-orange-focused: rgb(202, 125, 27, 90%);
          /*yellow*/
          --highlight-yellow: rgb(214, 193, 21, 80%);
          --highlight-yellow-focused: rgb(214, 193, 21, 90%);
          /*green*/
          --highlight-green: rgb(31, 193, 23, 80%);
          --highlight-green-focused: rgb(31, 193, 23, 90%);
          /*blue*/
          --highlight-blue: rgb(47, 126, 245, 80%);
          --highlight-blue-focused: rgb(25, 97, 201, 90%);
          /*purple*/
          --highlight-purple: rgb(165, 85, 239, 80%);
          --highlight-purple-focused: rgb(106, 26, 196, 90%);
      }
      ```
    - [ ] Light highlight colors
      ```css
      /* Light highlight colors */
      :root {
          /*red*/
          --highlight-red: #8F454C;
          --highlight-red-focused: #8E3842;
          /*orange*/
          --highlight-orange: #8F6949;
          --highlight-orange-focused: #8E6340;
          /*yellow*/
          --highlight-yellow: #928A56;
          --highlight-yellow-focused: #928642;
          /*green*/
          --highlight-green: #4E884E;
          --highlight-green-focused: #3B883C;
          /*blue*/
          --highlight-blue: #486691;
          --highlight-blue-focused: #3B5D90;
          /*purple*/
          --highlight-purple: #674989;
          --highlight-purple-focused: #613E87;
      }
      ```
    - [x] TreeNode Purple/Magenta
      - [ ] Lines
        ```css
        /* TreeNode Lines Purple/Magenta */
        :root {
        /* bullet color */
            --bullet-color: #797E7F;
            --hover-bullet-color: #8C3E83;
            --focused-bullet-color: #880579;
        /*Tree Lines*/
            --tree-lines-color: #60365B;
            --hover-tree-lines-color: var(--hover-bullet-color);
            --focused-tree-lines-color: var(--focused-bullet-color);
            --tree-focused-bullet-color: var(--focused-bullet-color);
            --tree-hover-focused-bullet-color: #882F7D;
        /*if Alternating lines indent color ON */    
            --alt-tree-lines-color: #553F5E;
            --alt-hover-tree-lines-color: #815892;
            --alt-focused-tree-lines-color: #8832AC;
            --alt-tree-focused-bullet-color: #8832AC;
            --alt-tree-hover-focused-bullet-color: #7D4793;
            --alt-tree-hover-bullet-color: #815892;
        }
        ```
      - [ ] Branch symbol
        ```css
        /* TreeNode branch symbols Purple/Magenta */
        :root {
            /* svg main lines */
            --focused-branch-tree-symbol: url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='400' height='400' viewBox='0 0 105.83333 105.83334'%3E%3Cpath d='M4.8645178 36.435266H44.988572m18.053281 7.477892a25.531159 25.531159 0 00-18.053281-7.477892m44.274625 23.124007h11.653483m-29.706763-7.477892a25.531159 25.531159 0 0018.05328 7.477892m-18.05328-7.477892l-8.168064-8.168223' stroke-width='9.08617' stroke-linecap='round' fill='none' stroke='%237e106b'/%3E%3C/svg%3E");
            --hover-focused-branch-tree-symbol: url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='400' height='400' viewBox='0 0 105.83333 105.83334'%3E%3Cpath d='M4.8645178 36.435266H44.988572m18.053281 7.477892a25.531159 25.531159 0 00-18.053281-7.477892m44.274625 23.124007h11.653483m-29.706763-7.477892a25.531159 25.531159 0 0018.05328 7.477892m-18.05328-7.477892l-8.168064-8.168223' stroke-width='9.08617' stroke-linecap='round' fill='none' stroke='%23882F7D'/%3E%3C/svg%3E");    
            --hover-branch-tree-symbol: url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='400' height='400' viewBox='0 0 105.83333 105.83334'%3E%3Cpath d='M4.8645178 36.435266H44.988572m18.053281 7.477892a25.531159 25.531159 0 00-18.053281-7.477892m44.274625 23.124007h11.653483m-29.706763-7.477892a25.531159 25.531159 0 0018.05328 7.477892m-18.05328-7.477892l-8.168064-8.168223' stroke-width='9.08617' stroke-linecap='round' fill='none' stroke='%238C3E83'/%3E%3C/svg%3E");
            /* svg alternate lines */
            --alt-focused-branch-tree-symbol: url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='400' height='400' viewBox='0 0 105.83333 105.83334'%3E%3Cpath d='M4.8645178 36.435266H44.988572m18.053281 7.477892a25.531159 25.531159 0 00-18.053281-7.477892m44.274625 23.124007h11.653483m-29.706763-7.477892a25.531159 25.531159 0 0018.05328 7.477892m-18.05328-7.477892l-8.168064-8.168223' stroke-width='9.08617' stroke-linecap='round' fill='none' stroke='%238832AC'/%3E%3C/svg%3E");
            --alt-hover-focused-branch-tree-symbol: url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='400' height='400' viewBox='0 0 105.83333 105.83334'%3E%3Cpath d='M4.8645178 36.435266H44.988572m18.053281 7.477892a25.531159 25.531159 0 00-18.053281-7.477892m44.274625 23.124007h11.653483m-29.706763-7.477892a25.531159 25.531159 0 0018.05328 7.477892m-18.05328-7.477892l-8.168064-8.168223' stroke-width='9.08617' stroke-linecap='round' fill='none' stroke='%237D4793'/%3E%3C/svg%3E");    
            --alt-hover-branch-tree-symbol: url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='400' height='400' viewBox='0 0 105.83333 105.83334'%3E%3Cpath d='M4.8645178 36.435266H44.988572m18.053281 7.477892a25.531159 25.531159 0 00-18.053281-7.477892m44.274625 23.124007h11.653483m-29.706763-7.477892a25.531159 25.531159 0 0018.05328 7.477892m-18.05328-7.477892l-8.168064-8.168223' stroke-width='9.08617' stroke-linecap='round' fill='none' stroke='%23815892'/%3E%3C/svg%3E");
            /* svg position variables */
            --branch-tree-symbol-size: 30px;
            --branch-tree-symbol-position-x: 12px;
            --branch-tree-symbol-position-y: -3px;
        }
        ```
    - [ ] TreeNode Blue/Lightblue
      - [ ] Lines
        ```css
        /* TreeNode Lines Blue/Lightblue */
        :root {
        /* bullet color */
            --bullet-color: #797E7F;
            --hover-bullet-color: #2D80DB;
            --focused-bullet-color: #146BCB;
        /*Tree Lines*/
            --tree-lines-color: #356EAE;
            --hover-tree-lines-color: var(--hover-bullet-color);
            --focused-tree-lines-color: var(--focused-bullet-color);
            --tree-focused-bullet-color: var(--focused-bullet-color);
            --tree-hover-focused-bullet-color: #2875CB;
        /*if Alternating lines indent color ON */    
            --alt-tree-lines-color: #536E87;
            --alt-hover-tree-lines-color: #5182AD;
            --alt-focused-tree-lines-color: #4B90CC;
            --alt-tree-focused-bullet-color: #4B90CC;
            --alt-tree-hover-bullet-color: #5182AD;
            --alt-tree-hover-focused-bullet-color: #67A7DE;
        }
        ```
      - [ ] Branch symbol
        ```css
        /* TreeNode branch symbols Blue/Lightblue */
        :root {
            /* svg main lines */
            --focused-branch-tree-symbol: url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='400' height='400' viewBox='0 0 105.83333 105.83334'%3E%3Cpath d='M4.8645178 36.435266H44.988572m18.053281 7.477892a25.531159 25.531159 0 00-18.053281-7.477892m44.274625 23.124007h11.653483m-29.706763-7.477892a25.531159 25.531159 0 0018.05328 7.477892m-18.05328-7.477892l-8.168064-8.168223' stroke-width='9.08617' stroke-linecap='round' fill='none' stroke='%23146BCB'/%3E%3C/svg%3E");
            --hover-branch-tree-symbol: url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='400' height='400' viewBox='0 0 105.83333 105.83334'%3E%3Cpath d='M4.8645178 36.435266H44.988572m18.053281 7.477892a25.531159 25.531159 0 00-18.053281-7.477892m44.274625 23.124007h11.653483m-29.706763-7.477892a25.531159 25.531159 0 0018.05328 7.477892m-18.05328-7.477892l-8.168064-8.168223' stroke-width='9.08617' stroke-linecap='round' fill='none' stroke='%232D80DB'/%3E%3C/svg%3E");
            --hover-focused-branch-tree-symbol: url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='400' height='400' viewBox='0 0 105.83333 105.83334'%3E%3Cpath d='M4.8645178 36.435266H44.988572m18.053281 7.477892a25.531159 25.531159 0 00-18.053281-7.477892m44.274625 23.124007h11.653483m-29.706763-7.477892a25.531159 25.531159 0 0018.05328 7.477892m-18.05328-7.477892l-8.168064-8.168223' stroke-width='9.08617' stroke-linecap='round' fill='none' stroke='%232875CB'/%3E%3C/svg%3E");
            /* svg alternate lines*/
            --alt-focused-branch-tree-symbol: url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='400' height='400' viewBox='0 0 105.83333 105.83334'%3E%3Cpath d='M4.8645178 36.435266H44.988572m18.053281 7.477892a25.531159 25.531159 0 00-18.053281-7.477892m44.274625 23.124007h11.653483m-29.706763-7.477892a25.531159 25.531159 0 0018.05328 7.477892m-18.05328-7.477892l-8.168064-8.168223' stroke-width='9.08617' stroke-linecap='round' fill='none' stroke='%234B90CC'/%3E%3C/svg%3E");
            --alt-hover-branch-tree-symbol: url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='400' height='400' viewBox='0 0 105.83333 105.83334'%3E%3Cpath d='M4.8645178 36.435266H44.988572m18.053281 7.477892a25.531159 25.531159 0 00-18.053281-7.477892m44.274625 23.124007h11.653483m-29.706763-7.477892a25.531159 25.531159 0 0018.05328 7.477892m-18.05328-7.477892l-8.168064-8.168223' stroke-width='9.08617' stroke-linecap='round' fill='none' stroke='%235182AD'/%3E%3C/svg%3E");
            --alt-hover-focused-branch-tree-symbol: url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='400' height='400' viewBox='0 0 105.83333 105.83334'%3E%3Cpath d='M4.8645178 36.435266H44.988572m18.053281 7.477892a25.531159 25.531159 0 00-18.053281-7.477892m44.274625 23.124007h11.653483m-29.706763-7.477892a25.531159 25.531159 0 0018.05328 7.477892m-18.05328-7.477892l-8.168064-8.168223' stroke-width='9.08617' stroke-linecap='round' fill='none' stroke='%2367A7DE'/%3E%3C/svg%3E");    
            /* svg position variables*/
            --branch-tree-symbol-size: 30px;
            --branch-tree-symbol-position-x: 12px;
            --branch-tree-symbol-position-y: -3px;
        }
        ```
  - [ ] **1 Body**
    ```css
    @import url("https://eustachi0.github.io/RemNoteThemes/CSS/01_Body.css");
    ```
  - [ ] **2 Scrollbars**
    ```css
    @import url("https://eustachi0.github.io/RemNoteThemes/CSS/02_Scrollbars.css");
    ```
  - [ ] **3 Portals**
    ```css
    @import url("https://eustachi0.github.io/RemNoteThemes/CSS/03_Portals.css");
    ```
  - [ ] **4 Side, Bottom, Nav Bars**
    ```css
    @import url("https://eustachi0.github.io/RemNoteThemes/CSS/04_SidebarNavbar.css");
    ```
  - [ ] **5 Highlight colours**
    ```css
    @import url("https://eustachi0.github.io/RemNoteThemes/CSS/05_HighlightColors.css");
    ```
  - [ ] **6 Search highlight boxes**
    ```css
    @import url("https://eustachi0.github.io/RemNoteThemes/CSS/06_SearchHighlightBoxes.css");
    ```
  - [ ] **7 Tags**
    ```css
    @import url("https://eustachi0.github.io/RemNoteThemes/CSS/07_Tags.css");
    ```
  - [ ] **8 Popups**
    ```css
    @import url("https://eustachi0.github.io/RemNoteThemes/CSS/08_Popups.css");
    ```
  - [ ] **9 Checkbox**
    ```css
    @import url("https://eustachi0.github.io/RemNoteThemes/CSS/09_Checkbox.css");
    ```
  - [ ] **10 Code block**
    ```css
    @import url("https://eustachi0.github.io/RemNoteThemes/CSS/10_CodeBlock.css");
    ```
  - [ ] **11 Flashcards**
    ```css
    @import url("https://eustachi0.github.io/RemNoteThemes/CSS/11_Flashcard.css");
    ```
  - [ ] **12 Sharing document**
    ```css
    @import url("https://eustachi0.github.io/RemNoteThemes/CSS/12_SharingDocument.css");
    ```
  - [ ] **13 Settings page**
    ```css
    @import url("https://eustachi0.github.io/RemNoteThemes/CSS/13_SettingsPage.css");
    ```
  - [ ] **14 Help Page**
    ```css
    @import url("https://eustachi0.github.io/RemNoteThemes/CSS/14_HelpPage.css");
    ```
  - [ ] **15 Highlighted focused rem**
    ```css
    @import url("https://eustachi0.github.io/RemNoteThemes/CSS/15_HighlightedFocusedRem.css");
    ```
  - [ ] **16 Windowed Panes**
    ```css
    @import url("https://eustachi0.github.io/RemNoteThemes/CSS/16_WindowedPanes.css");
    ```
  - [ ] **17 Latex**
    ```css
    @import url("https://eustachi0.github.io/RemNoteThemes/CSS/17_Latex.css");
    ```
  - [ ] **18 Branches**
    ```css
    @import url("https://eustachi0.github.io/RemNoteThemes/CSS/18_Branches.css");
    ```
  - [ ] **19 Showing the hamburger**
    ```css
    @import url("https://eustachi0.github.io/RemNoteThemes/CSS/19_ShowTheHamburger.css");
    ```
```
