# React formatting

Easy add formatting for your React/SCSS code

Use command to clone configs to your project root folder, use --force flag if necessary (usually it necessary if project folder is not empty):

```bash
# you can use folder name instead of a dot ".":
# npx degit aprokdev/react-formatting my-project-any-folder
```

```bash
npx degit aprokdev/react-formatting .
```

then install dependencies to your project by command

```bash
npm i --save-dev eslint eslint-config-prettier eslint-config-react-app eslint-plugin-eslint-comments eslint-plugin-prettier eslint-plugin-react-hooks prettier stylelint stylelint-config-prettier-scss stylelint-config-standard-scss stylelint-order
```

then add additional scripts if needed to package.json

```bash
{
    "scripts": {
        "lint": "npx eslint ./src --ext .js,.jsx",
        "stylelint": "npx stylelint **/*.scss --cache --fix",
        "prettify": "npx prettier --write ."
    }
}
```

then you will have automatic formatting/autofix when save your files in VS Code
