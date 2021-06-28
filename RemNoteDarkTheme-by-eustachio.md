- # RemNote Dark Theme by eustachio
- Created by eustachio
- This is something I do for fun as I like simple and modern UI's. I wanted to make RemNote look awesome!!!
- Version 1.2
- Release date: 28 June 2021

```markdown
- # RemNote Dark Theme by eustachio v1.2 ##Todo
  - Designed, created and maintained by Eustachio
  - This theme has been created to work with the `Dark Mode ON`
  - This is something I do for fun as I like simple and modern UI's. I wanted to make RemNote look awesome!!!
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
  - Tested on MacOS (Big Sur) and Fedora 34 apps.
  - https://github.com/eustachi0/RemNoteThemes/blob/main/RemNoteDarkTheme-by-eustachio.md
  - For bugs and suggestions, please drop me an email to: `eustachio.dipaola@gmail.com` with some screenshots if possible.
  - Please enable "Alternating Line Indent Colors" to see the treelines in two different colors.
  - By default "Optionals" blocks are deactivated, you can play with each block by unchecking them and see what they do.
  - For future updates, I recommend that you create a CSS code block at the bottom after this theme for your custom lines of code, things that you would like your way. So when an update, you can delete this theme and paste the new updated version without losing your customizations.
  - Latex and Image Occlusion jumps/glitches (on hover) seem to happen with and without the theme.
  - ## 0 Variable ##Todo
    - [ ] **General Customizations**
      ```css
      :root {
      /*body*/
          --body-background-color: rgb(38, 40, 40);
          --body-text-color: #DADADA;
          --accent-color: #8DABCC;
          --focused-accent-color: #9EBFE4;
          --font-name: myfont;
          --rem-margin-left: -16px;
          --rem-padding-left: 16px;
          --selected-background-color: #283645;
          --blackout-background-color: rgb(33, 36, 36); /* mod 4 Jun 2021*/
      /*Focused rem*/
          --focused-background-color: rgb(25,30,30); 
          --hover-background-color: rgb(40, 43, 43);
          --focused-text-color: #FDFDFD;/*#DCDCDC*/
          --accent-color-filter: grayscale(1) invert(80%) sepia(5%) saturate(3440%) hue-rotate(182deg) brightness(87%) contrast(81%);
          --focused-accent-color-filter: grayscale(1) invert(77%) sepia(47%) saturate(535%) hue-rotate(181deg) brightness(96%) contrast(86%);
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
          --sidebar-background-color: rgb(30, 32, 32);
          --sidebar-text-color: #BFBFBF;
          --sidebar-hover-background-color: rgb(39, 41, 41);
          --sidebar-hover-text-color: #D8D8D8;
          --nodocuments-text-color: rgb(88, 90, 90);
          --queue-indicator-icon-color: orange;
          --sidebar-focused-background-color: rgb(48, 50, 50);
          --sidebar-focused-left-border-color: rgb(48, 50, 50);
          --sidebar-focused-left-border-width: 0px;
          --sidebar-focused-text-color: white;
          --bars-border-color: rgb(52, 54, 54);
          --bars-border-width: 1px;
          --bars-border-radius: 7px;
      /* icons */
          --icons-color: #797E7F; /*#6F7E95*/
          --icons-filter: invert(51%) sepia(6%) saturate(227%) hue-rotate(142deg) brightness(95%) contrast(83%);
      /* popups */
          --popup-background-color: rgb(40, 42, 42);
          --popup-text-color: var(--body-text-color);
          --popup-hover-background-color: rgb(48, 50, 50); /* modified 05 Jun 2021*/
          --popup-selected-background-color: rgb(56, 58, 58); /*added 04 Jun 2021*/
          --popup-hover-text-color: var(--body-text-color);
          --popup-border-radius: 6px;
          --popup-border-color: rgb(50, 52, 52);
          --popup-border-width: 1px;
          --popup-keycode-color: var(--accent-color);
      /* queue */
          --queue-fill-in-the-blank-color: #6060CA;/*modified 04 Jun 2021*/
      /* scrollbar color*/
          --scrollbar-color: rgb(59, 61, 61); /*modified 04 Jun 2021*/
          --scrollbar-hover-color: rgb(69, 71, 71); /*modified 09 Jun 2021*/
          --scrollbar-track-color: rgb(42, 44, 44); /*added 09 Jun 2021*/
      /* toggle checkbox*/   
          --toggle-background-color: rgb(28, 30, 30);/*mod 08 Jun 2021*/
          --toggle-color: #CECECE;
      /* knowledge base page*/
          --knowledgebasepage-background-color: rgb(40, 42, 42);
          --knowledgebasepage-title-background-color: rgb(48, 50, 50);
      /*portals*/
          --portal-background-color: rgb(42, 44, 44);
          --portal-text-color: #C4C4C4;
          --embeddedsearch-background-color: rgb(39, 41, 41);
          --portal-border-color: rgb(42, 44, 44);
          --portal-inside-portal-border-color: rgb(52, 54, 54);
          --portal-inside-portal-left-margin: 11px;
          --searchkeywordhighlight-color: #8E9664;
          --searchkeywordhighlight-text-color: white;
      /*borders radius*/
          --border-radius: 10px;
      /* code block */
          --code-block-text-color: #B6B6B6;
          --code-block-background-color: rgb(28, 30, 30);
          --code-block-focused-background-color: rgb(22, 24, 24);
          --code-block-border-color: #49525B;
          --code-block-border-width: 2px;
      /* settings buttons color */
          --button-color: #435371;
      }
      ```
    - [x] **Bright highlight colors**
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
          --highlight-blue: rgb(25, 97, 201, 80%);
          --highlight-blue-focused: rgb(25, 97, 201, 90%);
          /*purple*/
          --highlight-purple: rgb(106, 26, 196, 80%);
          --highlight-purple-focused: rgb(106, 26, 196, 90%);
      }
      ```
    - [ ] **Light highlight colors**
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
    - [x] **TreeNode Purple/Magenta**
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
    - [ ] **TreeNode Blue/Lightblue**
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
            --alt-focused-tree-lines-color: #4B90CC/*#36A6B2*/;
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
  - ## 1 Body ##Todo
    ```css
    .dark-mode, .dark-mode-filter {
        filter: invert(0%) hue-rotate(0deg);
    }
    .dark-mode, .dark-mode-background {
        background-color: var(--body-background-color);
    }
    #ExamplesPageContainer .dark-mode #ExamplesPageContent, #export-container .dark-mode #export, #HelpPage .dark-mode #HelpPageContent, #sign-up-page-container .dark-mode #sign-up-page, #StatsPage .dark-mode #StatsPageContent, .dark-mode #ExamplesPageContainer #ExamplesPageContent, .dark-mode #export-container #export, .dark-mode #HelpPage #HelpPageContent, .dark-mode #sign-up-page-container #sign-up-page, .dark-mode #StatsPage #StatsPageContent, .dark-mode .centered-page, .dark-mode .document--narrow {
        background-color: var(--body-background-color);
    }
    body {
        background-color: var(--body-background-color);
        font-family: var(--font-name), -apple-system,BlinkMacSystemFont,segoe ui,Roboto,Helvetica,Arial,sans-serif,apple color emoji,segoe ui emoji,segoe ui symbol; 
        font-size: 15px;
        color: var(--body-text-color);
    }
    #ExamplesPageContainer #ExamplesPageContent, #export-container #export, #HelpPage #HelpPageContent, #sign-up-page-container #sign-up-page, #StatsPage #StatsPageContent, .centered-page, .document--narrow {
        background-color: var(--body-background-color);
    }
    /*----- this makes the 3 dots visible when in multiple window mode -----*/
    #multiple-windows .multiple-windows__document .document--narrow {
        padding-left: 42px;
        margin-top: -10px;
        padding-right: 25px;
    }
    #document {
        width: calc(100% - 65px);
    }
    /*----------------------------------------------*/
    #multiple-windows .multiple-windows__document {
        background-color: var(--body-background-color);
    }
    /* added 08 June 2021*/
    .tile__document {
        background-color: var(--body-background-color)!important;
    }
    #hierarchy-editor .rem-container .rem-text {
        color: var(--body-text-color);
        margin-left: 0px;
        margin-right: 0px;
        padding-left: 26px;
        padding-bottom: 3px!important;
    }
    #hierarchy-editor .rem {
        color: var(--body-text-color);
    }
    #hierarchy-editor .rem-container .concept_rem_type {
        color: var(--body-text-color);
    }
    #hierarchy-editor .rem-container .question_rem_type {
        color: var(--body-text-color);
    }
    .hierarchy-editor--ltr .rem-bullet__container {
        left: 2px;
    }
    .rem-bullet, .rem-bullet--in-list {
        width: 6px;
        height: 6px;
        background-color: var(--bullet-color);
        border-color: var(--collapse-bullet-border-color)!important;
    }
    .rem-bullet__icon.rem-bullet--hidden-children {
        background-color: var(--collapse-bullet-icon-border-color)!important;
    }
    .rem-container--not-in-article .rem-bullet__icon {
        border-color: var(--collapse-bullet-icon-border-color) !important;
        width: 13px !important;
        height: 10px !important;
    }
    .rem-bullet__container {
        top: 4px;
    }
    .rem-bullet__container-H1 {
        top: 4px;
    }
    .rem-bullet__container-H2 {
        top: 4px;
    }
    .rem-bullet__container-H3 {
        top: 4px;
    }
    /*document-top breadcrumbs*/
    #document-parents .RichTextViewer {
        color: var(--icons-color)!important;
        font-size: 12px;
    }
    #document-parents:hover .RichTextViewer {
        color: var(--accent-color)!important;
    }
    #document-parents .join-arrow {
        color: var(--icons-color)!important;
    }
    /* Document Title */
    #document #actionRequiredDocumentTitle, #document .document-title {
        font-size: 22px;
        font-weight: bold;
        color: var(--body-text-color)!important;
        margin-bottom: 15px;
    }
    .document-source {
        transition: opacity .09s;
        margin: .5em 0 .5rem;
        margin-top: 0.5em;
        margin-right: 0px;
        margin-bottom: 0.5rem;
        margin-left: 0px;
    }
    #document #AddNewDocumentButtonSmall {
        color: var(--body-text-color);
        font-size: 13px;
        font-style: italic;
    }
    #hierarchy-editor .is-toolbar-previous-focus-rem {
        box-shadow: 0 0 0px 0 rgba(85,205,196,0);
        border-radius: 2px;
        background-color: var(--focused-background-color);
    }
    .flash  {   
        background-color: var(--focused-background-color)!important;
        box-shadow: none;
        margin-left: 0px!important;
        padding-left: 0px!important;
    }
    .pane {
        padding-left: 0px;
    }
    #DocumentTable .Cell {
        color: var(--body-text-color);
    }
    #DocumentTable .ReactVirtualized__Table__headerRow {
        color: var(--body-text-color);
    }
    .gutter {
        background-color: var(--body-background-color);
        max-width: 2px!important;
        border-left-style: solid;
        border-left-width: var(--bars-border-width);
        border-left-color: var(--bars-border-color);
    }
    .gutter:hover {
        background-color: var(--accent-color);
        max-width: 2px!important;
        filter: brightness(0.8);
    }
    .rem-calendar-icon--today {
        filter: invert(47%) sepia(33%) saturate(684%) hue-rotate(91deg) brightness(93%) contrast(88%);
    }
    .LinkNode {
        text-decoration: underline;
        color: var(--link-text-color);
        font-weight: 500;
    }
    .rem-reference-link {
        color: var(--link-text-color);
        font-weight: 500;
    }
    .rem-indented-indicator {
        background-color: transparent;
    }
    .rem-reference-link:hover {
        background-color: transparent;
        color: var(--focused-accent-color);
    }
    .rem-reference--highlighted {
        border-color: rgba(0,0,0,0);
        box-shadow: none;
    }
    .rem-reference--focused {
        box-shadow: 0 0 0 0px rgba(0,0,0,0);
    }
    /* L a t e x */
    .katex {
        color: var(--latex-text-color);
    }
    .quote {
        background-color: var(--quote-background);
        color: var(--accent-color);
        border-radius: 0px!important;
        margin-left: 2px!important;
        margin-right: -2px!important;
        padding-left: 0px!important;
        padding-right: 0px!important;
        font-style: italic;
    }
    #hierarchy-editor .rem-container--default .quote {
        margin-right: -4px!important;
        margin-left: -4px!important;
        border-radius: 0px;
        padding: 0px!important;
        padding-left: 2px!important;
        padding-right: 2px!important;
    }
    #hierarchy-editor .rem-container--default:hover .quote {
        margin-right: -4px!important;
        margin-left: -4px!important;
        border-radius: 0px;
        padding: 0px!important;
        padding-left: 2px!important;
        padding-right: 2px!important;
        color: var(--focused-accent-color)!important;
    }
    #hierarchy-editor .rem-container--focused:hover .quote,
    #hierarchy-editor .rem-container--focused .quote {
        background-color: var(--focused-quote-background)!important;
        margin-right: -4px!important;
        margin-left: -4px!important;
        border-radius: 0px!important;
        padding: 0px!important;
        padding-left: 2px!important;
        padding-right: 2px!important;
        color: var(--focused-accent-color)!important;
    }
    /* web links logo*/
    #hierarchy-editor .rem-container .LinkNode img {
        filter: var(--accent-color-filter);
    }
    /* pdf highlight*/
    .rem-reference--pdf-highlight {
        border-color: transparent;
        border-bottom: solid transparent;
        border-width: 0px;
        color: var(--pdf-highlight-text-color);
        border-radius: 0px;
        text-decoration: underline;
    }
    #document #AddNewDocumentButtonSmall i {
        color: var(--icons-color);
    }
    #document #AddNewDocumentButtonSmall:hover i {
        color: var(--accent-color);
    }
    i.icons .corner.icon {
        text-shadow: -1px -1px 0 var(--body-background-color), 1px -1px 0 var(--body-background-color), -1px 1px 0 var(--body-background-color), 1px 1px 0 var(--body-background-color);
    }
    #document #add-new-document-button-text {
        color: var(--icons-color);
    }
    #document #add-new-document-button-text:hover {
        color: var(--accent-color);
    }
    i.icon.upload:before {
        color: var(--icons-color);
    }
    #help-button {
        color: var(--icons-color);
        box-shadow: none;
        background-color: var(--popup-background-color);
        border-style: solid;
        border-color: var(--bars-border-color);
    }
    #help-button:hover {
        color: var(--accent-color);
        box-shadow: none;
        background-color: var(--popup-hover-background-color);
    }
    .ui.message {
        background: var(--portal-background-color);
        color: var(--popup-text-color);
        border-radius: var(--popup-border-radius);
        border-color: var(--popup-border-color);
        box-shadow: none;
    }
    .ui.button {
        background: var(--popup-background-color);
        color: var(--popup-text-color);
        border-style: solid;
        border-color: var(--popup-border-color);
        border-width: var(--popup-border-width);
        border-radius: var(--popup-border-radius);
    }
    .ui.button:focus {
        background: var(--button-color);
        color: var(--popup-text-color);
    }
    .ui.button:hover {
        background: var(--button-color);
        color: var(--popup-text-color);
    }
    .ui.basic.button, .ui.basic.buttons {
        background: var(--popup-background-color)!important;
        color: var(--popup-text-color)!important;
        border-style: solid!important;
        border-color: var(--popup-border-color)!important;
        border-width: var(--popup-border-width)!important;
        border-radius: var(--popup-border-radius)!important;
    }
    .ui.basic.button:hover, .ui.basic.buttons:hover {
        background: var(--popup-hover-background-color)!important;
        color: var(--popup-text-color)!important;
        border-style: solid!important;
        border-color: var(--popup-border-color)!important;
        border-width: var(--popup-border-width)!important;
        border-radius: var(--popup-border-radius)!important;
    }
    .remHierarchyTop {
        margin-left: 10px;
    }
    .rem-hierarchy-bottom {
        margin-left: 9px;
    }
    .selected-rem  {
        background-color: var(--selected-background-color)!important;
    }
    #multiple-windows .multiple-windows__document .multiple-windows__close-pane__container .multiple-windows__close-pane {
        filter: var(--icons-filter);
    }
    #multiple-windows .multiple-windows__document .multiple-windows__close-pane__container .multiple-windows__close-pane:hover {
        filter: var(--accent-color-filter);
    }
    #SearchPopup {
        color: var(--body-text-color);
    }
    .work-in-progress-tag,
    .work-in-progress-rem {
        padding: 4px;
        border-radius: 5px;
        background-color: var(--search-box-background-color);
        color: var(--search-box-text-color) !important;
    }
    i.icon {
        color: var(--icons-color);
    }
    ```
  - ## 2 Scrollbars ##Todo
    ```css
    /*ScrollBar*/
    ::-webkit-scrollbar {
        width: 16px !important;
    }
    ::-webkit-scrollbar-track {
        background-color: var(--scrollbar-track-color) !important;
        border-radius: 0px;
    }
    ::-webkit-scrollbar-thumb {
        background-color: var(--scrollbar-color) !important;
        border-radius: 25px!important;
        border-style: solid!important;
        border-color: var(--scrollbar-track-color) !important;
        border-width: 4px!important;
    }
    ::-webkit-scrollbar-thumb:hover {
        background-color: var(--scrollbar-hover-color) !important;
        border-radius: 25px!important;
    }
    ```
  - ## 3 Portals ##Todo
    ```css
    #hierarchy-editor .TreeNode {
        border-color: var(--tree-lines-color);
        border-width: 2px !important;
        transition-timing-function: linear;
        position: relative;
        background-color: transparent;/*same color of body*/
        padding-left: var(--rem-padding-left);
        margin-left: 11px;
    }
    #hierarchy-editor .TreeNode--dark-indent-line {
        border-color: var(--alt-tree-lines-color) !important;
        border-width: 2px !important;
        background-color: transparent;/*same color of body*/
    }
    #hierarchy-editor .TreeNode--dark-indent-line:focus-within {
        border-color: var(--alt-focused-tree-lines-color) !important;
        border-width: 2px;
        background-color: transparent;/*same color of body*/
    }
    .hierarchy-editor--ltr .TreeNode {
        margin-left: 11px;
        padding-left: var(--rem-padding-left);
        border-left-style: solid;
    }
    .hierarchy-editor--ltr .TreeNode--list {
        margin-left: 11px;
        padding-left: var(--rem-padding-left);
        border-left-style: solid;
    }
    #hierarchy-editor .portal-rem {
        border-style: none none;
        border-top-style: none;
        border-right-style: none;
        border-bottom-style: none;
        border-left-style: none;
        border-width: 0px;
        margin-top: 10px;
        margin-left: -7px;
        margin-right: -7px;
        padding-top: 0px;
        height: 100%;
    }
    .dark-mode #show-embedded-search-button {
        background-color: var(--portal-background-color);
        padding-left: 10px;
        padding-top: 8px;
        padding-bottom: 10px;
        padding-right: 10px;
        margin-top: 10px;
        margin-bottom: 8px;
        border-color: var(--portal-border-color)!important;
        border: 2px solid var(--portal-border-color)!important;
        border-top: 2px solid var(--portal-border-color)!important;
        border-radius: var(--border-radius);
        border-bottom-right-radius: var(--border-radius);
        border-bottom-left-radius: var(--border-radius);
        margin-right: 6px;
        margin-left: 0px;
        color: grey;
        font-weight: 400;
    }
    .dark-mode .TreeNode #show-embedded-search-button {
        margin-left: 10px!important;
    }
    .embeddedSearch {
        border-top-left-radius: var(--border-radius);
        border-top-right-radius: var(--border-radius);
        border-bottom-right-radius: var(--border-radius);
        border-bottom-left-radius: var(--border-radius);
        border: 1px solid rgba(0,0,0,0);
        border-top-color: rgba(0,0,0,0);
        border-top-style: solid;
        border-top-width: 1px;
        border-right-color: rgba(0,0,0,0);
        border-right-style: solid;
        border-right-width: 1px;
        border-bottom-color: rgba(0,0,0,0);
        border-bottom-style: solid;
        border-bottom-width: 1px;
        border-left-color: rgba(0,0,0,0);
        border-left-style: solid;
        border-left-width: 1px;
        padding-top: 5px;
        padding-right: 5px;
        padding-bottom: 6px;
        padding-left: 10px;
        margin-bottom: 5px;
        margin-left: 10px;
        margin-right: 10px;
        margin-top: 0px;
        background-color: var(--embeddedsearch-background-color);
    }
    /*modified 28 Jun 2021*/
    #hierarchy-editor .portal-rem--embedded-search {
        background-color: var(--portal-background-color)!important;
        margin-right: 6px!important;
        padding-top: 0px!important;
        margin-top: 18px!important;
        margin-left: 0px!important;
        padding-bottom: 14px!important;
        margin-bottom: 20px!important;
        border-color: var(--portal-border-color)!important;
        border-left: 2px solid var(--portal-border-color)!important;
        border-right: 2px solid var(--portal-border-color)!important;
        border-bottom: 0px solid!important;
        border-bottom-right-radius: 0px!important;
        border-bottom-left-radius: 0px!important;
    }
    /*modified 28 Jun 2021*/
    #hierarchy-editor .TreeNode .portal-rem--embedded-search {
        margin-left: 10px!important;
    }
    #hierarchy-editor .search-portal-tree-node--dark {
        border-bottom-width: 0px;
        border-top-width: 0px;
        border-left: 2px solid var(--portal-border-color);
        border-bottom: 2px solid var(--portal-border-color);
        border-right: 2px solid var(--portal-border-color);
        border-top-color: rgb(0,0,0,0);
        margin-left: 0px;
        margin-right: 6px;
        padding-left: 6px;
        padding-right: 9px;
        padding-bottom: 10px;
        margin-bottom: 7px;
        margin-top: -30px;
        background-color: var(--portal-background-color);
        border-bottom-right-radius: var(--border-radius);
        border-bottom-left-radius: var(--border-radius);
    }
    #hierarchy-editor .TreeNode .search-portal-tree-node--dark {
        margin-left: 10px;
    }
    #hierarchy-editor .rem-container__top-level-spacer {
        margin-top: 10px;
        width: 100%;
        display: block;
    }
    #search-results__controls #search-results__control .search-results__control__keyboard-shortcut {
        margin-right: 0px;
        margin-left: 0px;
        background-color: green;
        border-radius: 30px;
        padding: 1px;
        padding-left: 6px;
        padding-right: 6px;
    }
    i.icon.search:before {
        content: "\f002";
        zoom: 125%;
        padding-top: 6px;
        padding-left: 2px;
        color: var(--icons-color);
    }
    /*modified 28 Jun 2021*/
    i.icon.refresh:before {
        content: "\f021";
        zoom: 120%;
        color: var(--icons-color);
    }
    /*modified 28 Jun 2021*/
    #embedded-search__button, .embedded-search__menu-button {
        float: right;
        padding-top: 6px;
        padding-right: 15px;
        padding-bottom: 10px;
        padding-left: 5px;
    }
    #no-search-results {
        background-color: var(--portal-background-color);
        color: var(--body-text-color);
        text-align: center;
        margin-top: 20px;
        margin-bottom: -20px;
        padding-bottom: 18px;
        margin-left: -2px;
        margin-right: -2px;
        border-top-style: none;
        border-left: 2px solid var(--portal-border-color);
        border-right: 2px solid var(--portal-border-color);
        border-bottom: 2px solid var(--portal-border-color);
        border-bottom-right-radius: var(--border-radius);
        border-bottom-left-radius: var(--border-radius);
    }
    #hierarchy-editor .portal-rem .portal-rem-top--embedded-search-top {
        border-color: rgb(0,0,0,0);
        text-align: right;
        border-top: solid rgb(0,0,0,0);
        border-width: 0px;
        position: relative;
        top: 0px;
        padding-top: 0px;
        margin-top: -25px;
    }
    .rem-indented-indicator {
        color: rgb(0,0,0,0);
        top: -1.8px;
        position: fixed;
    }
    #hierarchy-editor .isSearchResult {
        background-color: transparent;
        margin-top: 0px;
        margin-bottom: -0px;
        border: 0px solid rgb(0,0,0);
        border-radius: 0px;
        margin-right: 0px;
        margin-left: 0px;
        padding-left: 0px;
    }
    #hierarchy-editor .rem-container__top-level-rem-in-portal-border .rem-container__top-level-rem-in-portal-border__inner {
        display: none;
    }
    #hierarchy-editor .rem-container__top-level-spacer .rem-container__top-level-spacer__inner {
        border-color: rgb(0,0,0,0);
        border-top: solid rgb(0,0,0,0);
        border-width: 0px;
        bottom: 0px;
    }
    #hierarchy-editor .portal-rem .portal-rem-top, #hierarchy-editor .portal-rem .portal-rem-top--embedded-search-top {
        border-color: rgb(0,0,0,0);
        text-align: right;
        border-top: solid rgb(0,0,0);
        border-width: 0px;
        top: -4px;
        padding-top: 13px;
    }
    #hierarchy-editor .portal-tree-node {
        border-left: 2px solid var(--portal-border-color);
        border-right: 2px solid var(--portal-border-color);
        border-bottom: 2px solid var(--portal-border-color);
        border-top: 2px solid var(--portal-border-color);
        margin-left: 0px;
        margin-right: 6px;
        margin-top: -18px;
        margin-bottom: 10px;
        padding-left: 6px;
        padding-right: 9px;
        padding-top: 5px;
        padding-bottom: 10px;
        background-color: var(--portal-background-color);
        border-radius: var(--border-radius);
        border-bottom-right-radius: var(--border-radius);
        border-bottom-left-radius: var(--border-radius);
    }
    #hierarchy-editor .TreeNode .portal-tree-node {
        margin-left: 10px;
    }
    #hierarchy-editor .hierarchy-editor__after-portal .addItemAfterPortal {
        height: 25px;
        width: 100%;
        padding-left: 8px;
        margin-top: -8px;
        margin-bottom: -4px;
    }
    #hierarchy-editor .hierarchy-editor__after-portal {
        border-bottom-style: none;
        border-width: 0px;
        border-top-width: 0px;
        border-right-width: 0px;
        border-bottom-width: 0px;
        border-left-width: 0px;
        padding-top: 0px;
        padding-bottom: 0px;
        margin-left: -6px;
        margin-right: 7px;
    }
    .text-gray-500 {
        color: var(--accent-color);
        padding-top: 6px;
        padding-left: 8px;
    }
    /*---------- breadcrumbs inside portals ----------*/
    #hierarchy-editor .rem-container--not-included-in-document-scope .rem-text {
        padding-left: 26px !important;
    }
    #hierarchy-editor  .rem-container--not-included-in-document-scope .RichTextViewer  {
        font-size: 14px;
    }
    #hierarchy-editor  .rem-container--not-included-in-document-scope:hover .rem-text {
        background-color: transparent !important;
        margin-left: 0px;
        padding-left: 12px;
    }
    #hierarchy-editor .portal-tree-node .portal-tree-node .rem-container--not-included-in-document-scope:hover .rem-text {
        background-color: transparent !important;
        margin-left: 0px;
        padding-left: 12px;
    }
    #hierarchy-editor .portal-tree-node .search-portal-tree-node--dark .rem-container--not-included-in-document-scope:hover .rem-text {
        background-color: transparent !important;
        margin-left: 0px;
        padding-left: 12px;
    }
    #hierarchy-editor .search-portal-tree-node--dark .portal-tree-node .rem-container--not-included-in-document-scope:hover .rem-text {
        background-color: transparent !important;
        margin-left: 0px;
        padding-left: 12px;
    }
    #hierarchy-editor .search-portal-tree-node--dark .search-portal-tree-node--dark .rem-container--not-included-in-document-scope:hover .rem-text {
        background-color: transparent !important;
        margin-left: 0px;
        padding-left: 12px;
    }
    #hierarchy-editor .rem-container--not-included-in-document-scope .notIncludedAncestorClickable:hover {
        color: var(--accent-color);
        font-weight: 400;
        font-size: 14px;
    }
    #hierarchy-editor .rem-container--not-included-in-document-scope .notIncludedAncestorClickable {
        color: var(--body-text-color);
        font-weight: 400;
        font-size: 14px;
    }
    /*----------------------------------------------------*/
    #show-embedded-search-button #show-embedded-search-button__delete-button {
        filter: var(--icons-filter);
    }
    #show-embedded-search-button #show-embedded-search-button__delete-button:hover {
        filter: var(--accent-color-filter);
    }
    /* portals inside portals*/
    /* search inside portal */
    #hierarchy-editor .portal-tree-node #show-embedded-search-button  {
        border-color: var(--portal-inside-portal-border-color)!important;
        margin-left: var(--portal-inside-portal-left-margin);
    }
    #hierarchy-editor .search-portal-tree-node--dark #show-embedded-search-button  {
        border-color: var(--portal-inside-portal-border-color)!important;
        margin-left: var(--portal-inside-portal-left-margin);
    }
    #hierarchy-editor .portal-tree-node .portal-rem {
        border-color: var(--portal-inside-portal-border-color)!important;
        margin-left: var(--portal-inside-portal-left-margin);
    }
    #hierarchy-editor .search-portal-tree-node--dark .portal-rem {
        border-color: var(--portal-inside-portal-border-color)!important;
        margin-left: var(--portal-inside-portal-left-margin);
    }
    #hierarchy-editor .portal-tree-node .search-portal-tree-node--dark {
        border-color: var(--portal-inside-portal-border-color)!important;
        margin-left: var(--portal-inside-portal-left-margin);
    }
    #hierarchy-editor .search-portal-tree-node--dark .search-portal-tree-node--dark {
        border-color: var(--portal-inside-portal-border-color)!important;
        margin-left: var(--portal-inside-portal-left-margin);
    }
    #hierarchy-editor .portal-tree-node #no-search-results  {
        border-color: var(--portal-inside-portal-border-color)!important;
    }
    #hierarchy-editor .search-portal-tree-node--dark #no-search-results  {
        border-color: var(--portal-inside-portal-border-color)!important;
    }
    #hierarchy-editor .portal-tree-node .portal-tree-node {
        border-left: 2px solid var(--portal-inside-portal-border-color);
        border-right: 2px solid var(--portal-inside-portal-border-color);
        border-bottom: 2px solid var(--portal-inside-portal-border-color);
        border-top: 2px solid var(--portal-inside-portal-border-color);
        margin-left: var(--portal-inside-portal-left-margin);
        margin-right: 6px;
        margin-top: -16px;
        margin-bottom: 10px;
        padding-left: 7px;
        padding-right: 9px;
        padding-top: 6px;
        padding-bottom: 10px;
        background-color: var(--portal-background-color);
        border-radius: var(--border-radius);
        border-bottom-right-radius: var(--border-radius);
        border-bottom-left-radius: var(--border-radius);
    }
    #hierarchy-editor .search-portal-tree-node--dark .portal-tree-node {
        border-left: 2px solid var(--portal-inside-portal-border-color);
        border-right: 2px solid var(--portal-inside-portal-border-color);
        border-bottom: 2px solid var(--portal-inside-portal-border-color);
        border-top: 2px solid var(--portal-inside-portal-border-color);
        margin-left: var(--portal-inside-portal-left-margin);
        margin-right: 6px;
        margin-top: -16px;
        margin-bottom: 10px;
        padding-left: 7px;
        padding-right: 9px;
        padding-top: 6px;
        padding-bottom: 10px;
        background-color: var(--portal-background-color);
        border-radius: var(--border-radius);
        border-bottom-right-radius: var(--border-radius);
        border-bottom-left-radius: var(--border-radius);
    }
    ```
  - ## 4 Side, Bottom, Nav Bars ##Todo
    ```css
    .dark-mode #document-sidebar {
        background-color: var(--sidebar-background-color)!important;
    }
    #homepage #content .document-sidebar--pinned, #main #content .document-sidebar--pinned {
        height: 100%;
    }
    #homepage #content .document-sidebar--floating, #main #content .document-sidebar--floating {
        box-shadow: none;
        border-top-left-radius: 0px;
        border-top-right-radius: var(--bars-border-radius);
        border-bottom-left-radius: 0px;
        border-bottom-right-radius: var(--bars-border-radius);
        z-index: 7!important;
        background-color: var(--sidebar-background-color)!important;
    }
    #homepage #content #document-sidebar, #main #content #document-sidebar {
        background-color: var(--sidebar-background-color)!important;
        color: var(--sidebar-text-color)!important;
    }
    #DocumentationList .documentListNoDocuments, #documentList .documentListNoDocuments {
        color: var(--nodocuments-text-color);
    }
    #document-sidebar_top {
        background-color: var(--sidebar-top-background-color);
        border-right-style: solid;
        border-bottom-style: solid;
        border-color: var(--bars-border-color);
        border-width: var(--bars-border-width);
    }
    .document-sidebar--floating #document-sidebar_top {
        border-top-style: solid;
        border-color: var(--bars-border-color);
        border-width: var(--bars-border-width);
        border-top-right-radius: var(--bars-border-radius);
    }
    #DocumentationList, #documentList {
        border-right-style: solid;
        border-bottom-style: solid;
        border-color: var(--bars-border-color);
        border-width: var(--bars-border-width);
    }
    #document-sidebar__bottom-menu {
        border-right-style: solid;
        border-color: var(--bars-border-color);
        border-width: var(--bars-border-width);
        margin-left: calc(-1 * var(--bars-border-width)) !important;
    }
    .document-sidebar--floating #document-sidebar__bottom-menu {
        border-right-style: solid;
        border-bottom-style: solid;
        border-color: var(--bars-border-color);
        border-width: var(--bars-border-width);
        border-bottom-right-radius: 0px;
        margin-left: calc(-1 * var(--bars-border-width)) !important;
        border-bottom-right-radius: var(--bars-border-radius);
    }
    /*logo*/
    #document-sidebar_top #logo img {
        filter: contrast(1) brightness(1.2) grayscale(0);
        opacity: .5;
        height: 25px;
    } 
    #document-sidebar_top #logo img:hover {
        filter: contrast(1) brightness(1.2) grayscale(0);
        opacity: .8;
    } 
    #document-sidebar_top #logo {
        display: block;
        margin-top: 15px;
    }
    #document-sidebar__account-capsule:hover {
        background-color: var(--sidebar-hover-background-color);
    }
    #document-sidebar__collapse-icon__container img {
        filter: var(--icons-filter);
    }
    #document-sidebar__collapse-icon__container:hover img {
        filter: var(--accent-color-filter);
    }
    #document-sidebar__collapse-icon__container:hover {
        background-color: var(--sidebar-hover-background-color);
    }
    #acc-capsule__menu {
        background-color: var(--popup-background-color);
        border: var(--popup-border-width) solid var(--popup-border-color);
        color: var(--popup-text-color);
        border-radius: var(--popup-border-radius);
    }
    .acc-capsule__menu__title {
        color: var(--popup-text-color);
    }
    .acc-capsule__menu__account .acc-capsule__menu__name {
        color: var(--accent-color);
    }
    .acc-capsule__menu__account .acc-capsule__menu__email {
        color: var(--accent-color);
        font-size: 12px;   
    }
    .acc-capsule__menu__account {
        border-bottom: 0px;
    }
    .acc-capsule__menu__element--hoverable:hover {
        border-bottom: 0px;
    }
    .acc-capsule__menu__element--hoverable:hover {
        background-color: var(--popup-hover-background-color);
        color: var(--popup-hover-text-color);
    }
    .switch-knowledgebase .switch-knowledgebase__knowledgebase, .switch-knowledgebase .switch-knowledgebase__knowledgebase .switch-knowledgebase__knowledgebase__button {
        background-color: var(--popup-background-color);
        color: var(--accent-color);
    }
    .switch-knowledgebase .switch-knowledgebase__knowledgebase:hover, .switch-knowledgebase .switch-knowledgebase__knowledgebase .switch-knowledgebase__knowledgebase__button:hover {
        background-color: var(--popup-hover-background-color);
        color: var(--accent-color);
    }
    .switch-knowledgebase {
        border-color: var(--popup-border-color);
    }
    /* queue */
    #document-sidebar__link {
        color: var(--sidebar-text-color);
        margin-left: 5px !important;
        margin-right: 5px !important;
        padding-left: 10px !important;
        padding-right: 5px !important;
    }
    #document-sidebar__link:hover {
        background-color: var(--sidebar-hover-background-color) !important;
        color: var(--sidebar-hover-text-color);
    }
    .flashcards-icon {
        filter: var(--icons-filter); 
    }
    #document-sidebar__link__queue-indicator {
        background-color: transparent;
    }
    #document-sidebar__link__queue-indicator .icon {
        color: var(--queue-indicator-icon-color)!important;
    }
    /* documents */
    #document-sidebar__document-buttons .document-sidebar__document-buttons__button {
        filter: var(--icons-filter);
    }
    #document-sidebar__document-buttons .document-sidebar__document-buttons__button:hover {
        filter: var(--accent-color-filter);
    }
    #homepage #content #document-sidebar a, #main #content #document-sidebar a {
        color: var(--sidebar-text-color) !important;
    }
    #homepage #content #document-sidebar a:hover, #homepage #content #document-sidebar a:visited, #main #content #document-sidebar a:hover, #main #content #document-sidebar a:visited {
        color: var(--sidebar-text-color) !important;
    }
    #document-sidebar__document-buttons:hover  {
        background-color: var(--sidebar-hover-background-color) !important;
    }
    #homepage #content #document-sidebar a:hover, #main #content #document-sidebar a:hover {
        color: var(--sidebar-hover-text-color) !important;
    }
    #homepage #content #document-sidebar .document-sidebar__linkOpen  a, #main #content #document-sidebar .document-sidebar__linkOpen a {
        color: var(--sidebar-focused-text-color) !important;
    }
    .document-sidebar__linkOpen {
        background-color: var(--sidebar-focused-background-color)!important;
        border-left-style: none;
        border-left-color: var(--sidebar-focused-left-border-color);
        border-left-width: var(--sidebar-focused-left-border-width);
        border-radius: 7px;
        margin-left: 5px !important;
        margin-right: 5px !important;
        color: var(--sidebar-focused-text-color) !important;
    }
    .document-sidebar__linkOpen #document-sidebar__document-buttons__document-link-container {
        padding-left: 10px !important;
    }
    .document-sidebar__linkOpen .document-sidebar__document-buttons__button-container {
        padding-right: 5px !important;
    }
    /* knowledgebase page*/
    #KnowledgeBasePage {
        background-color: var(--knowledgebasepage-background-color);
    }
    #KnowledgeBasePage #KnowledgeBaseButtons .KnowledgeBaseButtons__display-settings {
        color: var(--body-text-color);
    }
    #KnowledgeBasePage #KnowledgeBaseButtons button {
        background-color: var(--body-background-color);
        color: var(--body-text-color);
    }
    #DocumentTable .ReactVirtualized__Table__headerRow {
        color: var(--accent-color);
        background-color: var(--knowledgebasepage-title-background-color);
        box-shadow: none !important;
        border-radius: 10px 10px 0px 0px;
    }
    #DocumentTable .ReactVirtualized__Grid {
        background-color: var(--knowledgebasepage-background-color);
        border-radius: 0 0 10px 10px;
        box-shadow: none !important;
        border-style: solid;
        border-color: var(--knowledgebasepage-title-background-color) !important;
    }
    #DocumentTable a, .black-links a {
        text-decoration: none!important;
        color: var(--body-text-color) !important;
    }
    #DocumentTable a:hover, .black-links a:hover {
        text-decoration: none!important;
        background-color: var(--hover-background-color) !important;
        color: var(--body-text-color) !important;
    }
    #documentList .document-list-item__plus-icon {
        filter: var(--icons-filter) !important;
    }
    #documentList .document-list-item__plus-icon:hover {
        filter: brightness(0.8) !important;
    }
    #DocumentationList .folder-float-button:hover, #documentList .folder-float-button:hover {
        -webkit-filter: var(--accent-color-filter) !important;
        filter: var(--accent-color-filter) !important;
    }
    .document-sidebar__document-buttons__menu:hover .document-sidebar__document-buttons__menu__button:hover {
        background-color: var(--popup-hover-background-color);
        color: var(--popup-hover-text-color);
    }
    .document-sidebar__document-buttons__menu:hover .document-sidebar__document-buttons__menu__button:hover {
        background-color: var(--popup-hover-background-color);
        color: var(--popup-hover-text-color);
    }
    #DocumentationList .document-list-item .document-list-item__folder-icon-container, #documentList .document-list-item .document-list-item__folder-icon-container {
        filter: var(--icons-filter);
    }
    /* bottom bar */
    /* added 09 June 2020 */
    #hierarchy-editor-toolbar-container {
        background-color: var(--body-background-color);
        margin-bottom: 3px;
        border-radius: var(--bars-border-radius);
    }
    .hierarchy-editor-toolbar-container--thin {
        display: flow-root;
        border-color: var(--bars-border-color)!important;
        border-top: solid var(--bars-border-color);
        border-width: var(--bars-border-width)!important;
        border-radius: var(--bars-border-radius)!important;
        background-color: var(--body-background-color)!important;
        height: 28px!important;
        margin-bottom: 2px!important;
    }
    .hierarchy-editor-toolbar-container--opened #hierarchy-editor-toolbar {
        background-color: var(--sidebar-background-color);
        border-style: solid;
        border-width: var(--bars-border-width);
        border-color: var(--bars-border-color);
        border-radius: var(--bars-border-radius);
    }
    .hierarchy-editor-toolbar-container--opened #hierarchy-editor-toolbar .hierarchy-editor-toolbar-item {
        color: var(--icons-color);
    }
    .hierarchy-editor-toolbar-container--opened #hierarchy-editor-toolbar .hierarchy-editor-toolbar-item__type-icon--dark {
        -webkit-filter: var(--icons-filter);
        filter: var(--icons-filter);
    }
    .hierarchy-editor-toolbar-container--opened #hierarchy-editor-toolbar .hierarchy-editor-toolbar-item__type-icon--dark:hover {
        -webkit-filter: var(--focused-accent-color-filter);
        filter: var(--focused-accent-color-filter);
    }
    .hover-card-menu__view-as-card {
        background-color: var(--popup-background-color);
        border-radius: var(--popup-border-radius) !important;
    }
    .hover-card-menu__view-as-card .view-as-card__no-card-focus {
        color: var(--popup-text-color);
    }
    .hover-card-menu__view-as-card .view-as-card__no-card-focus #quote {
        background-color: var(--popup-background-color);
        border-color: var(--popup-border-color);
        color: var(--popup-text-color);
    }
    /* modified 04 Jun 2021*/
    .hover-card-menu__view-as-card--on-right {
        background-color: var(--blackout-background-color)!important;
        margin-left: 40px;
        border: var(--bars-border-width) solid var(--bars-border-color);
    }
    /* modified 04 Jun 2021*/
    #view-as-card #view-as-card__cards .view-as-card__card .spacedRepetition {
        border: 2px solid var(--popup-border-color);
        box-shadow: none;
        border-radius: var(--popup-border-radius);
    }
    /* added 04 Jun 2021 */
    #hierarchy-editor .rem-bullet__number:hover {
      color: var(--focused-text-color);
    }
    #view-as-card #view-as-card__cards .view-as-card__card .scroll-drag-component {
        background-color: transparent;
    }
    #view-as-card #view-as-card__cards .view-as-card__card .spacedRepetition .spacedRepetitionContent {
        border-top-right-radius: var(--popup-border-radius);
        border-top-left-radius: var(--popup-border-radius);
    }
    /* modified 04 Jun 2021*/
    .hierarchy-editor-toolbar-container--opened #hierarchy-editor-toolbar .hierarchy-editor-toolbar-item__type-icon {
        -webkit-filter: var(--accent-color-filter) grayscale(.5) brightness(1.2);
        filter: var(--accent-color-filter) grayscale(0.5) brightness(1.2);
    }
    /* modified 04 Jun 2021*/
    .hierarchy-editor-toolbar-container--opened #hierarchy-editor-toolbar .hierarchy-editor-toolbar-item__type-icon:hover {
        -webkit-filter: var(--accent-color-filter) grayscale(0.4) brightness(1.4);
        filter: var(--accent-color-filter) grayscale(0.4) brightness(1.4);
    }
    /* added 05 Jun 2021*/
    .hierarchy-editor-toolbar__menu .hierarchy-editor-toolbar__menu__item {
        border-radius: 7px;
        margin-left: 6px!important;
        margin-right: 6px!important;
        padding-top: 6px!important;
      padding-bottom: 6px!important;
    }
    /* modified 04 Jun 2021*/
    .hierarchy-editor-toolbar__menu .hierarchy-editor-toolbar__menu__item:hover {
        background-color: var(--popup-hover-background-color);
        border-radius: 7px;
        margin-left: 6px!important;
        margin-right: 6px!important;
        padding-top: 6px!important;
      padding-bottom: 6px!important;
    }
    /* modified 04 Jun 2021*/
    .hierarchy-editor-toolbar__menu .hierarchy-editor-toolbar__menu__item--selected,
    .hierarchy-editor-toolbar__menu .hierarchy-editor-toolbar__menu__item--selected:hover {
        background-color: var(--popup-selected-background-color);
        border-radius: 7px;
        margin-left: 6px!important;
        margin-right: 6px!important;
        padding-top: 6px!important;
      padding-bottom: 6px!important;
    }
    /* modified 04 Jun 2021*/
    .hierarchy-editor-toolbar__menu .hierarchy-editor-toolbar__menu__item .hierarchy-editor-toolbar__menu__item__icon  {
        filter: var(--accent-color-filter) grayscale(1);
    }
    /* modified 04 Jun 2021*/
    .hierarchy-editor-toolbar__menu .hierarchy-editor-toolbar__menu__item:hover .hierarchy-editor-toolbar__menu__item__icon  {
        filter: var(--accent-color-filter) grayscale(0.4) brightness(1.4);
    }
    /* modified 04 Jun 2021*/
    .hierarchy-editor-toolbar__menu .hierarchy-editor-toolbar__menu__item--selected .hierarchy-editor-toolbar__menu__item__icon  {
        filter: var(--accent-color-filter) grayscale(0.5) brightness(1.2);
    }
    /* added 04 Jun 2021*/
    .hierarchy-editor-toolbar__menu .hierarchy-editor-toolbar__menu__item--selected:hover .hierarchy-editor-toolbar__menu__item__icon  {
        filter: var(--accent-color-filter) grayscale(0.5) brightness(1.2);
    }
    .hierarchy-editor-toolbar__menu #quote {
        background-color: var(--popup-background-color);
        border-color: var(--popup-border-color);
        color: var(--popup-text-color);
    }
    .hierarchy-editor-toolbar-container--opened #hierarchy-editor-toolbar .hierarchy-editor-toolbar__vertical-divider {
        border-color: var(--popup-border-color);
    }
    .hierarchy-editor-toolbar-container--opened .hierarchy-editor-toolbar__button {
        color: var(--icons-color);
    }
    .hierarchy-editor-toolbar-container--opened .hierarchy-editor-toolbar__button:hover {
        color: var(--accent-color)!important;
    }
    .hierarchy-editor-toolbar-container--opened .header-editor-toolbar__button-header {
        color: var(--accent-color)!important;
    }
    .hierarchy-editor-toolbar-container--opened .header-editor-toolbar__button-header i.icon.header:before {
        color: var(--icons-color);
    }
    .hierarchy-editor-toolbar-container--opened .header-editor-toolbar__button-header:hover i.icon.header:before {
        color: var(--accent-color);
    }
    .hierarchy-editor-toolbar-container--opened i.icon.circle:before,
    .hierarchy-editor-toolbar-container--opened i.icon.check.square:before,
    .hierarchy-editor-toolbar-container--opened i.icon.numbered.list:before,
    .hierarchy-editor-toolbar-container--opened i.icon.inbox:before,
    .hierarchy-editor-toolbar-container--opened i.icon.file:before,
    .hierarchy-editor-toolbar-container--opened i.icon.chess.board:before {
        color: var(--accent-color);
    }
    /* merge bottom */
    .hierarchy-editor-toolbar-container--opened #hierarchy-editor-toolbar .ToolbarDuplicateKeyButton {
        color: grey;
        border-radius: 5px;
        border: none;
        padding: 3px;
        margin-left: 5px;
        background-color: var(--popup-background-color);
    }
    .hierarchy-editor-toolbar-container--opened #hierarchy-editor-toolbar .ToolbarDuplicateKeyButton:hover {
        color: var(--accent-color);
        border-radius: 5px;
        border: none;
        padding: 3px;
        margin-left: 5px;
        background-color: var(--popup-hover-background-color);
    }
    .popup .toolbar-button {
        border-color: var(--popup-border-color);
        border-width: var(--popup-border-width);
        border-radius: var(--popup-border-radius);
        color: var(--popup-text-color);
    }
    .popup .toolbar-button:hover {
        border-color: var(--accent-color);
        color: var(--accent-color);
    }
    .popup .toolbar-button--selected__header {
        background-color: var(--popup-background-color);
    }
    .popup #BulletFormatIcons .BulletFormatIcons__icon__active, .popup #BulletFormatIcons .icon:hover {
        color: var(--accent-color) !important;
    }
    #hierarchy-editor-toolbar-container #hierarchy-editor__add-to-portal .rich-text-editor {
        border: var(--popup-border-width) solid var(--popup-border-color);
        border-radius: var(--popup-border-radius);
        background-color: var(--search-box-background-color);
        color: var(--popup-text-color);
        padding-top: 4px;
        margin-right: -7px;
    }
    .search-results #search-results__no-results {
        padding: 10px;
        color: var(--popup-text-color);
        background-color: var(--popup-background-color);
    }
    #hierarchy-editor-toolbar-container #hierarchy-editor__add-to-portal .search-results {
        box-shadow: none;
        border-style: solid;
        border-width: var(--popup-border-width);
        border-color: var(--popup-border-color);
        border-radius: var(--popup-border-radius);
    }
    .document-sidebar--collapsed--horizontal {
        border-color: rgba(0,0,0,0);
        border-bottom: solid rgba(0,0,0,0);
        border-width: thin;
        width: 100%;
        height: 40px;
        flex-shrink: 0;
    }
    .underlined-link {
        color: var(--accent-color);
    }
    /* document list*/
    #DocumentationList .document-list-item, #documentList .document-list-item {
        margin-left: 10px;
        margin-right: 10px;
        padding-top: 6px !important;
        padding-bottom: 6px !important;
        border-radius: 7px;
    }
    #DocumentationList .document-list-item--opened, #documentList .document-list-item--opened {
        font-weight: 600 !important;
        background-color: var(--sidebar-focused-background-color);
        border-width: var(--sidebar-focused-left-border-width);
        border-left-color: var(--sidebar-focused-left-border-color);
        font-size: 14px !important;
        color: var(--sidebar-focused-text-color) !important;
        margin-left: 10px !important;
        margin-right: 10px !important;
        border-radius: 7px;
    }
    /*Hover*/
    #DocumentationList .document-list-item:hover, #documentList .document-list-item:hover {
        background-color: var(--sidebar-hover-background-color);
        color: var(--sidebar-hover-text-color);
        margin-left: 10px;
        margin-right: 10px;
    }
    #DocumentationList .document-list-item--opened:hover, #documentList .document-list-item--opened:hover {
        font-weight: 600 !important;
        background-color: var(--sidebar-focused-background-color);
        border-width: var(--sidebar-focused-left-border-width);
        border-left-color: var(--sidebar-focused-left-border-color);
        font-size: 14px !important;
        color: var(--sidebar-focused-text-color) !important;
        margin-left: 10px !important;
        margin-right: 10px !important;
        border-radius: 7px;
        filter: brightness(1);
    }
    #DocumentationList .document-list-item, #documentList .document-list-item {
        font-weight: 500;
        border-left-width: var(--sidebar-focused-left-border-width)!important;
        font-size: 14px;
        height: 14px;
        margin-top: 0px;
        margin-bottom: 0px;
        padding-top: 5px;
        padding-bottom: 5px;
    }
    #document-sidebar__hidden-link__container {
        padding-top: 5px;
        padding-left: 5px;
        padding-right: 0px;
        background-color: var(--sidebar-top-background-color);
        border-right-style: solid;
        border-right-width: var(--bars-border-width);
        border-right-color: var(--bars-border-color);
    }
    #document-sidebar__bottom-buttons .document-sidebar__bottom-buttons__button {
        filter: var(--icons-filter);
    }
    #document-sidebar__bottom-buttons .document-sidebar__bottom-buttons__button:hover {
        filter: var(--accent-color-filter);
    }
    .document__options-menu__item-graph img {
        filter: var(--icons-filter);
    }
    #document-hover-preview {
        background-color: var(--body-background-color);
        border: var(--popup-border-width) solid var(--popup-border-color);
        border-radius: var(--popup-border-radius);
        color: var(--popup-text-color);
        padding-top: 17px;
        padding-bottom: 0px;
        margin-left: 15px;
        padding-left: 15px;
        padding-right: 9px;
        box-shadow: none;
    }
    .document-link__right-click-menu {
        background-color: var(--popup-background-color);
        border: var(--popup-border-width) solid var(--popup-border-color);
        border-radius: var(--popup-border-radius);
        color: var(--popup-text-color);
    }
    .document-link__right-click-menu .item:hover {
        background-color: var(--popup-hover-background-color);
        border-radius: 3px;
        color: var(--popup-hover-text-color);
    }
    .right-click-menu {
        box-shadow: none;
    }
    .ui.dropdown .menu {
        background: var(--popup-background-color);
        box-shadow: none;
    }
    .ui.header, .ui.header .sub.header {
        color: var(--popup-text-color);
    }
    /*Tutorial menu*/
    #DocumentationList #documentation-list__section__large-title {
        background-color: #3B464B;
    }
    #DocumentationList #documentation-list__section {
        border-color: cyan;
    }
    .navigation-bar  {
        background-color: var(--sidebar-background-color);
        border-bottom-style: solid;
        border-bottom-color: var(--bars-border-color);
        border-bottom-width: var(--bars-border-width); 
    }
    .navigation-bar i.icon  {
        filter: var(--icons-filter) !important; 
    }
    .navigation-bar i.icon:hover  {
        filter: var(--accent-color-filter) !important; 
    }
    #UpdateIndicator {
        border: 0px;
        font-size: 13px;
        color: var(--focused-accent-color);
        font-weight: 600;
    }
    ```
  - ## 5 Highlight colours ##Todo
    ```css
    /*RED*/
    /*general*/
    .highlight-color--red {
        background: linear-gradient(
            0deg, 
            var(--highlight-red) 0%,
            var(--highlight-red) 100%);
        border-radius: 20px;                 
        padding-left: 3px;
        padding-right: 3px;
    }
    .rich-text-editor__selected-text-menu .highlight-color--red {
        background: linear-gradient(
            0deg, 
            var(--highlight-red) 0%,
            var(--highlight-red) 100%);
        margin-left: -1px;
        margin-right: -1px;
    }
    /*container*/
    #hierarchy-editor .rem-container--default .highlight-color--red {
        background: linear-gradient(
            0deg, 
            var(--highlight-red) 0%,
            var(--highlight-red) 100%);
        border-radius: 20px;
        color: var(--focused-text-color);
    }
    #hierarchy-editor .rem-container--focused .highlight-color--red {
        background: linear-gradient(
            0deg, 
            var(--highlight-red-focused) 0%,
            var(--highlight-red-focused) 100%);
        border-radius: 20px;
        color: var(--focused-text-color);
    }
    #hierarchy-editor .TreeNode .rem-container--default .highlight-color--red {
        background: linear-gradient(
            0deg, 
            var(--highlight-red) 0%,
            var(--highlight-red) 100%);
        border-radius: 20px;
        margin-left: 11px!important;
        padding-left: 15px!important;
    }
    #hierarchy-editor .TreeNode .rem-container--focused .highlight-color--red {
        background: linear-gradient(
            0deg, 
            var(--highlight-red-focused) 0%,
            var(--highlight-red-focused) 100%);
        border-radius: 20px;
        margin-left: 11px!important;
        padding-left: 15px!important;
        color: var(--focused-text-color);
    }
    /*text*/
    #hierarchy-editor .rem-text .highlight-color--red {
        background: linear-gradient(
            0deg, 
            var(--highlight-red) 0%,
            var(--highlight-red) 100%);
        border-radius: 20px;
        margin-left: -3px!important;
        margin-right: -3px!important;
        padding-left: 3px!important;
        padding-right: 3px!important;
    }
    #hierarchy-editor .TreeNode .rem-text .highlight-color--red {
        background: linear-gradient(
            0deg, 
            var(--highlight-red) 0%,
            var(--highlight-red) 100%);
        border-radius: 20px;
        margin-left: -3px!important;
        margin-right: -3px!important;
        padding-left: 3px!important;
        padding-right: 3px!important;
    }
    /*--- highlight container tag ---*/
    #hierarchy-editor .rem .hierarchy-editor__tag-bar .highlight-color--red {
        background: linear-gradient(
            0deg, 
            var(--highlight-red) 0%,
            var(--highlight-red) 100%);
        border-radius: 20px;
        padding-left: 5px!important;
    }
    /*--- highlight text tag ---*/
    #hierarchy-editor .rem .hierarchy-editor__tag-bar .RichTextViewer .highlight-color--red {
        background: linear-gradient(
            0deg, 
            var(--highlight-red) 0%,
            var(--highlight-red) 100%);
        border-radius: 20px;
        margin-left: 1px!important;
        margin-right: -3px!important;
        padding-left: 3px!important;
        padding-right: 3px!important;   
    }
    /*---------- ORANGE ----------*/
    /*--- general ---*/
    .highlight-color--orange {
        background: linear-gradient(
            0deg, 
            var(--highlight-orange) 0%,
            var(--highlight-orange) 100%);
        border-radius: 20px;                 
        padding-left: 3px;
        padding-right: 3px;
    }
    .rich-text-editor__selected-text-menu  .highlight-color--orange {
        background: linear-gradient(
            0deg, 
            var(--highlight-orange) 0%,
            var(--highlight-orange) 100%);
        margin-left: -1px;
        margin-right: -1px;
    }
    /*--- container ---*/
    #hierarchy-editor .rem-container--default .highlight-color--orange {
        background: linear-gradient(
            0deg, 
            var(--highlight-orange) 0%,
            var(--highlight-orange) 30%);
        border-radius: 20px;
        color: var(--focused-text-color);
    }
    #hierarchy-editor .rem-container--focused .highlight-color--orange {
        background: linear-gradient(
            0deg, 
            var(--highlight-orange-focused) 0%,
            var(--highlight-orange-focused) 100%);
        border-radius: 20px;
        color: var(--focused-text-color);
    }
    #hierarchy-editor .TreeNode .rem-container--default .highlight-color--orange {
        background: linear-gradient(
            0deg, 
            var(--highlight-orange) 0%,
            var(--highlight-orange) 100%);
        border-radius: 20px;
        margin-left: 11px!important;
        padding-left: 15px!important;
    }
    #hierarchy-editor .TreeNode .rem-container--focused .highlight-color--orange {
        background: linear-gradient(
            0deg, 
            var(--highlight-orange-focused) 0%,
            var(--highlight-orange-focused) 100%);
        border-radius: 20px;
        margin-left: 11px!important;
        padding-left: 15px!important;
        color: var(--focused-text-color);
    }
    /*--- text ---*/
    #hierarchy-editor .rem-text .highlight-color--orange {
        background: linear-gradient(
            0deg, 
            var(--highlight-orange) 0%,
            var(--highlight-orange) 100%);
        border-radius: 20px;
        margin-left: -3px!important;
        margin-right: -3px!important;
        padding-left: 3px!important;
        padding-right: 3px!important;
    }
    #hierarchy-editor .TreeNode .rem-text .highlight-color--orange {
        background: linear-gradient(
            0deg, 
            var(--highlight-orange) 0%,
            var(--highlight-orange) 100%);
        border-radius: 20px;
        margin-left: -3px!important;
        margin-right: -3px!important;
        padding-left: 3px!important;
        padding-right: 3px!important;
    }
    /*--- highlight container tag ---*/
    #hierarchy-editor .rem .hierarchy-editor__tag-bar .highlight-color--orange {
        background: linear-gradient(
            0deg, 
            var(--highlight-orange) 0%,
            var(--highlight-orange) 100%);
        border-radius: 20px;
        padding-left: 5px!important;
    }
    /*--- highlight text tag ---*/
    #hierarchy-editor .rem .hierarchy-editor__tag-bar .RichTextViewer .highlight-color--orange {
        background: linear-gradient(
            0deg, 
            var(--highlight-orange) 0%,
            var(--highlight-orange) 100%);
        border-radius: 20px;
        margin-left: 1px!important;
        margin-right: -3px!important;
        padding-left: 3px!important;
        padding-right: 3px!important;   
    }
    /*---------- YELLOW ----------*/
    /*--- general ---*/
    .highlight-color--yellow {
        background: linear-gradient(
            0deg, 
            var(--highlight-yellow) 0%,
            var(--highlight-yellow) 100%);
        border-radius: 20px;                 
        padding-left: 3px;
        padding-right: 3px;
    }
    .rich-text-editor__selected-text-menu .highlight-color--yellow {
        background: linear-gradient(
            0deg, 
            var(--highlight-yellow) 0%,
            var(--highlight-yellow) 100%);
        margin-left: -1px;
        margin-right: -1px;
    }
    /*--- container ---*/
    #hierarchy-editor .rem-container--default .highlight-color--yellow {
        background: linear-gradient(
            0deg, 
            var(--highlight-yellow) 0%,
            var(--highlight-yellow) 100%); 
        border-radius: 20px;
        color: var(--focused-text-color);
    }
    #hierarchy-editor .rem-container--focused .highlight-color--yellow {
        background: linear-gradient(
            0deg, 
            var(--highlight-yellow-focused) 0%,
            var(--highlight-yellow-focused) 100%);
        border-radius: 20px;
        color: var(--focused-text-color);
    }
    #hierarchy-editor .TreeNode .rem-container--default .highlight-color--yellow {
        background: linear-gradient(
            0deg, 
            var(--highlight-yellow) 0%,
            var(--highlight-yellow) 100%);
        border-radius: 20px;
        margin-left: 11px!important;
        padding-left: 15px!important;
    }
    #hierarchy-editor .TreeNode .rem-container--focused .highlight-color--yellow {
        background: linear-gradient(
            0deg, 
            var(--highlight-yellow-focused) 0%,
            var(--highlight-yellow-focused) 100%);
        border-radius: 20px;
        margin-left: 11px!important;
        padding-left: 15px!important;
        color: var(--focused-text-color);
    }
    /*--- text ---*/
    #hierarchy-editor .rem-text .highlight-color--yellow {
        background: linear-gradient(
            0deg, 
            var(--highlight-yellow) 0%,
            var(--highlight-yellow) 30%);
        border-radius: 20px;
        margin-left: -3px!important;
        margin-right: -3px!important;
        padding-left: 3px!important;
        padding-right: 3px!important;
    }
    #hierarchy-editor .TreeNode .rem-text .highlight-color--yellow {
        background: linear-gradient(
            0deg, 
            var(--highlight-yellow) 0%,
            var(--highlight-yellow) 30%);
        border-radius: 20px;
        margin-left: -3px!important;
        margin-right: -3px!important;
        padding-left: 3px!important;
        padding-right: 3px!important;
    }
    /*--- highlight container tag ---*/
    #hierarchy-editor .rem .hierarchy-editor__tag-bar .highlight-color--yellow {
        background: linear-gradient(
            0deg, 
            var(--highlight-yellow) 0%,
            var(--highlight-yellow) 100%);
        border-radius: 20px;
        padding-left: 5px!important;
    }
    /*--- highlight text tag ---*/
    #hierarchy-editor .rem .hierarchy-editor__tag-bar .RichTextViewer .highlight-color--yellow {
        background: linear-gradient(
            0deg, 
            var(--highlight-yellow) 0%,
            var(--highlight-yellow) 100%);
        border-radius: 20px;
        margin-left: 1px!important;
        margin-right: -3px!important;
        padding-left: 3px!important;
        padding-right: 3px!important;   
    }
    /*---------- GREEN ----------*/
    /*--- general ---*/
    .highlight-color--green {
        background: linear-gradient(
            0deg, 
            var(--highlight-green) 0%,
            var(--highlight-green) 100%);
        border-radius: 20px;                 
        padding-left: 3px;
        padding-right: 3px;
    }
    .rich-text-editor__selected-text-menu  .highlight-color--green {
        background: linear-gradient(
            0deg, 
            var(--highlight-green) 0%,
            var(--highlight-green) 100%);
        margin-left: -1px;
        margin-right: -1px;
    }
    /*--- container ---*/
    #hierarchy-editor .rem-container--default .highlight-color--green {
        background: linear-gradient(
            0deg, 
            var(--highlight-green) 0%,
            var(--highlight-green) 30%);
        border-radius: 20px;
        color: var(--focused-text-color);
    }
    #hierarchy-editor .rem-container--focused .highlight-color--green {
        background: linear-gradient(
            0deg, 
            var(--highlight-green-focused) 0%,
            var(--highlight-green-focused) 100%);
        border-radius: 20px;
        color: var(--focused-text-color);
    }
    #hierarchy-editor .TreeNode .rem-container--default .highlight-color--green {
        background: linear-gradient(
            0deg, 
            var(--highlight-green) 0%,
            var(--highlight-green) 100%);
        border-radius: 20px;
        margin-left: 11px!important;
        padding-left: 15px!important;
    }
    #hierarchy-editor .TreeNode .rem-container--focused .highlight-color--green {
        background: linear-gradient(
            0deg, 
            var(--highlight-green-focused) 0%,
            var(--highlight-green-focused) 100%);
        border-radius: 20px;
        margin-left: 11px!important;
        padding-left: 15px!important;
        color: var(--focused-text-color);
    }
    /*--- text ---*/
    #hierarchy-editor .rem-text .highlight-color--green {
        background: linear-gradient(
            0deg, 
            var(--highlight-green) 0%,
            var(--highlight-green) 100%);
        border-radius: 20px;
        margin-left: -3px!important;
        margin-right: -3px!important;
        padding-left: 3px!important;
        padding-right: 3px!important;
    }
    #hierarchy-editor .TreeNode .rem-text .highlight-color--green {
        background: linear-gradient(
            0deg, 
            var(--highlight-green) 0%,
            var(--highlight-green) 100%);
        border-radius: 20px;
        margin-left: -3px!important;
        margin-right: -3px!important;
        padding-left: 3px!important;
        padding-right: 3px!important;
    }
    /*--- highlight container tag ---*/
    #hierarchy-editor .rem .hierarchy-editor__tag-bar .highlight-color--green {
        background: linear-gradient(
            0deg, 
            var(--highlight-green) 0%,
            var(--highlight-green) 100%);
        border-radius: 20px;
        padding-left: 5px!important;
    }
    /*--- highlight text tag ---*/
    #hierarchy-editor .rem .hierarchy-editor__tag-bar .RichTextViewer .highlight-color--green {
        background: linear-gradient(
            0deg, 
            var(--highlight-green) 0%,
            var(--highlight-green) 100%);
        border-radius: 20px;
        margin-left: 1px!important;
        margin-right: -3px!important;
        padding-left: 3px!important;
        padding-right: 3px!important;   
    }
    /*---------- BLUE ----------*/
    /*--- general ---*/
    .highlight-color--blue {
        background: linear-gradient(
            0deg, 
            var(--highlight-blue) 0%,
            var(--highlight-blue) 100%);
        border-radius: 20px;                 
        padding-left: 3px;
        padding-right: 3px;
    }
    .rich-text-editor__selected-text-menu  .highlight-color--blue {
        background: linear-gradient(
            0deg, 
            var(--highlight-blue) 0%,
            var(--highlight-blue) 100%);
        margin-left: -1px;
        margin-right: -1px;
    }
    /*--- container ---*/
    #hierarchy-editor .rem-container--default .highlight-color--blue {
        background: linear-gradient(
            0deg, 
            var(--highlight-blue) 0%,
            var(--highlight-blue) 100%);
        border-radius: 20px;
        color: var(--focused-text-color);                
    }
    #hierarchy-editor .rem-container--focused .highlight-color--blue {
        background: linear-gradient(
            0deg, 
            var(--highlight-blue-focused) 0%,
            var(--highlight-blue-focused) 100%);
        border-radius: 20px;
        color: var(--focused-text-color);
    }
    #hierarchy-editor .TreeNode .rem-container--default .highlight-color--blue {
        background: linear-gradient(
            0deg, 
            var(--highlight-blue) 0%,
            var(--highlight-blue) 100%);
        border-radius: 20px;
        margin-left: 11px!important;
        padding-left: 15px!important;
    }
    #hierarchy-editor .TreeNode .rem-container--focused .highlight-color--blue {
        background: linear-gradient(
            0deg, 
            var(--highlight-blue-focused) 0%,
            var(--highlight-blue-focused) 100%);
        border-radius: 20px;
        margin-left: 11px!important;
        padding-left: 15px!important;
        color: var(--focused-text-color);
    }
    /*--- text ---*/
    #hierarchy-editor .rem-text .highlight-color--blue {
        background: linear-gradient(
            0deg, 
            var(--highlight-blue) 0%,
            var(--highlight-blue) 100%);
        border-radius: 20px;
        margin-left: -3px!important;
        margin-right: -3px!important;
        padding-left: 3px!important;
        padding-right: 3px!important;
    }
    #hierarchy-editor .TreeNode .rem-text .highlight-color--blue {
        background: linear-gradient(
            0deg, 
            var(--highlight-blue) 0%,
            var(--highlight-blue) 100%);
        border-radius: 20px;
        margin-left: -3px!important;
        margin-right: -3px!important;
        padding-left: 3px!important;
        padding-right: 3px!important;
    }
    /*--- highlight container tag ---*/
    #hierarchy-editor .rem .hierarchy-editor__tag-bar .highlight-color--blue {
        background: linear-gradient(
            0deg, 
            var(--highlight-blue) 0%,
            var(--highlight-blue) 100%);
        border-radius: 20px;
        padding-left: 5px!important;
    }
    /*--- highlight text tag ---*/
    #hierarchy-editor .rem .hierarchy-editor__tag-bar .RichTextViewer .highlight-color--blue {
        background: linear-gradient(
            0deg, 
            var(--highlight-blue) 0%,
            var(--highlight-blue) 100%);
        border-radius: 20px;
        margin-left: 1px!important;
        margin-right: -3px!important;
        padding-left: 3px!important;
        padding-right: 3px!important;   
    }
    /*---------- PURPLE ----------*/
    /*--- general ---*/
    .highlight-color--purple {
        background: linear-gradient(
            0deg, 
            var(--highlight-purple) 0%,
            var(--highlight-purple) 100%);
        border-radius: 20px;                 
        padding-left: 3px;
        padding-right: 3px;
    }
    .rich-text-editor__selected-text-menu  .highlight-color--purple {
        background: linear-gradient(
            0deg, 
            var(--highlight-purple) 0%,
            var(--highlight-purple) 100%);
        margin-left: -1px;
        margin-right: -1px;
    }
    /*--- container ---*/
    #hierarchy-editor .rem-container--default .highlight-color--purple {
        background: linear-gradient(
            0deg, 
            var(--highlight-purple) 0%,
            var(--highlight-purple) 30%);
        border-radius: 20px;
        color: var(--focused-text-color);    
    }
    #hierarchy-editor .rem-container--focused .highlight-color--purple {
        background: linear-gradient(
            0deg, 
            var(--highlight-purple-focused) 0%,
            var(--highlight-purple-focused) 100%);
        border-radius: 20px;
        color: var(--focused-text-color);
    }
    #hierarchy-editor .TreeNode .rem-container--default .highlight-color--purple {
        background: linear-gradient(
            0deg, 
            var(--highlight-purple) 0%,
            var(--highlight-purple) 100%);
        border-radius: 20px;
        margin-left: 11px!important;
        padding-left: 15px!important;
    }
    #hierarchy-editor .TreeNode .rem-container--focused .highlight-color--purple {
        background: linear-gradient(
            0deg, 
            var(--highlight-purple-focused) 0%,
            var(--highlight-purple-focused) 100%);
        border-radius: 20px;
        margin-left: 11px!important;
        padding-left: 15px!important;
        color: var(--focused-text-color);
    }
    /*--- text ---*/
    #hierarchy-editor .rem-text .highlight-color--purple {
        background: linear-gradient(
            0deg, 
            var(--highlight-purple) 0%,
            var(--highlight-purple) 100%);
        border-radius: 20px;                 
        margin-left: -3px!important;
        margin-right: -3px!important;
        padding-left: 3px!important;
        padding-right: 3px!important;
    }
    #hierarchy-editor .TreeNode .rem-text .highlight-color--purple {
        background: linear-gradient(
            0deg, 
            var(--highlight-purple) 0%,
            var(--highlight-purple) 100%);
        border-radius: 20px;                 
        margin-left: -3px!important;
        margin-right: -3px!important;
        padding-left: 3px!important;
        padding-right: 3px!important;
    }
    /*--- highlight container tag ---*/
    #hierarchy-editor .rem .hierarchy-editor__tag-bar .highlight-color--purple {
        background: linear-gradient(
            0deg, 
            var(--highlight-purple) 0%,
            var(--highlight-purple) 100%);
        border-radius: 20px;
        padding-left: 5px!important;    
    }
    /*--- highlight text tag ---*/
    #hierarchy-editor .rem .hierarchy-editor__tag-bar .RichTextViewer .highlight-color--purple {
        background: linear-gradient(
            0deg, 
            var(--highlight-purple) 0%,
            var(--highlight-purple) 100%);
        border-radius: 20px;
        margin-left: 1px!important;
        margin-right: -3px!important;
        padding-left: 3px!important;
        padding-right: 3px!important;   
    }
    .rem-header--1 {
        background-color: transparent;
        border-radius: 0px;
    }
    ```
  - ## 6 Search highlight boxes ##Todo
    ```css
    .embeddedSearch:focus-within {
        border-top-left-radius: var(--border-radius);
        border-top-right-radius: var(--border-radius);
        border-bottom-right-radius: var(--border-radius);
        border-bottom-left-radius: var(--border-radius);
        border: 1px solid var(--accent-color);
        border-top-color: var(--accent-color);
        border-top-style: solid;
        border-top-width: 1px;
        border-right-color: var(--accent-color);
        border-right-style: solid;
        border-right-width: 1px;
        border-bottom-color: var(--accent-color);
        border-bottom-style: solid;
        border-bottom-width: 1px;
        border-left-color: var(--accent-color);
        border-left-style: solid;
        border-left-width: 1px;
        padding-top: 5px;
        padding-right: 5px;
        padding-bottom: 6px;
        padding-left: 10px;
        margin-bottom: 5px;
        margin-left: 10px;
        margin-right: 10px;
        margin-top: 0px;
        background-color: var(--embeddedsearch-background-color);
    }
    #hierarchy-editor-toolbar-container #hierarchy-editor__add-to-portal:focus-within .rich-text-editor {
        border: var(--popup-border-width) solid var(--accent-color);
        border-radius: var(--popup-border-radius);
        background-color: var(--search-box-background-color);
        color: var(--popup-text-color);
        padding-top: 3px;
        margin-right: -7px;
    }
    .hierarchy-editor__hidden-children .hierarchy-editor__hidden-children__search:focus-within .rich-text-editor {
        border-color: var(--accent-color);
    }
    ```
  - ## 7 Search keyword highlight ##Todo
    ```css
    .searchKeywordHighlight {
        background: var(--searchkeywordhighlight-color)!important;
        color: var(--searchkeywordhighlight-text-color)!important;
        border-radius: 0px!important;
        margin-left: 0px!important;
        margin-right: 0px!important;
        padding-left: 0px!important;
        padding-right: 0px!important;
        position: relative;
        z-index: 0!important;
    }
    #hierarchy-editor .rem-container--default:hover  .searchKeywordHighlight  {
        background: var(--searchkeywordhighlight-color)!important;
        color: var(--searchkeywordhighlight-text-color)!important;
        border-radius: 0px!important;
        margin-left: 0px!important;
        margin-right: 0px!important;
        padding-left: 0px!important;
        padding-right: 0px!important;
        position: relative;
        z-index: 0!important;
    }
    #hierarchy-editor .rem-container--focused .searchKeywordHighlight  {
        background: var(--searchkeywordhighlight-color)!important;
        color: var(--searchkeywordhighlight-text-color)!important;
        border-radius: 0px!important;
        margin-left: 0px!important;
        margin-right: 0px!important;
        padding-left: 0px!important;
        padding-right: 0px!important;
        position: relative;
        z-index: 0!important;
    }
    #hierarchy-editor .quote .searchKeywordHighlight {
        background: var(--searchkeywordhighlight-color)!important;
        border-radius: 0px!important;
        margin-left: 2px!important;/*modified 28 Jun 2021*/
        margin-right: -2px!important;
        padding-left: 0px!important;
        padding-right: 0px!important;
    }
    ```
  - ## 8 Tags ##Todo
    ```css
    .hierarchy-editor__tag-bar__tag {
        border-radius: 15px;
        padding-top: 0px;
        padding-bottom: 0px;
        padding-left: 10px;
        padding-right: 5px;
        color: var(--body-text-color);
        font-size: 13px;
        background-color: transparent;
        white-space: pre;
        font-weight: 500;
        margin-top: 0px;
        margin-bottom: 0px;
        margin-right: 5px;
    }
    .hierarchy-editor__tag-bar {
        top: 1px;
        bottom: 0px;
    }
    .hierarchy-editor__tag-bar__tag__delete:hover {
        color: var(--accent-color);
        background-color: transparent;
    }
    #hierarchy-editor .rem-container--focused .hierarchy-editor__tag-bar__tag .gray {
        color: var(--focused-text-color)!important;
    }
    #hierarchy-editor .rem-container--default .hierarchy-editor__tag-bar__tag .gray {
        color: var(--body-text-color);
    }
    #hierarchy-editor .rem-container--default .hierarchy-editor__tag-bar__tag .join-arrow {
        color:  var(--body-text-color);
    }
    #hierarchy-editor .rem-container--focused .hierarchy-editor__tag-bar__tag .join-arrow {
        color: var(--focused-text-color);
    }
    .hierarchy-editor__tag-bar .hierarchy-editor__tag-bar__power-up-tag {
        color: var(--icons-color);
    }  
    ```
  - ## 9 Popups ##Todo
    ```css
    .ui.popup {
        background-color: var(--popup-background-color) !important;
        border: var(--popup-border-width) solid var(--popup-border-color) !important;
        border-radius: var(--popup-border-radius) !important;
        color: var(--popup-text-color) !important;
        margin-left: 0px!important;
        margin-right: 0px!important;
        padding-top: 6px!important;
        padding-bottom: 6px!important;
    }
    .rem-reference__popup {
        width: 275px;
        font-size: 14px;
        background-color: var(--popup-background-color);
        border: var(--popup-border-width) solid var(--popup-border-color);
        border-radius: var(--popup-border-radius);
        box-shadow: none;
        color: var(--popup-text-color)!important;
    }
    .rem-reference__popup__item {
        color: var(--popup-text-color)!important;
    }
    .rem-reference__popup__item .icon:not(i.icon) {
        filter: var(--icons-filter);
    }
    .rem-reference__popup__item:hover {
        background-color: var(--popup-hover-background-color)!important;
        color: var(--popup-hover-text-color);
    }
    .rem-reference__popup .rem-reference__popup__preview {
        font-size: 16px;
        border-color: var(--popup-border-color);
        border-bottom: solid var(--popup-border-color);
        border-width: thin;
        margin-bottom: 5px;
        padding: 8px 11px;
        font-weight: 700;
        color: var(--popup-text-color);
    }
    .hierarchy-editor__hidden-children {
        background-color: var(--popup-background-color);
        box-shadow: none;
        border-radius: var(--popup-border-radius);
        border-style: solid;
        border-color: var(--popup-border-color);
        border-width: var(--popup-border-width);
        color: var(--popup-text-color);
    }
    .hierarchy-editor__hidden-children .hierarchy-editor__hidden-children__search .rich-text-editor {
        background-color: var(--search-box-background-color);
        border-radius: var(--popup-border-radius);
        border-style: solid;
        border-color: var(--popup-border-color);
        border-width: var(--popup-border-width)
    }
    .hierarchy-editor__hidden-children .selectedResult {
        background-color: var(--popup-hover-background-color);
        border-radius: var(--popup-border-radius) !important;
    }
    .hierarchy-editor__hidden-children #search-results__result:hover {
        background-color: var(--popup-hover-background-color);
    }
    .hierarchy-editor__hidden-children .rem-bullet__queue {
        background-color: var(--bullet-color);
    }
    .rich-text-editor__selected-text-menu {
        background-color: transparent ;
        border-style:none;
        box-shadow: none;
    }
    .rich-text-editor__selected-text-menu .rich-text-editor__selected-text-menu__doc-options {
        background-color: var(--popup-background-color);
        border-radius: var(--popup-border-radius);
        border-style: solid;
        border-color: var(--popup-border-color);
        border-width: var(--popup-border-width);
    }
    .rich-text-editor__selected-text-menu .selected-text-menu__button:hover {
        background-color: var(--popup-hover-background-color);
    }
    .rich-text-editor__selected-text-menu .selected-text-menu__button:hover .icon {
        color: var(--accent-color);
    }
    .rich-text-editor__selected-text-menu .selected-text-menu__button:hover .flashcards-icon {
        filter: var(--accent-color-filter);
    }
    .rich-text-editor__selected-text-menu .rich-text-editor__selected-text-menu__divider {
        border-color: var(--popup-border-color);
    }
    .rich-text-editor__selected-text-menu .selected-text-menu__button--color {
        border-color: var(--popup-border-color);
        border-width: var(--popup-border-width);
        border-radius: var(--popup-border-radius);
    }
    .rich-text-editor__selected-text-menu .selected-text-menu__button--color:hover {
        border-color: var(--accent-color);
    }
    .rich-text-editor__selected-text-menu .rich-text-editor__selected-text-menu__search {
        border-style: none;
    }
    .search-results {
        background-color: var(--popup-background-color) !important;
        border-color: var(--popup-border-color) !important;
        border-width: var(--popup-border-width) !important;
        border-radius: var(--popup-border-radius) !important;
    }
    .search-results #search-results__list {
        background-color: var(--popup-background-color) !important;
        color: var(--popup-text-color);
    }
    .search-results #search-results__list .selectedResult {
        background-color: var(--popup-hover-background-color) !important;
    }
    .search-results #search-results__list #search-results__result:hover {
        background-color: var(--popup-hover-background-color)
        !important;
    }
    .search-result__rem-breadcrumbs {
        color: var(--popup-text-color) !important;
    }
    .gray {
        color: var(--popup-text-color) !important;
    }
    #search-results__list #quote {
        background-color: var(--popup-background-color) !important;
        border-color: var(--popup-border-color);
    }
    #quote {
        background-color: transparent;
        border-color: var(--accent-color);
        color: var(--accent-color);
    }
    .react-contextmenu--visible {
        background-color: var(--popup-background-color);
        box-shadow: none;
        border-style: solid;
        border-color: var(--popup-border-color);
        border-width: var(--popup-border-width);
        border-radius: var(--popup-border-radius);
    }
    .keycode {
        color: var(--popup-keycode-color)!important;
    }
    .rem-reference__popup .rem-reference__popup__item .keycode {
        color: var(--popup-keycode-color)!important;
    }
    .hierarchy-editor-toolbar__menu .hierarchy-editor-toolbar__menu__item .hierarchy-editor-toolbar__menu__keycode {
        color: var(--popup-keycode-color)!important;
    }
    .react-contextmenu--visible .hierarchy-editor__rem-menutoolbar-buttons .toolbar-button {
        border-color: var(--popup-border-color);
        border-width: var(--popup-border-width);
        border-radius: var(--popup-border-radius);
        color: var(--popup-text-color);
    }
    .react-contextmenu--visible .hierarchy-editor__rem-menutoolbar-buttons .toolbar-button:hover {
        border-color: var(--accent-color);
        border-width: var(--popup-border-width);
        border-radius: var(--popup-border-radius);
        color: var(--accent-color);
    }
    .react-contextmenu--visible #menu-divider {
        border: 1px solid var(--popup-border-color);
        margin: 5px 0;
    }
    .react-contextmenu--visible .hierarchy-editor__rem-menu {
        color: var(--popup-text-color);
    }
    .react-contextmenu--visible .hierarchy-editor__rem-menu:hover {
        background-color: var(--popup-hover-background-color);
    }
    #document .document__top-bar .document__options-menu .ui.right.pointing.dropdown>.menu {
        background-color: var(--popup-background-color);
        box-shadow: none;
        border-radius: 13px;
    }
    .ui.right.pointing.dropdown>.menu:after {
        background-color: var(--popup-background-color);
    }
    .ui.dropdown .menu>.item {
        color: var(--popup-text-color);
    }
    .ui.dropdown .menu>.item:hover {
        color: var(--popup-text-color);
        background-color: var(--popup-hover-background-color);
    }
    .ui.dropdown .menu .left.menu, .ui.dropdown>.left.menu .menu {
        background-color: var(--popup-background-color);
        color: var(--popup-text-color);
    }
    .ui.dropdown .menu>.item>img {
        filter: var(--icons-filter);
    }
    #hierarchy-editor .HierarchyEditorChildrenList {
        color: var(--body-text-color);
    }
    #hierarchy-editor .HierarchyEditorChildrenList:hover {
        color: var(--accent-color);
    }
    #hierarchy-editor .hierarchy-editor__children-list--focused {
        color: var(--accent-color)!important;
    }
    #hierarchy-editor .HierarchyEditorChildrenList .children-list-content {
        background-color: var(--popup-background-color);
        border-color: var(--popup-border-color);
        border-width: var(--popup-border-width);
        border-radius: var(--popup-border-radius);
        color: var(--popup-text-color);
        box-shadow: none;
    }
    #hierarchy-editor .HierarchyEditorChildrenList .children-list-content .childrenListItem:hover {
        background-color: var(--popup-hover-background-color);
        color: var(--popup-text-color);
    }
    #bordered-card, #Popup #PopupContent, .HierarchyEditorBodyview-as-cardTooltip {
        background-color: var(--popup-background-color);
        color: var(--popup-text-color);
        box-shadow: none;
    }
    .rem-reference a {
        color: var(--link-text-color)!important;
    }
    .react-datepicker {
        background-color: rgb(35, 37, 37);
        color: var(--accent-color);
        border: var(--popup-border-width) solid var(--popup-border-color);
        border-radius: var(--popup-border-radius);
    }
    .react-datepicker__header {
        border-bottom: var(--popup-border-width) solid var(--popup-border-color);
        border-top: none;
        background-color: rgb(35, 37, 37);
        border-radius: var(--popup-border-radius) !important;
        border-bottom-left-radius: 0px !important;
        border-bottom-right-radius: 0px !important;
    }
    .react-datepicker-time__header, .react-datepicker__current-month {
        color: var(--popup-text-color);
    }
    .react-datepicker__day, .react-datepicker__day-name, .react-datepicker__time-name {
        color: var(--popup-text-color);
    }
    .react-datepicker__today-button {
        border-radius: 0 0 var(--popup-border-radius) var(--popup-border-radius);
        border-top: var(--popup-border-width) solid var(--popup-border-color);
        background-color: rgb(35, 37, 37);
    }
    .react-datepicker__day:hover {
        background-color: var(--popup-hover-background-color);
        color: var(--popup-text-color);
    }
    .react-datepicker__day--selected {
        background-color: var(--accent-color);
        color: var(--focused-text-color);
    }
    .react-datepicker__day--selected:hover {
        background-color: var(--focused-accent-color);
        color: var(--focused-text-color);
    }
    .link-node__popup .link-node__popup__option .link-node__popup__link {
        color: var(--link-text-color);
    }
    .link-node__popup .link-node__popup__option .link-node__popup__shortcut {
        color: var(--popup-keycode-color);
    }
    #status-indicator {
        background-color: var(--popup-background-color);
        color: var(--popup-text-color);
        border-color: var(--popup-border-color);
    }
    /* added 05 Jun 2021 */
    #help-menu-popup .help-menu-item:hover {
        background-color: var(--popup-hover-background-color);
        color: var(--focused-accent-color);
    }
    /* added 11 Jun 2021 */
    .popup-menu {
        font-size: 14px;
        background-color: var(--popup-background-color)!important;
        border: var(--popup-border-width) solid var(--popup-border-color);
        box-shadow: none;
        border-radius: var(--popup-border-radius);
    }
    .popup-menu .popup-meue__item--static {
        border-bottom: var(--popup-border-width) solid var(--popup-border-color);
    }
    .date-picker__container {
        padding-top: 15px;
    }
    .ui.divider:not(.vertical):not(.horizontal) {
        border-top: 1px solid var(--popup-border-color);
        border-bottom: 1px solid var(--popup-border-color);
    }
    .popup-menu .popup-menu__item--small {
        color: var(--popup-text-color);
    }
    .popup-menu .popup-menu__item--small:hover {
        background-color: var(--popup-hover-background-color);
        color: var(--popup-hover-text-color);
    }
    .popup-menu .popup-menu__item--small .keycode {
        color: var(--popup-keycode-color)!important;
    }
    .popup-menu .popup-menu__item--small img {
        filter: var(--icons-filter);
    }
    /*Added 28 Jun 2021*/
    /*Search popup*/
    #SearchPopup #PinnedResults .SectionHeader {
        color: var(--accent-color);
    }
    #SearchPopup #PinnedResults .PinnedResult {
        color: var(--body-text-color);
    }
    #SearchPopup #PinnedResults .PinnedResult:hover {
        background-color: var(--popup-hover-background-color);
    }
    /*Quick Add*/
    .mobile-quick-add .mobile-quick-add__rich-text-editor, .mobile-quick-add textarea {
        background-color: var(--body-background-color);
        border: 2px solid var(--popup-border-color);
    }
    /*Tags right-click menu*/
    .react-contexify {
        background-color: var(--popup-background-color)!important;
        box-shadow: none;
        border: var(--popup-border-width) solid var(--popup-border-color);
        border-radius: var(--popup-border-radius);
    }
    .react-contexify__item__content {
        margin-left: 3px;
        margin-right: 3px;
        border-radius: var(--border-radius);
        color: var(--popup-text-color);
    }
    .react-contexify__item__content:hover {
        background-color: var(--popup-hover-background-color)!important;
    }
    /*------ end of added 28 Jun 2021 ------*/
    ```
  - ## 10 Checkbox ##Todo
    ```css
    .rem-checkbox {
        margin-right: 10px;
        margin-top: 3px;
        filter: invert(88%)
    }
    .rem-checkbox:checked {
        margin-right: 10px;
        margin-top: 3px;
        filter: var(--accent-color-filter);
    }
    .rem-todo--finished {
        color: var(--todo-finished-text-color)!important;
        filter: opacity(.85);
    }
    #code-node #code-node__change-language-dropdown .menu {
        background-color: var(--popup-background-color);
    }
    #code-node #code-node__change-language-dropdown .menu .item:first-child {
        color: grey;
    }
    .ui.upward.dropdown>.menu {
        box-shadow: none;
    }
    /* toggle */
    .ui.toggle.checkbox .box:before, .ui.toggle.checkbox label:before {
        background-color: var(--toggle-background-color);
    }
    .ui.toggle.checkbox .box:after, .ui.toggle.checkbox label:after {
        background-color: var(--toggle-color);
        top: .18rem!important;
        margin-left: 2px;
    }
    .ui.toggle.checkbox input:checked~.box:before, .ui.toggle.checkbox input:checked~label:before {
        background-color: var(--button-color)!important;
        border-style: solid;
        border-color: var(--button-color)!important;
    }
    .ui.toggle.checkbox input:checked~.box:after, .ui.toggle.checkbox input:checked~label:after {
        left: 2.1rem!important;
        box-shadow: none!important;
        background-color: var(--toggle-color)!important;
    }
    /* radio buttons*/
    .ui.checkbox .box:before, .ui.checkbox label:before {
        background-color: var(--toggle-background-color)!important;
        border: 1px solid var(--bars-border-color)!important;
    }
    .ui.checkbox:hover .box:before, .ui.checkbox:hover label:before {
        background-color: rgb(33, 35, 35)!important;
        border: 1px solid var(--bars-border-color)!important;
    }
    .ui.radio.checkbox input:checked~.box:before, .ui.radio.checkbox input:checked~label:before {
        background-color: var(--toggle-background-color)!important;
    }
    .ui.checkbox input:checked~.box:before, .ui.checkbox input:checked~label:before {
        border-color: var(--accent-color);
    }
    .ui.radio.checkbox input:checked~.box:after, .ui.radio.checkbox input:checked~label:after {
        background-color: var(--accent-color);
    }
    /* bigger check box ui */
    .ui.checkbox input:checked~.box:before, .ui.checkbox input:checked~label:before {
        background-color: rgb(93, 112, 151)!important;/*modified 11 June 2021*/
        border-color: rgb(54, 62, 78)!important;/*modified 11 June 2021*/
    }
    .ui.checkbox input:checked~.box:after, .ui.checkbox input:checked~label:after {
        color: rgb(54, 62, 78)!important;/*modified 11 June 2021*/
    }
    ```
  - ## 11 Code block ##Todo
    ```css
    #code-node {
        font-family: monaco,menlo,consolas,courier new;
        color: var(--code-block-text-color);
        background-color: var(--code-block-background-color);
        border-color: var(--code-block-border-color);
        border-width: var(--code-block-border-width);
        margin-left: -18px;
        padding-right: 86px !important;
        margin-top: -3px;
        margin-bottom: -3px;   
    }
    body #code-node {
        caret-color: red;
    }
    #code-node .token.url {
        background-color: transparent;
    }
    #hierarchy-editor .rem-container--focused > div #code-node {
        background-color: var(--code-block-focused-background-color);
        border-color: #62778D;
    }
    ```
  - ## 12 Flashcards ##Todo
    ```css
    .concept_rem_type, .question_rem_type, .descriptor_rem_type {
        font-weight: 700;
        color: var(--body-text-color)!important;
    }
    /* multi-line/list card tree lines*/
    #hierarchy-editor .TreeNode--list--in-card-content {
        border-color: var(--cloze-cards-lines);
        border-width: 2px;
        margin-bottom: 6px;
        padding-left: var(padding-left);
    }
    .cloze {
        background-color: transparent;
        border-bottom: 2px solid var(--cloze-cards-lines);
        padding-bottom: 0px;
        font-weight: 600;
        font-style: italic;
    }
    #homepage #content .DocumentationPageWrapper, #homepage #content .page, #main #content .DocumentationPageWrapper, #main #content .page {
        background: linear-gradient(to top, rgb(25,28,28), rgb(30,33,33))!important;
    }
    .dark-mode .black-out--enable {
        background: linear-gradient(to top, rgb(25,28,28), rgb(30,33,33))!important;
    }
    .QueueDesktop {
        background-color: var(--popup-background-color);
        box-shadow: none;
        border-style: solid;
        border-color: var(--popup-border-color)!important;
        border-width: var(--popup-border-width)!important;
        border-radius: var(--popup-border-radius)!important;
    }
    .Queue .queue__title {
        background-color: var(--popup-background-color);
    }
    .Queue .queue__title .queue__middle {
        color: var(--popup-text-color);
    }
    .Queue .queue__badge {
        background-color: var(--popup-background-color);
        color: var(--popup-text-color);
    }
    .Queue .queue__title .queue__sizeButton {
        background-color: var(--popup-background-color);
        color: var(--popup-text-color);
    }
    .Queue .queue__title #queue__top-right,
    .queue__streak-indicator {
        color: var(--popup-text-color);
    }
    .queue__streak-indicator i.icon.fire:before {
        color: var(--queue-indicator-icon-color);
    }
    .Queue #queue__progress-bar {
        background-color: var(--queue-fill-in-the-blank-color) !important;
        height: 8px;
    }
    .spacedRepetition .spaced-repetition__prompt .spaced-repetition__prompt__breadcrumbs {
        color: var(--popup-text-color);
    }
    .spacedRepetition .spacedRepetitionContent {
        background-color: var(--popup-background-color);
        color: var(--popup-text-color);
    }
    .spacedRepetition .spaced-repetition__prompt .indented-rem .rem-bullet__document {
        background-color: var(--popup-background-color);
    }
    .rem-bullet__queue {
        background-color: var(--bullet-color);
    }
    .spacedRepetition .fill-in-the-blank {
        color: var(--queue-fill-in-the-blank-color);
        border-width: thin;
    }
    /* modified 05 Jun 2021 */
    #QueueTypeAnswerBoxContainer #QueueTypeAnswerBox {
        background-color: rgb(36, 39, 39);
        border: var(--popup-border-width) solid var(--popup-border-color);
        border-radius: var(--popup-border-radius);
    }
    /* modified 05 Jun 2021 */
    #QueueTypeAnswerBoxContainer #QueueTypeAnswerBox:focus-within {
        background-color: rgb(36, 39, 39);
        border: var(--popup-border-width) solid var(--accent-color);
        border-radius: var(--popup-border-radius);
    }        
    #QueueTypeAnswerBoxContainer .ui.compact.button {
        color: var(--accent-color);
        margin-top: 9px;
        margin-bottom: 9px;
        padding-top: 0px;
        padding-bottom: 0px;
    }
    #QueueTypeAnswerBoxContainer .ui.compact.button:hover {
        color: var(--focused-accent-color);
        background-color: var(--popup-hover-background-color);
        margin-top: 9px;
        margin-bottom: 9px;
        padding-top: 0px;
        padding-bottom: 0px;
    }
    .spacedRepetition .spaced-repetition__bottom,
    .spacedRepetition .spaced-repetition__reveal {
        background-color: var(--popup-background-color);
        color: var(--accent-color);
        border-top-style: solid;
        border-top-width: 1px;
        border-top-color: var(--popup-border-color);
        border-bottom-left-radius: var(--popup-border-radius)!important;
        border-bottom-right-radius: var(--popup-border-radius)!important;
    }
    .spacedRepetition .spaced-repetition__bottom:hover,
    .spacedRepetition .spaced-repetition__reveal:hover {
        background-color: var(--popup-background-color);
        color: var(--focused-accent-color);
        border-top-style: solid;
        border-top-width: 1px;
        border-top-color: var(--popup-border-color);
        border-bottom-left-radius: var(--popup-border-radius)!important;
        border-bottom-right-radius: var(--popup-border-radius)!important;
    }
    .scroll-drag-component {
        background-color: transparent;
    }
    .spacedRepetition .spacedRepetitionAnswer {
        border-top: solid;
        border-width: var(--popup-border-width);
        border-color: var(--popup-text-color);
        padding-top: 10px;
        margin: 10px;
    }
    .spacedRepetitionAnswer .rem-container--default:hover .rem-text {
        color: var(--focused-text-color) !important;
    }
    .spacedRepetition .queue__response-button__image {
        filter: var(--icons-filter);
    }
    .queue__response-button:hover .queue__response-button__image {
        filter: var(--focused-accent-color-filter);
    }
    .queue__response-button {
        background-color: var(--popup-background-color);
        color: var(--popup-text-color);
        border-radius: 5px;
    }
    .queue__response-button:hover {
        background-color: var(--popup-hover-background-color);
        color: var(--focused-accent-color);
        border-radius: 5px;
    }
    .Queue .queue__no-items {
        color: var(--popup-text-color);
    }
    .Queue .queue__no-items a {
        color: var(--accent-color);
    }
    .milestone-bottom {
        background-color: var(--popup-background-color)!important;
        color: var(--accent-color)!important;
        border-radius: 5px;
    }
    /* modified 05 Jun 2021 */
    #milestone .badge {
        background-color: var(--popup-background-color);
        color: var(--queue-fill-in-the-blank-color);
        border-color: var(--popup-border-color);
    }
    #milestone #milestone__content {
        color: var(--popup-text-color);
    }
    #milestone #milestone__content b {
        color: var(--accent-color);
    }
    .queue-sub-folder-selector {
        background-color: var(--popup-background-color);
        color: var(--popup-text-color);
        border-bottom-left-radius: var(--popup-border-radius)!important;
        border-bottom-right-radius: var(--popup-border-radius)!important;
    }
    .queue-sub-folder-selector td, .queue-sub-folder-selector th {
        border-color: var(--popup-border-color);
        border-bottom: solid var(--popup-border-color);
        border-width: var(--popup-border-width);
        border-left-style: none;
        border-right-style: none;
    }
    .Queue .queue__title .queue__top-left .queue__back-button,
    .Queue .queue__title .queue__sizeButton img {
        filter: var(--icons-filter);
    }
    .queue-sub-folder-selector .queue-sub-folder-selector__search-box {
        border: var(--popup-border-width) solid var(--popup-border-color);
        border-radius: var(--popup-border-radius);
        background-color: var(--search-box-background-color);
    }
    .queue-sub-folder-selector__table__row:hover {
        background-color: var(--popup-hover-background-color)!important;
    }
    ```
  - ## 13 Sticky menu ##Todo
    ```css
    #hierarchy-editor #hierarchy-editor-list__sticky-top__container #hierarchy-editor-list__sticky-top .hierarchy-editor-list__sticky-top__rem-container .rem-text {
        background-color: var(--body-background-color);
        border-style: none;
        color: var(--body-text-color);
    }
    #hierarchy-editor .rem-container--sticky-document-title .rem-text {
        font-size: 18px;
        color: var(--body-background-color);
        border-style: none;
    }
    #hierarchy-editor #hierarchy-editor-list__sticky-top__container #hierarchy-editor-list__sticky-top {
        background-color: var(--body-background-color);
        color: var(--body-text-color);
        padding-left: 0px;
        margin-left: -13px;
    }
    .remInPortalBlue {
        border-style: none;
    }
    .remInPortal {
        border-style: none;
    }
    #hierarchy-editor .indented-hierarchy-editor-remPortal {
        border-style: none;
    }
    #hierarchy-editor #hierarchy-editor-list__sticky-top__container #hierarchy-editor-list__sticky-top #hierarchy-editor-list__sticky-top__bottom {
        border-bottom: 6px solid var(--popup-border-color);
        border-radius: 10px;
    }
    ```
  - ## 14 Sharing document ##Todo
    ```css
    .article-publish-confirmation {
        color: var(--body-text-color);
    }
    .ui.checkbox+label, .ui.checkbox label {
        color: var(--body-text-color);
    }
    ArticleViewer #ArticleViewerTop {
        color: var(--body-text-color);
    }
    #ExamplesPageContainer #ExamplesPageContent, #export-container #export, #HelpPage #HelpPageContent, #sign-up-page-container #sign-up-page, #StatsPage #StatsPageContent, .centered-page, .document--narrow {
        background-color: var(--body-background-color);
        color: var(--body-text-color);
    }
    ```
  - ## 15 Settings page ##Todo
    ```css
    /* settings page sidebar */
    .settings-page .settings-page__sidebar {
        min-width: 200px;
        max-height: 100%;
        display: flex;
        flex-direction: column;
        border-color: var(--popup-border-color);
        border-right: solid var(--popup-border-color);
        border-width: 1px;
        background-color: var(--sidebar-background-color);
    }
    .settings-page .settings-page__sidebar .settings-page__sidebar__link {
        border-color: var(--popup-border-color);
        color: var(--sidebar-text-color);
        font-size: 16px;
        padding: 10px 10px 10px 10px;
        border-bottom: solid var(--popup-border-color);
        border-width: 0;
        display: flex;
        align-items: center;
        margin: 5px;
        border-radius: var(--border-radius);
    }
    .settings-page .settings-page__sidebar .settings-page__sidebar__link:hover {
        background-color: var(--sidebar-hover-background-color);
        margin: 5px;
        border-radius: var(--border-radius);
    }
    .settings-page .settings-page__sidebar .settings-page__sidebar__link--active:hover {
        font-weight: 600;
        background-color: var(--sidebar-focused-background-color);
        color: var(--focused-text-color);
        border-left-style: none;
        margin: 5px;
        border-radius: var(--border-radius);
    }
    .settings-page .settings-page__sidebar .settings-page__sidebar__link--active {
        font-weight: 700;
        background-color: var(--sidebar-focused-background-color);
        color: var(--focused-text-color);
        border-left-style: none;
        margin: 5px;
        border-radius: var(--border-radius);
    }
    .settings-page .settings-page__sidebar .settings-page__sidebar__title {
        color: var(--sidebar-text-color);
        font-weight: 700;
        font-size: 24px;
        margin: 20px;
    }
    /* settings page body*/
    .settings-page .settings-page__content {
        background-color: var(--body-background-color);
    }
    .settings-page label {
        font-size: 14px!important;
        color: var(--body-text-color);
        font-weight: 600;
    }
    .settings-page .settings-page__content .settings-page__content-inner {
        padding: 30px;
        color: var(popup-text-color);
        background-color: var(--body-background-color);
    }
    .settings-page__option {
        margin-top: 10px;
        padding-bottom: 10px;
        display: flex;
        border-width: 1px;
        border-color: var(--popup-border-color);
    }
    .settings-page .settings-page__sub-header {
        border-width: 1px;
        border-color: var(--popup-border-color);
        color: var(--popup-text-color);
        font-size: 18px;
        margin: 40px 0 10px;
        padding-bottom: 5px;
        font-weight: 700;
    }
    .settings-page__option .settings-page__text .settings-page__text__subtext {
        color: var(--icons-color);
        margin-top: 5px;
        font-weight: 400;
    }
    .settings-page__option .settings-page__input .settings-page__input-box {
        border-style: none;
        background-color: var(--search-box-background-color);
        color: var(--focused-text-color);
    }
    .ui.dropdown .menu .selected.item, .ui.dropdown.selected {
        background: var(--popup-background-color);
        color: var(--popup-text-color);
    }
    /* custom schedulers */
    .ui.form .field>label {
        color: var(--accent-color);
    }
    .ui.input>input {
        border: 1px solid var(--popup-border-color);
        background: var(--body-background-color);
        box-shadow: none;
        color: var(--body-text-color);
    }
    .ui.input.focus>input, .ui.input>input:focus {
        border-color: var(--popup-border-color);
        background: var(--body-background-color);
        color: var(--body-text-color);
        box-shadow: none;
    }
    .ui.checkbox+label, .ui.checkbox label {
        color: var(--body-text-color);
        font-weight: 400;
    }
    .ui.checkbox+label, .ui.checkbox label:hover {
        color: var(--accent-color);
        font-weight: 400;
    }
    .spaced-repetition-scheduler-form .spaced-repetition-scheduler-form__section--examples {
        background-color: var(--body-background-color);
        border-color: var(--popup-border-color);
    }
    /* keyboard shortcuts*/
    #change-keyboard-shortcuts .change-keyboard-shortcut-list-item .change-keyboard-shortcut-list-item__code {
        color: var(--accent-color);
    }
    /* plugins */
    .ui.card, .ui.cards>.card {
        background: var(--body-background-color);
        border: 1px solid var(--popup-border-color);
        box-shadow: none;
        color: var(--popup-text-color);
    }
    a {
        color: var(--accent-color);
    }
    #PluginsConfiguration img {
        background: white;
        filter: invert(1) hue-rotate(160deg);
        border-top-left-radius: 5px;
        border-top-right-radius: 5px;    
    }
    .ui.card>.content>.header, .ui.cards>.card>.content>.header {
        color: var(--accent-color);
    }
    .ui.table {
        background: var(--body-background-color);
        border: 1px solid var(--popup-border-color);
        box-shadow: none;
        color: var(--accent-color);
        border-radius: 5px;
    }
    .ui.table thead th {
        background: var(--body-background-color);
        color: var(--body-text-color);
        border-bottom: 1px solid var(--popup-border-color);
        border-top-left-radius: 5px;
        border-top-right-radius: 5px; 
    }
    .PluginsConfiguration__table {
        overflow-y: overlay;
        height: 100%;
        width: 100%;
    }
    /* Account */
    .HomePageComponents button {
        background-color: var(--button-color);
        color: var(--body-text-color);
    }
    /* subscription */
    .HomePageComponents h1,
    .HomePageComponents h2,
    .HomePageComponents h3,
    .HomePageComponents h4,
    .HomePageComponents h5 {
        color: var(--accent-color);
    }
    .HomePageComponents p {
        color: var(--body-text-color);
    }
    .HomePageComponents .visual-link {
        color: var(--accent-color);
    }
    .HomePageComponents .settings__pricing-options .settings__pricing-option-item__current {
        background-color: var(--popup-background-color);
    }
    .HomePageComponents .from-container-blue-background {
        background-color: var(--popup-background-color);
    }
    .HomePageComponents .form-input {
        border: 2px solid var(--popup-border-color);
        color: var(--body-text-color);
        background-color: var(--sidebar-background-color);
    }
    .HomePageComponents .button--light {
        background-color: var(--popup-background-color);
        color: var(--accent-color);
        border: 1px solid var(--accent-color);
    }
    .popup-close-button {
        filter: var(--icons-filter);
    }
    .popup-close-button:hover {
        filter: var(--accent-color-filter) brightness(1.6);
    }
    #export-container #export #export__preview {
        border-style: solid;
        border-color: var(--popup-border-color);
        border-radius: 5px;
        overflow-x: overlay!important;
        overflow-y: overlay!important;
    }
    /* knowledgebase import */
    #ImportContainer .ImportTabs .menu .item {
        background-color: var(--popup-background-color);
        border-color: var(--popup-border-color);
        border-top-left-radius: 5px;
        border-top-right-radius: 5px;
        border-bottom-left-radius: 0px;
        border-bottom-right-radius: 0px;
        border-width: var(--popup-border-width);
        color: var(--icons-color);
        border-bottom-style: solid;
    }
    #ImportContainer .ImportTabs .menu .item:hover {
        color: var(--accent-color);
    }
    .ui.tabular.menu+.attached:not(.top).segment, .ui.tabular.menu+.attached:not(.top).segment+.attached:not(.top).segment {
        margin-top: -2px;
    }
    #ImportContainer .bottom {
        box-shadow: none;
    }
    .ui.segment {
        background: var(--popup-background-color);
        border: 1px solid var(--popup-border-color);
        padding: 9px;
        border-top-left-radius: 0px;
        border-top-right-radius: 0px;
    }
    .ui.tabular.menu .active.item {
        background-color: var(--popup-background-color)!important;
        color: var(--popup-text-color)!important;
        border-bottom-style: solid !important;
        border-bottom-width: 0px!important;
        border-bottom-left-radius: 0px!important;
        border-bottom-right-radius: 0px!important;
        font-weight: 500!important;
        margin-bottom: 0px;
    }
    /* dynalist */
    .ui.blue.button, .ui.blue.buttons .button {
        background-color: var(--button-color);
        color: var(--body-text-color);
        text-shadow: none;
        background-image: none;
        border-style: none;
    }
    /* paste */
    .ui.form textarea {
        background: var(--body-background-color);
        border: 1px solid var(--popup-border-color);
        color: var(--body-text-color);
    }
    .graph-viewer--dark {
        filter: invert(0%) hue-rotate(0deg);
    }
    ```
  - ## 16 Help Page ##Todo
    ```css
    #HelpPage a {
        color: var(--body-text-color);
    }
    .help-knowledge-base-search .rich-text-editor {
        background-color: var(--search-box-background-color);
        color: var(--search-box-text-color);
        padding: 7px;
        border-radius: 7px;
        font-size: 17px;
        border: 2px solid var(--popup-border-color);
    }
    .help-knowledge-base-search:focus-within .rich-text-editor {
        border: 2px solid var(--accent-color);
    }
    #HelpPage li {
        color: var(--accent-color);
        margin-top: 2px;
        margin-bottom: 2px;
        padding-top: 5px;
        padding-bottom: 5px;
        border-radius: 7px;
    }
    #HelpPage li:hover {
        background-color: var(--sidebar-hover-background-color);
        color: var(--focused-accent-color);
        padding-top: 5px;
        padding-bottom: 5px;
        border-radius: 7px;
    }
    #AboutSectionTitle {
        font-size: 24px;
        font-weight: 700;
        margin-bottom: 15px;
        margin-top: 20px;
        z-index: 1;
        padding-bottom: 5px;
        background-color: var(--body-background-color);
        border-bottom: thin solid;
        border-color: var(--popup-border-color);
    }
    #hierarchy-editor .rem-container--article-link:hover {
        background-color: var(--body-background-color);
    }
    /* interactive tour*/
    /* added 05 Jun 2021*/
    .onboarding-panel {
      background-color: var(--sidebar-background-color);
      border-left-style: solid;
      border-left-width: var(--bars-border-width);
      border-left-color: var(--bars-border-color);
    }
    .onboarding-panel .onboarding-panel__lesson-stub .onboarding-panel__lesson-stub__info .onboarding-panel__lesson-stub__title {
      color: var(--body-text-color);
    }
    .onboarding-panel .onboarding-panel__title-container .onboarding-panel__close-button {
      filter: var(--icons-filter);
    }
    .onboarding-panel .onboarding-panel__title-container .onboarding-panel__close-button:hover {
      filter: var(--accent-color-filter) grayscale(0.3) brightness(1.8);
    }
    .onboarding-panel .onboarding-panel__title-container .onboarding-panel__title {
      color: var(--body-text-color);
    }
    .onboarding-panel .onboarding-panel__subtitle {
        color: var(--accent-color);
    }
    .onboarding-panel .onboarding-panel__active-lesson .onboarding-panel__active-lesson__tasks .onboarding-panel__active-lesson__task {
        color: var(--body-text-color);
    }
    .onboarding-panel .onboarding-panel__lesson-stub .icon {
        color: var(--icons-color);
    }
    .onboarding-panel .onboarding-panel__active-lesson .onboarding-panel__active-lesson__tasks .onboarding-panel__active-lesson__task--active .onboarding-panel__active-lesson__task__main-text {
        color: var(--accent-color);
    }
    .ui.green.button, .ui.green.buttons .button {
        background-color: var(--button-color);
    }
    .onboarding-panel .onboarding-panel__image-container .onboarding-panel__image {
      filter: var(--accent-color-filter) contrast(1.3);
    }
    .onboarding-panel .onboarding-panel__active-lesson .onboarding-panel__active-lesson__tasks .onboarding-panel__active-lesson__task .onboarding-panel__active-lesson__task__subtext-read-more:hover {
        color: var(--accent-color);
    }
    ```
  - ## 17 Highlighted focused rem ##Todo
    - [ ] General in focus highlights
        ```css
        body {
            caret-color: var(--focused-text-color);
        }
        #hierarchy-editor .tree-node-container 
            > div:not(:first-child) .rem-container--focused  {
            background: none;
            background-image: none;
        }
        /*--------------- 1st Tree Lines ------------------ */
        #hierarchy-editor .TreeNode:hover {
            border-color: var(--hover-tree-lines-color) !important;
        }
        #hierarchy-editor .TreeNode:focus-within {
            border-color: var(--focused-tree-lines-color) !important;
            border-width: 2px;
        }
        /*--------------- Alt Tree Lines ------------------ */
        #hierarchy-editor .TreeNode--dark-indent-line:hover {
            border-color: var(--alt-hover-tree-lines-color) !important;
        }
        #hierarchy-editor .TreeNode--dark-indent-line:focus-within {
            border-color: var(--alt-focused-tree-lines-color) !important;
        }
        /* rem text in focus and hover */
        #hierarchy-editor .rem-container--default:hover .rem-text:not(.highlight-color--red):not(.highlight-color--orange):not(.highlight-color--yellow):not(.highlight-color--green):not(.highlight-color--blue):not(.highlight-color--purple):not(.rem-todo--finished) {
            color: var(--focused-text-color);
            background-color: transparent;
            margin-left: 11px;
            padding-left: 15px !important;
            border-radius: 6px;
        }
        #hierarchy-editor .rem-container--focused .rem-text:not(.highlight-color--red):not(.highlight-color--orange):not(.highlight-color--yellow):not(.highlight-color--green):not(.highlight-color--blue):not(.highlight-color--purple):not(.rem-todo--finished) {
            color: var(--focused-text-color);
            background-color: var(--focused-background-color);
            margin-left: 11px;
            padding-left: 15px !important;
            border-radius: 6px;
        }
        #hierarchy-editor .rem-container--focused:hover .rem-text:not(.highlight-color--red):not(.highlight-color--orange):not(.highlight-color--yellow):not(.highlight-color--green):not(.highlight-color--blue):not(.highlight-color--purple):not(.rem-todo--finished) {
            color: var(--focused-text-color);
            background-color: var(--focused-background-color);
            margin-left: 11px;
            padding-left: 15px !important;
            border-radius: 6px;
        }
        #hierarchy-editor .rem-container--focused .concept_rem_type {
            color: var(--focused-text-color);
        }
        #hierarchy-editor .rem-container--focused .question_rem_type {
            color: var(--focused-text-color);
        }
        #hierarchy-editor .rem-container--focused .hierarchy-editor__tag-bar__tag {
            color: var(--focused-text-color);
        }
        #hierarchy-editor .rem-container--focused .rem-text .descriptor_rem_type {
            color: var(--focused-text-color);
        }
        /*---------- bullets in focus and hover ----------*/
        /*----general rems bullet hover ----*/
        #hierarchy-editor .rem-container--default:hover .rem-bullet {
            background-color: var(--hover-bullet-color);
            width: 8px;
            height: 8px;
        }
        #hierarchy-editor .rem-container--focused .rem-bullet {
            background-color: var(--focused-bullet-color);
            width: 8px;
            height: 8px;
        }
        /*---- 1st in focus hierarchy bullets ----*/
        #hierarchy-editor .rem-container--focused .rem-bullet, .rem-bullet--in-list,
        #hierarchy-editor  .TreeNode .tree-node-container:focus-within
            > div:first-child .rem-bullet, .rem-bullet--in-list {
            background-color: var(--tree-focused-bullet-color);
            width: 8px;
            height: 8px;
        }
        /*--- 1st in focus hierarchy bullets hover ----*/
        #hierarchy-editor .rem-container--focused .rem-bullet, .rem-bullet--in-list,
        #hierarchy-editor .tree-node-container:focus-within
            > div .rem-container:hover .rem-bullet, .rem-bullet--in-list  {
            background-color: var(--tree-hover-focused-bullet-color);
            width: 8px;
            height: 8px;
        }
        /*---- 1st in focus hierarchy bullets focused hover ----*/
        #hierarchy-editor .rem-container--focused .rem-bullet, .rem-bullet--in-list,
        #hierarchy-editor .tree-node-container:focus-within
            > div .rem-container--focused:hover .rem-bullet, .rem-bullet--in-list  {
            background-color: var(--tree-focused-bullet-color);
            width: 8px;
            height: 8px;
        }
        /*---- 1st NOT in focus hierarchy bullets hover ----*/
        #hierarchy-editor .tree-node-container
            > .TreeNode:not(:focus-within)
            > div ~ div .rem-container:hover .rem-bullet, .rem-bullet--in-list {
            background-color: var(--hover-bullet-color);
            width: 8px;
            height: 8px;
        }
        /*---- in portals ----*/
        #hierarchy-editor .rem-container--focused .rem-bullet, .rem-bullet--in-list,
        #hierarchy-editor .portal-tree-node .tree-node-container:focus-within
            > div:first-child .rem-container--focused .rem-bullet, .rem-bullet--in-list {
            background-color: var(--tree-focused-bullet-color);
            width: 8px;
            height: 8px;
        }
        #hierarchy-editor .rem-container--focused .rem-bullet, .rem-bullet--in-list,
        #hierarchy-editor .portal-tree-node .tree-node-container:focus-within
            > div .rem-container:hover .rem-bullet, .rem-bullet--in-list  {
            background-color: var(--tree-hover-focused-bullet-color);
            width: 8px;
            height: 8px;    
        }
        #hierarchy-editor .rem-container--focused .rem-bullet, .rem-bullet--in-list,
        #hierarchy-editor .portal-tree-node .tree-node-container:focus-within
            > div .rem-container--focused:hover .rem-bullet, .rem-bullet--in-list  {
            background-color: var(--tree-focused-bullet-color);
            width: 8px;
            height: 8px;
        }
        #hierarchy-editor .portal-tree-node .tree-node-container
            > .TreeNode:not(:focus-within)
            > div ~ div .rem-container:hover .rem-bullet, .rem-bullet--in-list {
            background-color: var(--hover-bullet-color);
            width: 8px;
            height: 8px;
        }
        /*---- in search portals ----*/
        #hierarchy-editor .rem-container--focused .rem-bullet, .rem-bullet--in-list,
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container:focus-within
            > div:first-child .rem-container--focused .rem-bullet, .rem-bullet--in-list {
            background-color: var(--tree-focused-bullet-color);
            width: 8px;
            height: 8px;
        }
        #hierarchy-editor .rem-container--focused .rem-bullet, .rem-bullet--in-list,
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container:focus-within
            > div .rem-container:hover .rem-bullet, .rem-bullet--in-list  {
            background-color: var(--tree-hover-focused-bullet-color);
            width: 8px;
            height: 8px;
        }
        #hierarchy-editor .rem-container--focused .rem-bullet, .rem-bullet--in-list,
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container:focus-within
            > div .rem-container--focused:hover .rem-bullet, .rem-bullet--in-list  {
            background-color: var(--tree-focused-bullet-color);
            width: 8px;
            height: 8px;
        }
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container
            > .TreeNode:not(:focus-within)
            > div ~ div .rem-container:hover .rem-bullet, .rem-bullet--in-list {
            background-color: var(--hover-bullet-color);
            width: 8px;
            height: 8px;
        }
        /*---------- Alt bullets in focus and hover ----------*/
        /*---- tree container ----*/
        /*---- Alt in focus hierarchy bullets ----*/
        #hierarchy-editor .tree-node-container 
            > .TreeNode--dark-indent-line > div:focus-within
            > div:first-child .rem-container--default .rem-bullet, .rem-bullet--in-list {
            background-color: var(--alt-tree-focused-bullet-color);
            width: 8px;
            height: 8px;
        }
        /*---- Alt in focus hierarchy bullets hover ----*/
        #hierarchy-editor .tree-node-container 
            > .TreeNode--dark-indent-line:focus-within > div:hover
            > div:first-child .rem-container--default:hover .rem-bullet, .rem-bullet--in-list {
            background-color: var(--alt-tree-hover-focused-bullet-color);
            width: 8px;
            height: 8px;
        }
        /*---- Alt in focus hierarchy bullets focused ----*/
        #hierarchy-editor .tree-node-container 
            > .TreeNode--dark-indent-line:focus-within > div
            > div:first-child .rem-container--focused .rem-bullet, .rem-bullet--in-list {
            background-color: var(--alt-tree-focused-bullet-color);
            width: 8px;
            height: 8px;
        }
        #hierarchy-editor .tree-node-container 
            > .TreeNode--dark-indent-line > div
            > div:first-child .rem-container--focused .rem-bullet, .rem-bullet--in-list {
            background-color: var(--alt-tree-focused-bullet-color);
            width: 8px;
            height: 8px;
        }
        /*---- Alt in focus hierarchy bullets focused:hover ----*/
        #hierarchy-editor .tree-node-container 
            > .TreeNode--dark-indent-line:focus-within > div:hover
            > div:first-child .rem-container--focused:hover .rem-bullet, .rem-bullet--in-list {
            background-color: var(--alt-tree-focused-bullet-color);
            width: 8px;
            height: 8px;
        }
        /*---- Alt NOT in focus hierarchy bullets hover ----*/
        #hierarchy-editor .tree-node-container 
            > .TreeNode--dark-indent-line:not(:focus-within) > div:hover
            > div:first-child .rem-container--default:hover .rem-bullet, .rem-bullet--in-list {
            background-color: var(--alt-tree-hover-bullet-color);
            width: 8px;
            height: 8px;
        }
        /*---- in portals ----*/
        /*---- Alt in focus hierarchy bullets ----*/
        #hierarchy-editor .portal-tree-node .tree-node-container 
            > .TreeNode--dark-indent-line > div:focus-within
            > div:first-child .rem-container--default .rem-bullet, .rem-bullet--in-list {
            background-color: var(--alt-tree-focused-bullet-color);
            width: 8px;
            height: 8px;
        }
        /*---- Alt in focus hierarchy bullets hover ----*/
        #hierarchy-editor .portal-tree-node .tree-node-container 
            > .TreeNode--dark-indent-line:focus-within > div:hover
            > div:first-child .rem-container--default:hover .rem-bullet, .rem-bullet--in-list {
            background-color: var(--alt-tree-hover-focused-bullet-color);
            width: 8px;
            height: 8px;
        }
        /*---- Alt in focus hierarchy bullets focused ----*/
        #hierarchy-editor .portal-tree-node .tree-node-container 
            > .TreeNode--dark-indent-line:focus-within > div
            > div:first-child .rem-container--focused .rem-bullet, .rem-bullet--in-list {
            background-color: var(--alt-tree-focused-bullet-color);
            width: 8px;
            height: 8px;
        }
        #hierarchy-editor .portal-tree-node .tree-node-container 
            > .TreeNode--dark-indent-line > div
            > div:first-child .rem-container--focused .rem-bullet, .rem-bullet--in-list {
            background-color: var(--alt-tree-focused-bullet-color);
            width: 8px;
            height: 8px;
        }
        /*---- Alt in focus hierarchy bullets focused:hover ----*/
        #hierarchy-editor .portal-tree-node .tree-node-container 
            > .TreeNode--dark-indent-line:focus-within > div:hover
            > div:first-child .rem-container--focused:hover .rem-bullet, .rem-bullet--in-list {
            background-color: var(--alt-tree-focused-bullet-color);
            width: 8px;
            height: 8px;
        }
        /*---- Alt NOT in focus hierarchy bullets hover ----*/
        #hierarchy-editor .portal-tree-node .tree-node-container 
            > .TreeNode--dark-indent-line:not(:focus-within) > div:hover
            > div:first-child .rem-container--default:hover .rem-bullet, .rem-bullet--in-list {
            background-color: var(--alt-tree-hover-bullet-color);
            width: 8px;
            height: 8px;
        }
        /*---- in search portals ----*/
        /*---- Alt in focus hierarchy bullets ----*/
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container 
            > .TreeNode--dark-indent-line > div:focus-within
            > div:first-child .rem-container--default .rem-bullet, .rem-bullet--in-list {
            background-color: var(--alt-tree-focused-bullet-color);
            width: 8px;
            height: 8px;
        }
        /*---- Alt in focus hierarchy bullets hover ----*/
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container 
            > .TreeNode--dark-indent-line:focus-within > div:hover
            > div:first-child .rem-container--default:hover .rem-bullet, .rem-bullet--in-list {
            background-color: var(--alt-tree-hover-focused-bullet-color);
            width: 8px;
            height: 8px;
        }
        /*---- Alt in focus hierarchy bullets focused ----*/
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container 
            > .TreeNode--dark-indent-line:focus-within > div
            > div:first-child .rem-container--focused .rem-bullet, .rem-bullet--in-list {
            background-color: var(--alt-tree-focused-bullet-color);
            width: 8px;
            height: 8px;
        }
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container 
            > .TreeNode--dark-indent-line > div
            > div:first-child .rem-container--focused .rem-bullet, .rem-bullet--in-list {
            background-color: var(--alt-tree-focused-bullet-color);
            width: 8px;
            height: 8px;
        }
        /*---- Alt in focus hierarchy bullets focused:hover ----*/
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container 
            > .TreeNode--dark-indent-line:focus-within > div:hover
            > div:first-child .rem-container--focused:hover .rem-bullet, .rem-bullet--in-list {
            background-color: var(--alt-tree-focused-bullet-color);
            width: 8px;
            height: 8px;
        }
        /*---- Alt NOT in focus hierarchy bullets hover ----*/
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container 
            > .TreeNode--dark-indent-line:not(:focus-within) > div:hover
            > div:first-child .rem-container--default:hover .rem-bullet, .rem-bullet--in-list {
            background-color: var(--alt-tree-hover-bullet-color);
            width: 8px;
            height: 8px;
        }
        /*---------- bullets icons in focus and hover ----------*/
        /*----general rems bullet icons hover ----*/
        #hierarchy-editor .rem-container--default:hover .rem-bullet__icon {
            color: var(--hover-bullet-color) !important;
        }
        /*---- 1st in focus hierarchy bullet icons ----*/
        #hierarchy-editor .tree-node-container:focus-within
            > div:first-child .rem-bullet__icon {
            color: var(--tree-focused-bullet-color) !important;
        }
        #hierarchy-editor .tree-node-container 
            > div
            > div:first-child .rem-container--focused .rem-bullet__icon {
            color: var(--tree-focused-bullet-color);
        }
        /*--- 1st in focus hierarchy bullet icons hover ----*/
        #hierarchy-editor .tree-node-container:focus-within
            > div .rem-container:hover .rem-bullet__icon  {
            color: var(--tree-hover-focused-bullet-color) !important;
        }
        /*---- 1st in focus hierarchy bullet icons focused hover ----*/
        #hierarchy-editor .tree-node-container:focus-within
            > div .rem-container--focused:hover .rem-bullet__icon  {
            color: var(--tree-focused-bullet-color) !important;
        }
        /*---- 1st NOT in focus hierarchy bullet icons hover ----*/
        #hierarchy-editor .tree-node-container
            > .TreeNode:not(:focus-within)
            > div ~ div .rem-container:hover .rem-bullet__icon {
            color: var(--hover-bullet-color) !important;
        }
        /*---- in portals ----*/
        #hierarchy-editor .portal-tree-node .tree-node-container:focus-within
            > div:first-child .rem-container--focused .rem-bullet__icon {
            color: var(--tree-focused-bullet-color) !important;
            width: 8px;
            height: 8px;
        }
        #hierarchy-editor .portal-tree-node .tree-node-container 
            > div
            > div:first-child .rem-container--focused .rem-bullet__icon {
            color: var(--tree-focused-bullet-color);
        }
        #hierarchy-editor .portal-tree-node .tree-node-container:focus-within
            > div .rem-container:hover .rem-bullet__icon  {
            color: var(--tree-hover-focused-bullet-color) !important;
            width: 8px;
            height: 8px;    
        }
        #hierarchy-editor .portal-tree-node .tree-node-container:focus-within
            > div .rem-container--focused:hover .rem-bullet__icon  {
            color: var(--tree-focused-bullet-color) !important;
            width: 8px;
            height: 8px;
        }
        #hierarchy-editor .portal-tree-node .tree-node-container
            > .TreeNode:not(:focus-within)
            > div ~ div .rem-container:hover .rem-bullet__icon {
            color: var(--hover-bullet-color) !important;
            width: 8px;
            height: 8px;
        }
        /*---- in search portals ----*/
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container:focus-within
            > div:first-child .rem-container--focused .rem-bullet__icon {
            color: var(--tree-focused-bullet-color) !important;
            width: 8px;
            height: 8px;
        }
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container 
            > div
            > div:first-child .rem-container--focused .rem-bullet__icon {
            color: var(--tree-focused-bullet-color);
        }
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container:focus-within
            > div .rem-container:hover .rem-bullet__icon  {
            color: var(--tree-hover-focused-bullet-color) !important;
            width: 8px;
            height: 8px;
        }
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container:focus-within
            > div .rem-container--focused:hover .rem-bullet__icon  {
            color: var(--tree-focused-bullet-color) !important;
            width: 8px;
            height: 8px;
        }
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container
            > .TreeNode:not(:focus-within)
            > div ~ div .rem-container:hover .rem-bullet__icon {
            color: var(--hover-bullet-color) !important;
            width: 8px;
            height: 8px;
        }
        /*---------- Alt bullet icons in focus and hover ----------*/
        /*---- tree container ----*/
        /*---- Alt in focus hierarchy bullet icons ----*/
        #hierarchy-editor .tree-node-container 
            > .TreeNode--dark-indent-line > div:focus-within
            > div:first-child .rem-container--default .rem-bullet__icon {
            color: var(--alt-tree-focused-bullet-color) !important;
            width: 8px;
            height: 8px;
        }
        /*---- Alt in focus hierarchy bullet icons hover ----*/
        #hierarchy-editor .tree-node-container 
            > .TreeNode--dark-indent-line:focus-within > div:hover
            > div:first-child .rem-container--default:hover .rem-bullet__icon {
            color: var(--alt-tree-hover-focused-bullet-color) !important;
            width: 8px;
            height: 8px;
        }
        /*---- Alt in focus hierarchy bullet icons focused ----*/
        #hierarchy-editor .tree-node-container 
            > .TreeNode--dark-indent-line:focus-within > div
            > div:first-child .rem-container--focused .rem-bullet__icon {
            color: var(--alt-tree-focused-bullet-color) !important;
        }
        #hierarchy-editor .tree-node-container 
            > .TreeNode--dark-indent-line > div
            > div:first-child .rem-container--focused .rem-bullet__icon {
            color: var(--alt-tree-focused-bullet-color);
        }
        /*---- Alt in focus hierarchy bullet icons focused:hover ----*/
        #hierarchy-editor .tree-node-container 
            > .TreeNode--dark-indent-line:focus-within > div:hover
            > div:first-child .rem-container--focused:hover .rem-bullet__icon {
            color: var(--alt-tree-focused-bullet-color) !important;
            width: 8px;
            height: 8px;
        }
        /*---- Alt NOT in focus hierarchy bullet icons hover ----*/
        #hierarchy-editor .tree-node-container 
            > .TreeNode--dark-indent-line:not(:focus-within) > div:hover
            > div:first-child .rem-container--default:hover .rem-bullet__icon {
            color: var(--alt-tree-hover-bullet-color) !important;
            width: 8px;
            height: 8px;
        }
        /*---- in portals ----*/
        /*---- Alt in focus hierarchy bullet icons ----*/
        #hierarchy-editor .portal-tree-node .tree-node-container 
            > .TreeNode--dark-indent-line > div:focus-within
            > div:first-child .rem-container--default .rem-bullet__icon {
            color: var(--alt-tree-focused-bullet-color) !important;
            width: 8px;
            height: 8px;
        }
        /*---- Alt in focus hierarchy bullet icons hover ----*/
        #hierarchy-editor .portal-tree-node .tree-node-container 
            > .TreeNode--dark-indent-line:focus-within > div:hover
            > div:first-child .rem-container--default:hover .rem-bullet__icon {
            color: var(--alt-tree-hover-focused-bullet-color) !important;
            width: 8px;
            height: 8px;
        }
        /*---- Alt in focus hierarchy bullet icons focused ----*/
        #hierarchy-editor .portal-tree-node .tree-node-container 
            > .TreeNode--dark-indent-line:focus-within > div
            > div:first-child .rem-container--focused .rem-bullet__icon {
            color: var(--alt-tree-focused-bullet-color) !important;
            width: 8px;
            height: 8px;
        }
        #hierarchy-editor .portal-tree-node .tree-node-container 
            > .TreeNode--dark-indent-line > div
            > div:first-child .rem-container--focused .rem-bullet__icon {
            color: var(--alt-tree-focused-bullet-color);
        }
        /*---- Alt in focus hierarchy bullet icons focused:hover ----*/
        #hierarchy-editor .portal-tree-node .tree-node-container 
            > .TreeNode--dark-indent-line:focus-within > div:hover
            > div:first-child .rem-container--focused:hover .rem-bullet__icon {
            color: var(--alt-tree-focused-bullet-color) !important;
            width: 8px;
            height: 8px;
        }
        /*---- Alt NOT in focus hierarchy bullet icons hover ----*/
        #hierarchy-editor .portal-tree-node .tree-node-container 
            > .TreeNode--dark-indent-line:not(:focus-within) > div:hover
            > div:first-child .rem-container--default:hover .rem-bullet__icon {
            color: var(--alt-tree-hover-bullet-color) !important;
            width: 8px;
            height: 8px;
        }
        /*---- in search portals ----*/
        /*---- Alt in focus hierarchy bullet icons ----*/
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container 
            > .TreeNode--dark-indent-line > div:focus-within
            > div:first-child .rem-container--default .rem-bullet__icon {
            color: var(--alt-tree-focused-bullet-color) !important;
            width: 8px;
            height: 8px;
        }
        /*---- Alt in focus hierarchy bullet icons hover ----*/
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container 
            > .TreeNode--dark-indent-line:focus-within > div:hover
            > div:first-child .rem-container--default:hover .rem-bullet__icon {
            color: var(--alt-tree-hover-focused-bullet-color) !important;
            width: 8px;
            height: 8px;
        }
        /*---- Alt in focus hierarchy bullet icons focused ----*/
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container 
            > .TreeNode--dark-indent-line:focus-within > div
            > div:first-child .rem-container--focused .rem-bullet__icon {
            color: var(--alt-tree-focused-bullet-color) !important;
            width: 8px;
            height: 8px;
        }
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container 
            > .TreeNode--dark-indent-line > div
            > div:first-child .rem-container--focused .rem-bullet__icon {
            color: var(--alt-tree-focused-bullet-color);
        }
        /*---- Alt in focus hierarchy bullet icons focused:hover ----*/
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container 
            > .TreeNode--dark-indent-line:focus-within > div:hover
            > div:first-child .rem-container--focused:hover .rem-bullet__icon {
            color: var(--alt-tree-focused-bullet-color) !important;
            width: 8px;
            height: 8px;
        }
        /*---- Alt NOT in focus hierarchy bullet icons hover ----*/
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container 
            > .TreeNode--dark-indent-line:not(:focus-within) > div:hover
            > div:first-child .rem-container--default:hover .rem-bullet__icon {
            color: var(--alt-tree-hover-bullet-color) !important;
            width: 8px;
            height: 8px;
        }
        /*---------- hamburger and collapse button position ----------*/
        /*rem container*/
        #hierarchy-editor .TreeNode .rem-container:hover .rem-hamburger {
            margin-left: -16px;
            margin-top: 0px !important;
        }
        #hierarchy-editor .TreeNode .rem-container--focused .rem-hamburger {
            filter: brightness(1.4);
            margin-left: -16px;
            margin-top: 0px !important;
        }
        #hierarchy-editor .rem-container--focused .rem-hamburger {
            filter: brightness(1.4);
        }
        #hierarchy-editor .TreeNode .rem-container:hover .toggleCollapseButton {
            margin-left: -18px;
            margin-top: 1px !important;
        }
        #hierarchy-editor .TreeNode .rem-container--focused .toggleCollapseButton {
            filter: brightness(1.4);
            margin-left: -18px;
            margin-top: 1px !important;
        }
        #hierarchy-editor .rem-container--focused .toggleCollapseButton {
            filter: brightness(1.4);
        }
        /*H1*/
        #hierarchy-editor .rem__button-offset-1  {
            margin-top: 0px !important;
            padding-top: 1px !important;
        } 
        /*H2*/
        #hierarchy-editor .rem__button-offset-2 {
            margin-top: 0px !important;
            padding-top: 1px !important;
        }
        /*H3*/
        #hierarchy-editor .rem__button-offset-3 {
            margin-top: 0px !important;
            padding-top: 1px !important;
        }
        /* list in cards*/
        #hierarchy-editor .tree-node-container .TreeNode--list--in-card-content  .rem-container:hover .rem-hamburger {
            margin-left: -12px;
            margin-top: 0px;
        }
        #hierarchy-editor .tree-node-container .TreeNode--list--in-card-content .rem-container:hover .toggleCollapseButton {
            margin-left: -15px;
            margin-top: 1px;
        }
        #hierarchy-editor .rem-container--focused .rem-reference-link {
            color: var(--focused-accent-color);
            font-weight: 500;
        }
        #hierarchy-editor .rem-container--focused .LinkNode {
            text-decoration: underline;
            color: var(--focused-accent-color);
            font-weight: 500;
        }
        #hierarchy-editor .rem-container--default .rem-reference-link i.icon.calendar.alternate.outline::before {
            filter: var(--accent-color-filter) brightness(1.3);
        }
        #hierarchy-editor .rem-container--focused .rem-reference-link i.icon.calendar.alternate.outline::before {
            filter: var(--accent-color-filter) brightness(1.5);
        }
        #hierarchy-editor .rem-container--focused i.icon.calendar.alternate.outline::before {
            filter: var(--icons-filter) brightness(1.5);
        }
        #hierarchy-editor .rem-container--focused .quote {
            margin-right: 0px;
            margin-left: 0px;
            background-color: transparent;
            border-radius: 5px;   
        }
        #hierarchy-editor .rem-container--focused .katex {
            color: var(--focused-accent-color);
        }
        #hierarchy-editor .rem-container--focused .LinkNode img {
            filter: var(--focused-accent-color-filter);
        }
        #hierarchy-editor .search-portal-tree-node--dark .quote {
            margin-left: 0px;
            margin-right: 0px;
            padding-left: 2px;
            padding-right: 2px;
        }
        /* Hannesfrank column library*/
        #hierarchy-editor .tree-node-container[data-rem-container-tags~="columns"] > .TreeNode > .tree-node-container .rem-container:hover  {
            background: none;
            background-image: none!important;
        }
        #hierarchy-editor .tree-node-container[data-rem-container-tags~="columns"] > .TreeNode > .tree-node-container .rem-container--focused  {
            background: none;
            background-image: none!important;
        }
        #hierarchy-editor .tree-node-container[data-rem-container-tags~="columns"] > .TreeNode > .tree-node-container .rem-container--focused:hover  {
            background: none;
            background-image: none!important;    
        }
        ```
    - [ ] Treenode Branch symbols
        ```css
        /*------- 1st Tree node symbols when in focus and hover ------*/
        #hierarchy-editor .tree-node-container
            > .TreeNode > div:focus-within 
            > div:first-child .rem-container--default {
            background: none;
            background-image: var(--focused-branch-tree-symbol);
            background-repeat: no-repeat;
            background-size: var(--branch-tree-symbol-size);
            background-position-x: var(--branch-tree-symbol-position-x);
            background-position-y: var(--branch-tree-symbol-position-y);
        }
        #hierarchy-editor .tree-node-container
            > .TreeNode > div 
            > div:first-child .rem-container--focused {
            background: none;
            background-image: var(--focused-branch-tree-symbol);
            background-repeat: no-repeat;
            background-size: var(--branch-tree-symbol-size);
            background-position-x: var(--branch-tree-symbol-position-x);
            background-position-y: var(--branch-tree-symbol-position-y);
        }
        #hierarchy-editor .tree-node-container 
            > .TreeNode > div
            > div:first-child .rem-container--default:hover {
            background: none;
            background-image: var(--hover-focused-branch-tree-symbol);
            background-repeat: no-repeat;
            background-size: var(--branch-tree-symbol-size);
            background-position-x: var(--branch-tree-symbol-position-x);
            background-position-y: var(--branch-tree-symbol-position-y);
        }
        #hierarchy-editor .tree-node-container
            > .TreeNode > div 
            > div:first-child .rem-container--focused:hover {
            background: none;
            background-image: var(--focused-branch-tree-symbol);
            background-repeat: no-repeat;
            background-size: var(--branch-tree-symbol-size);
            background-position-x: var(--branch-tree-symbol-position-x);
            background-position-y: var(--branch-tree-symbol-position-y);
        }
        /*---- in portals ----*/
        #hierarchy-editor .portal-tree-node .tree-node-container 
            > .TreeNode
            > div .rem-container--default:hover {
            background: none;
            background-image: var(--hover-focused-branch-tree-symbol);
            background-repeat: no-repeat;
            background-size: var(--branch-tree-symbol-size);
            background-position-x: var(--branch-tree-symbol-position-x);
            background-position-y: var(--branch-tree-symbol-position-y);
        }
        /*---- in search portals ----*/
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container 
            > .TreeNode
            > div .rem-container--default:hover {
            background: none;
            background-image: var(--hover-focused-branch-tree-symbol);
            background-repeat: no-repeat;
            background-size: var(--branch-tree-symbol-size);
            background-position-x: var(--branch-tree-symbol-position-x);
            background-position-y: var(--branch-tree-symbol-position-y);
        }
        /*---- Not in focus general ----*/
        #hierarchy-editor .tree-node-container
            > .TreeNode:not(:focus-within)
            > div ~ div .rem-container--default:hover {
            background: none;
            background-image: var(--hover-branch-tree-symbol);
            background-repeat: no-repeat;
            background-size: var(--branch-tree-symbol-size);
            background-position-x: var(--branch-tree-symbol-position-x);
            background-position-y: var(--branch-tree-symbol-position-y);
        }
        /*---- Not in focus portals ----*/
        #hierarchy-editor .portal-tree-node .tree-node-container
            > .TreeNode:not(:focus-within)
            > div ~ div .rem-container--default:hover {
            background: none;
            background-image: var(--hover-branch-tree-symbol);
            background-repeat: no-repeat;
            background-size: var(--branch-tree-symbol-size);
            background-position-x: var(--branch-tree-symbol-position-x);
            background-position-y: var(--branch-tree-symbol-position-y);
        }
        /*---- Not in focus search portals ----*/
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container
            > .TreeNode:not(:focus-within)
            > div ~ div .rem-container--default:hover {
            background: none;
            background-image: var(--hover-branch-tree-symbol);
            background-repeat: no-repeat;
            background-size: var(--branch-tree-symbol-size);
            background-position-x: var(--branch-tree-symbol-position-x);
            background-position-y: var(--branch-tree-symbol-position-y);
        }
        /*---- Portals within portals first symbol hidden ----*/
        /*---- in portals ----*/
        #hierarchy-editor .tree-node-container 
            > .TreeNode .portal-tree-node
            > div 
            > div:first-child .rem-container--focused  {
            background: none;
            background-image: none;
        }
        #hierarchy-editor .tree-node-container 
            > .TreeNode .portal-tree-node
            > div 
            > div:first-child .rem-container--default:hover  {
            background: none;
            background-image: none;
        }
        #hierarchy-editor .tree-node-container:focus-within 
            > .TreeNode .portal-tree-node
            > div 
            > div:first-child .rem-container--default:hover  {
            background: none;
            background-image: none;
        }
        /*---- in search portal ----*/
        #hierarchy-editor .tree-node-container 
            > .TreeNode .search-portal-tree-node--dark
            > div 
            > div:first-child .rem-container--focused  {
            background: none;
            background-image: none;
        }
        #hierarchy-editor .tree-node-container 
            > .TreeNode .search-portal-tree-node--dark
            > div 
            > div:first-child .rem-container--default:hover  {
            background: none;
            background-image: none;
        }
        #hierarchy-editor .tree-node-container:focus-within 
            > .TreeNode .search-portal-tree-node--dark
            > div 
            > div:first-child .rem-container--default:hover {
            background: none;
            background-image: none;
        }
        /*------- Alt Tree node symbols when in focus and hover ------*/
        /*general tree node hierarchy container symbol*/
        #hierarchy-editor .tree-node-container 
            > .TreeNode--dark-indent-line > div:focus-within
            > div:first-child .rem-container--default {
            background: none;
            background-image: var(--alt-focused-branch-tree-symbol);
            background-repeat: no-repeat;
            background-size: var(--branch-tree-symbol-size);
            background-position-x: var(--branch-tree-symbol-position-x);
            background-position-y: var(--branch-tree-symbol-position-y);
        }
        /*------ Alt Tree node rem container when in focus and hover -----*/
        /*general tree node container focused*/
        #hierarchy-editor .tree-node-container 
            > .TreeNode--dark-indent-line > div
            > div:first-child .rem-container--focused {
            background: none;
            background-image: var(--alt-focused-branch-tree-symbol);
            background-repeat: no-repeat;
            background-size: var(--branch-tree-symbol-size);
            background-position-x: var(--branch-tree-symbol-position-x);
            background-position-y: var(--branch-tree-symbol-position-y);
        }
        /*general tree node container hover*/
        #hierarchy-editor .tree-node-container 
            > .TreeNode--dark-indent-line > div
            > div:first-child .rem-container--default:hover {
            background: none;
            background-image: var(--alt-hover-focused-branch-tree-symbol);
            background-repeat: no-repeat;
            background-size: var(--branch-tree-symbol-size);
            background-position-x: var(--branch-tree-symbol-position-x);
            background-position-y: var(--branch-tree-symbol-position-y);   
        }
        /*general tree node container focused:hover*/
        #hierarchy-editor .tree-node-container 
            > .TreeNode--dark-indent-line > div
            > div:first-child .rem-container--focused:hover {
            background: none;
            background-image: var(--alt-focused-branch-tree-symbol);
            background-repeat: no-repeat;
            background-size: var(--branch-tree-symbol-size);
            background-position-x: var(--branch-tree-symbol-position-x);
            background-position-y: var(--branch-tree-symbol-position-y);
        }
        /*general tree node container hover after the in focus rem container*/
        #hierarchy-editor .tree-node-container 
            > .TreeNode--dark-indent-line:not(:focus-within) > div
            > div:first-child .rem-container--default:hover {
            background: none;
            background-image: var(--alt-hover-branch-tree-symbol);
            background-repeat: no-repeat;
            background-size: var(--branch-tree-symbol-size);
            background-position-x: var(--branch-tree-symbol-position-x);
            background-position-y: var(--branch-tree-symbol-position-y);
        }
        /*---------- in portals ----------*/
        /*------- Alt Tree node symbols when in focus and hover ------*/
        /*---- in portal tree node hierarchy container symbol ----*/
        #hierarchy-editor .portal-tree-node .tree-node-container 
            > .TreeNode--dark-indent-line > div:focus-within
            > div:first-child .rem-container--default {
            background: none;
            background-image: var(--alt-focused-branch-tree-symbol);
            background-repeat: no-repeat;
            background-size: var(--branch-tree-symbol-size);
            background-position-x: var(--branch-tree-symbol-position-x);
            background-position-y: var(--branch-tree-symbol-position-y);
        }
        /*------ Alt Tree node rem container when in focus and hover -----*/
        /*---- in portal tree node container focused ----*/
        #hierarchy-editor .portal-tree-node .tree-node-container 
            > .TreeNode--dark-indent-line > div
            > div:first-child .rem-container--focused {
            background: none;
            background-image: var(--alt-focused-branch-tree-symbol);
            background-repeat: no-repeat;
            background-size: var(--branch-tree-symbol-size);
            background-position-x: var(--branch-tree-symbol-position-x);
            background-position-y: var(--branch-tree-symbol-position-y);
        }
        /*---- in portal tree node container hover ----*/
        #hierarchy-editor .portal-tree-node .tree-node-container 
            > .TreeNode--dark-indent-line > div
            > div:first-child .rem-container--default:hover {
            background: none;
            background-image: var(--alt-hover-focused-branch-tree-symbol);
            background-repeat: no-repeat;
            background-size: var(--branch-tree-symbol-size);
            background-position-x: var(--branch-tree-symbol-position-x);
            background-position-y: var(--branch-tree-symbol-position-y);
        }
        /*---- in portal tree node container focused:hover ----*/
        #hierarchy-editor .portal-tree-node .tree-node-container 
            > .TreeNode--dark-indent-line > div
            > div:first-child .rem-container--focused:hover {
            background: none;
            background-image: var(--alt-focused-branch-tree-symbol);
            background-repeat: no-repeat;
            background-size: var(--branch-tree-symbol-size);
            background-position-x: var(--branch-tree-symbol-position-x);
            background-position-y: var(--branch-tree-symbol-position-y);
        }
        /*---- in portal tree node container hover after the in focus rem container ----*/
        #hierarchy-editor .portal-tree-node .tree-node-container 
            > .TreeNode--dark-indent-line:not(:focus-within) > div
            > div:first-child .rem-container--default:hover {
            background: none;
            background-image: var(--alt-hover-branch-tree-symbol);
            background-repeat: no-repeat;
            background-size: var(--branch-tree-symbol-size);
            background-position-x: var(--branch-tree-symbol-position-x);
            background-position-y: var(--branch-tree-symbol-position-y);
        }
        /*---------- Search portals ----------*/
        /*------- Alt Tree node symbols when in focus and hover ------*/
        /*---- in portal tree node hierarchy container symbol ----*/
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container 
            > .TreeNode--dark-indent-line > div:focus-within
            > div:first-child .rem-container--default {
            background: none;
            background-image: var(--alt-focused-branch-tree-symbol);
            background-repeat: no-repeat;
            background-size: var(--branch-tree-symbol-size);
            background-position-x: var(--branch-tree-symbol-position-x);
            background-position-y: var(--branch-tree-symbol-position-y);
        }
        /*------ Alt Tree node rem container when in focus and hover -----*/
        /*---- in portal tree node container focused ----*/
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container 
            > .TreeNode--dark-indent-line > div
            > div:first-child .rem-container--focused {
            background: none;
            background-image: var(--alt-focused-branch-tree-symbol);
            background-repeat: no-repeat;
            background-size: var(--branch-tree-symbol-size);
            background-position-x: var(--branch-tree-symbol-position-x);
            background-position-y: var(--branch-tree-symbol-position-y);
        }
        /*---- in portal tree node container hover ----*/
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container 
            > .TreeNode--dark-indent-line > div
            > div:first-child .rem-container--default:hover {
            background: none;
            background-image: var(--alt-hover-focused-branch-tree-symbol);
            background-repeat: no-repeat;
            background-size: var(--branch-tree-symbol-size);
            background-position-x: var(--branch-tree-symbol-position-x);
            background-position-y: var(--branch-tree-symbol-position-y);
        }
        /*---- in portal tree node container focused:hover ----*/
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container 
            > .TreeNode--dark-indent-line > div
            > div:first-child .rem-container--focused:hover {
            background: none;
            background-image: var(--alt-focused-branch-tree-symbol);
            background-repeat: no-repeat;
            background-size: var(--branch-tree-symbol-size);
            background-position-x: var(--branch-tree-symbol-position-x);
            background-position-y: var(--branch-tree-symbol-position-y);
        }
        /*---- in portal tree node container hover after the in focus rem container ----*/
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container 
            > .TreeNode--dark-indent-line:not(:focus-within) > div
            > div:first-child .rem-container--default:hover {
            background: none;
            background-image: var(--alt-hover-branch-tree-symbol);
            background-repeat: no-repeat;
            background-size: var(--branch-tree-symbol-size);
            background-position-x: var(--branch-tree-symbol-position-x);
            background-position-y: var(--branch-tree-symbol-position-y);
        }
        /*--------- multi-line/list card in focus and hover ----------*/
        #hierarchy-editor .tree-node-container
            > .TreeNode
            > div:focus-within .TreeNode--list--in-card-content .rem-container--focused {
            background-image: none;
        }
        #hierarchy-editor .tree-node-container
            > .TreeNode
            > div:hover .TreeNode--list--in-card-content .rem-container:hover {
            background-image: none;
        }
        #hierarchy-editor .tree-node-container
            > .TreeNode
            > div:focus-within .TreeNode--list--in-card-content .rem-container--focused:hover {
            background-image: none;
        }
        /*-------- multi-line/list card in focus and hover -----------*/
        /*inside portals*/
        #hierarchy-editor .portal-tree-node .tree-node-container
            > .TreeNode
            > div:focus-within .TreeNode--list--in-card-content .rem-container--focused {
            background-image: none;
        }
        #hierarchy-editor .portal-tree-node .tree-node-container
            > .TreeNode
            > div:hover .TreeNode--list--in-card-content .rem-container:hover {
            background-image: none;
        }
        #hierarchy-editor .portal-tree-node .tree-node-container
            > .TreeNode
            > div:focus-within .TreeNode--list--in-card-content .rem-container--focused:hover {
            background-image: none;
        }
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container
            > .TreeNode
            > div:focus-within .TreeNode--list--in-card-content .rem-container--focused {
            background-image: none;
        }
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container
            > .TreeNode
            > div:hover .TreeNode--list--in-card-content .rem-container:hover {
            background-image: none;
        }
        #hierarchy-editor .search-portal-tree-node--dark .tree-node-container
            > .TreeNode
            > div:focus-within .TreeNode--list--in-card-content .rem-container--focused:hover {
            background-image: none;
        }
        ```
  - ## 18 Windowed Panes ##Todo
    ```css
    /* If Windowed Panes is ON*/
    /* Code by Henrik */
    /* added 09 June 2021 */
    .mosaic-window-body {
        background: var(--body-background-color)!important;
    }
    .mosaic {
        background: var(--blackout-background-color)!important
    }
    .mosaic-window-toolbar.draggable,
    .mosaic-preview .mosaic-window-toolbar, .mosaic-window .mosaic-window-toolbar {
        background-color: var(--body-background-color)!important;
    }
    .mosaic.mosaic-blueprint-theme .mosaic-preview .mosaic-window-toolbar.draggable:hover, .mosaic.mosaic-blueprint-theme .mosaic-window .mosaic-window-toolbar.draggable:hover
    {
        background: var(--selected-background-color)!important;
    }
    .mosaic-default-control {
    color: var(--button-color)!important;
    background: none;
    border: none;
    cursor: pointer;
    }
    ```
  - ## 19 Latex ##Todo
    ```css
    .katex {
        color: var(--latex-text-color);
    }
    .latex-node__empty {
        padding: 3px;
        border-radius: 3px;
        background-color: transparent;
        color: var(--icons-color);
        filter: brightness(0.85);
    }
    .rich-text-editor__popup-text-editor {
        background-color: var(--popup-background-color)!important;
        border: var(--popup-border-width) solid var(--popup-border-color);
        border-radius: var(--popup-border-radius);
        box-shadow: none;
    }.rich-text-editor__popup-text-editor .rich-text-editor__popup-text-editor__input__latex {
        background-color: var(--popup-background-color);
        color: var(--body-text-color);
    }
    .katex-display {
        border-radius: 10px;
        background-color: rgb(34, 36, 36);
    }
    ```
  - ## * Optionals * ##Todo
    - [x] Op01 Hide Remnote Logo
      ```css
      #document-sidebar_top #logo {
          display: none !important;
      }
      .document-sidebar_top__user-and-collapse {
          margin-top: 10px !important;
      }
      ```
    - [x] Op02 Account/Knowledge base name
      ```css
      :root {
          --sidebar-account-name: 'Eustachio';
          --sidebar-account-name-text-size: 20px;
      }
      #document-sidebar__account-capsule__text {
          display: none !important;
      }
      .acc-capsule__menu__account .acc-capsule__menu__name{
          font-size: 0px;
      }
      .acc-capsule__menu__account .acc-capsule__menu__name::before {
          content: var(--sidebar-account-name);
          color: var(--accent-color);
          font-size: 14px;
      }
      #document-sidebar__account-capsule .document-sidebar__account-capsule__name {
          font-size: 0px;
          padding-right: 70px !important;
          margin-right: -65px !important;
          max-width: 200px;
      }
      #document-sidebar__account-capsule .document-sidebar__account-capsule__name::before {
          content: var(--sidebar-account-name);
          font-size: var(--sidebar-account-name-text-size);
      }      
      ```
    - [x] Op03 Document hover preview OFF
      ```css
      #document-hover-preview {
          display: none!important;
      }
      ```
    - [x] Op04 Hide help button
      ```css
      #help-button {
          display: none;
      }
      ```
    - [x] Op05 Power-up symbols OFF
      ```css
      .hierarchy-editor__tag-bar .hierarchy-editor__tag-bar__power-up-tag {
          display: none;
      }
      ```
    - [x] Op06 Minimal sidebar
      ```css
      /* hide logo */
      #document-sidebar_top #logo {
          display: none !important;
      }
      .document-sidebar_top__user-and-collapse {
          margin-top: 10px !important;
      }
      /*hide queue block */
      #document-sidebar__link {
          display: none;
      }
      /* no highlight colors */
      #documentList .highlight-color--red,
      #documentList .highlight-color--orange,
      #documentList .highlight-color--yellow,
      #documentList .highlight-color--green,
      #documentList .highlight-color--blue,
      #documentList .highlight-color--purple {
          background: none;
      }
      ```
    - [x] Op07 Wider SideBar / Document
      ```css
      :root {
          --document-width: 900px; /*RemNote by default is 800px*/
          --sidebar-width: 260px; /*RemNote by default is 240px*/
      }
      /* wider/narrower document*/
      #multiple-windows .multiple-windows__document .document--narrow {
          max-width: var(--document-width);
      }
      /* wider/narrower sidebar*/
      #homepage #content .document-sidebar--floating, #main #content .document-sidebar--floating {
          max-width: var(--sidebar-width)!important;
          min-width: var(--sidebar-width)!important;
      }
      #homepage #content #document-sidebar, #main #content #document-sidebar {
          max-width: var(--sidebar-width)!important;
          min-width: var(--sidebar-width)!important;
      }
      #document-sidebar__bottom-menu {

          width: var(--sidebar-width);
      }
      .document-sidebar--floating #document-sidebar__bottom-menu {
          width: var(--sidebar-width);
      }
      ```
    - [x] Op08 Reference brackets
      ```css
      .rem-reference-container::before {
          content: "[[";
          color: grey;
          font-weight: 400;
      }

      .rem-reference-container::after {
          content: "]]";
          color: grey;
          font-weight: 400;
      }
      ```
    - [x] Op09 Coding like editing
      ```css
      :root {
          --focused-background-color: transparent;
          --portal-focused-background-color: transparent;
          --focused-background-editing-color: rgb(21, 21, 21, 0.3);
          --portal-focused-background-editing-color: rgb(26, 26, 26, 0.3);    
      }
      #hierarchy-editor .rem-container--focused .rem-text span {
          background-color: var(--focused-background-editing-color);
      }
      #hierarchy-editor .rem-container--focused .rem-text .rem-reference-link span,
      #hierarchy-editor .rem-container--focused .rem-text .rem-reference span,
      #hierarchy-editor .rem-container--focused .rem-text .rem-indented-indicator span,
      #hierarchy-editor .rem-container--focused .rem-text .searchKeywordHighlight span  {
          background: none;
      }
      #hierarchy-editor .portal-tree-node .rem-container--focused .rem-text span {
          background-color: var(--portal-focused-background-editing-color);
      }
      #hierarchy-editor .portal-tree-node .rem-container--focused .rem-text .rem-reference-link span,
      #hierarchy-editor .portal-tree-node .rem-container--focused .rem-text .rem-reference span,
      #hierarchy-editor .portal-tree-node .rem-container--focused .rem-text .rem-indented-indicator span,
      #hierarchy-editor .rem-container--focused .rem-text .searchKeywordHighlight span  {
          background: none;
      }
      #hierarchy-editor .search-portal-tree-node--dark .rem-container--focused .rem-text span {
          background-color: var(--portal-focused-background-editing-color);
      }
      #hierarchy-editor .search-portal-tree-node--dark .rem-container--focused .rem-text .rem-reference-link span,
      #hierarchy-editor .search-portal-tree-node--dark .rem-container--focused .rem-text .rem-reference span,
      #hierarchy-editor .search-portal-tree-node--dark .rem-container--focused .rem-text .rem-indented-indicator span,
      #hierarchy-editor .rem-container--focused .rem-text .searchKeywordHighlight span  {
          background: none;
      }
      #hierarchy-editor .rem-container--focused #code-node {
          background-color: var(--code-block-focused-background-color);
      }
      .embeddedSearch span {
          background-color: var(--code-block-focused-background-color);
      }
      #hierarchy-editor-toolbar-container #hierarchy-editor__add-to-portal .rich-text-editor span {
          background-color: var(--focused-background-editing-color);
      }
      .hierarchy-editor__hidden-children .hierarchy-editor__hidden-children__search .rich-text-editor span {
          background-color: var(--focused-background-editing-color);
      }
      #QueueTypeAnswerBoxContainer #QueueTypeAnswerBox span {
          background-color: var(--focused-background-editing-color);
      }
      ```
    - [x] Op10 Dark PDF (inverted, no real colors)
      ```css
      .pdfViewer {
          filter: invert(100%) hue-rotate(180deg) !important;
      }

      /* highlight colors*/
      /*red*/
      .pdf-viewer__highlight-container--red .AreaHighlight,
      .pdf-viewer__highlight-container--red .Highlight__part {
          background-color: var(--highlight-red)!important;
          opacity: 0.7;
      }
      /*orange*/
      .pdf-viewer__highlight-container--orange .AreaHighlight,
      .pdf-viewer__highlight-container--orange .Highlight__part {
          background-color: var(--highlight-orange)!important;
          filter: brightness(.7);
          opacity: 0.7;
      }
      /*yellow*/
      .pdf-viewer__highlight-container--yellow .AreaHighlight, .pdf-viewer__highlight-container--yellow .Highlight__part {
          background-color: var(--highlight-yellow)!important;
          filter: brightness(.6);
          opacity: 0.7;
      }
      /*green*/
      .pdf-viewer__highlight-container--green .AreaHighlight,
      .pdf-viewer__highlight-container--green .Highlight__part {
          background-color: var(--highlight-green)!important;
          opacity: 0.7;
      }
      /*blue*/
      .pdf-viewer__highlight-container--blue .AreaHighlight,
      .pdf-viewer__highlight-container--blue .Highlight__part {
          background-color: var(--highlight-blue)!important;
          opacity: 0.7;
      }
      /*purple*/
      .pdf-viewer__highlight-container--purple .AreaHighlight,
      .pdf-viewer__highlight-container--purple .Highlight__part {
          background-color: var(--highlight-purple)!important;
          opacity: 0.7;
      }

      /*when selecting to highlight (by default is yellow) I set it to gray*/
      .pdf-viewer__highlight-container--undefined .Highlight__part,
      .pdf-viewer__highlight-container--undefined .AreaHighlight,
      .PdfHighlighter .textLayer ::selection {
          background-color: gray!important;
          filter: brightness(.75)!important;
          opacity: 0.7;
      }
      ```
    - [x] Op11 Image Occlusion (inverted, no real colors)
      ```css
      .tumbnail--with-width {
          filter: invert(87%) hue-rotate(170deg) !important;
      }
      #image-viewer-popup img {
          filter: invert(87%) hue-rotate(170deg) !important;
      }
      .image-occlusion .image-occlusion__canvas-container {
          filter: invert(87%) hue-rotate(170deg) !important;
      }
      ```
```
