# Tips

## VSCode

### Opening VSCode with current directory from your terminal

Instructions [here](https://www.freecodecamp.org/news/how-to-open-visual-studio-code-from-your-terminal/).

### Formatting and Autosave in VSCode

- Make sure you have extension "Prettier - Code formatter" installed ([link](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)).
- Then go to Settings and type "format" in the search bar
- Set Prettier as default formatter under "Editor: Default Formatter"
- Check tickbox under "Editor: Format On Save"
- Type "autosave" into search bar
- Under "Files: Auto Save" select "onFocusChange"

### Make VSCode Pretty

- Go to [VSCodeThemes](https://vscodethemes.com/) and find your favourite colour theme.
- Click on the image and it will take you to a theme page with previews and a button to add this theme to your editor.
- Install [Material Icons](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme) to make your file and filder icons pretty

## Building webpages

### Live Server

When building webpages you're going to want to have [LiveServer](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) installed. It means you never have to manually refresh the browser again.

### For easier writing of HTML

- Use [Emmet snippets](https://code.visualstudio.com/docs/editor/emmet)
- Install extension "Auto Close Tag"
- Install extension "Auto Rename Tag"

### font-size: 62.5%

In your CSS file, apply the below code:

```
:root {
  font-size: 62.5%;
}
```

The default size for font in browsers is 16px. 62.5% of 16px = 10px. Now when you size using rem units, each rem = 10px, so 2rem = 20px, 10rem = 100px. Makes using rem units much easier! Read about using rem units [**here**](https://www.sitepoint.com/understanding-and-using-rem-units-in-css/).

## VSCode Snippets

This repo contains a txt file with helpful snippets. [Click here](https://code.visualstudio.com/docs/editor/userdefinedsnippets) for info on what snippets are.

### Console.log() snippet

Add the below to your snippets.code-snippets file in VSCode for easier writing of console.log().

```
  "Print to console": {
    "prefix": "cl",
    "scope": "javascript,typescript,javascriptreact",
    "body": ["console.log($1)"],
    "description": "console.log"
  }
```

### For easier writing of React code

- Use [Snippets](https://marketplace.visualstudio.com/items?itemName=xabikos.ReactSnippets)

## Node modules

### Git ignore file

In your ".gitignore" file, make sure you have node modules mentioned:

```
/node_modules
```

That way git won't track that folder and won't upload it to GitHub.

### Old projects

When you are finished with a project, delete the folder "node_modules". It takes up a lot of space and you don't keep to keep it for old projects. If you ever want to revisit an old project and run it again just type the following in the terminal and the folder will be reinstalled.

```
npm i
```
