Use command to clone configst to your project root folder:

```
# you can use folder name instead of a dot ".":
# npx degit aprokdev/react-formatting my-project-any-folder

npx degit aprokdev/react-formatting .
```

then install dependencies to your project by command

```
npm i --save-dev eslint eslint-config-prettier eslint-config-react-app eslint-plugin-eslint-comments eslint-plugin-prettier eslint-plugin-react-hooks prettier stylelint stylelint-config-prettier-scss stylelint-config-standard-scss stylelint-order
```

then add additional scripts if needed to package.json

```
{
    "scripts": {
        "lint": "npx eslint ./src --ext .js,.jsx",
        "stylelint": "npx stylelint **/*.scss --cache --fix",
        "prettify": "npx prettier --write ."
    }
}
```

then you will have automatic formatting/autofix when save your files in VS Code
