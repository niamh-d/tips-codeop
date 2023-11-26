# Tips

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

## Formatting and Autosave in VSCode

- Make sure you have extension "Prettier - Code formatter" installed ([link](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)).
- Then go to Settings and type "format" in the search bar
- Set Prettier as default formatter under "Editor: Default Formatter"
- Check tickbox under "Editor: Format On Save"
- Type "autosave" into search bar
- Under "Files: Auto Save" select "onFocusChange"
