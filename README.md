# Settings Flepsz

This repository houses my personal development environment settings, meticulously crafted to optimize my coding workflow and enhance productivity. It encompasses configurations for Visual Studio Code, preferred fonts, and Git configurations, ensuring a consistent and efficient development experience across my projects.

## Git Config

Configure Git with your username and email:

```bash
git config user.name "Flepsz"
git config user.email "luisfelipelfsp3@gmail.com"
```

## VsCode settings.json

```json
{
    "workbench.colorTheme": "Catppuccin Macchiato",
    "editor.tabSize": 2,
    "editor.fontFamily": "Fira Code",
    "editor.fontSize": 13,
    "editor.formatOnSave": true,
    "editor.defaultFormatter": "esbenp.prettier-vscode",
    "editor.fontLigatures": true,
    "editor.wordWrap": "on",
    "editor.bracketPairColorization.enabled": true,
    "editor.parameterHints.enabled": false,
    "editor.semanticHighlighting.enabled": false,
    "editor.renderLineHighlight": "gutter",
    "editor.suggestSelection": "first",
    "editor.acceptSuggestionOnCommitCharacter": false,
    "editor.accessibilitySupport": "off",
    "editor.minimap.enabled": false,
    "editor.cursorBlinking": "expand",
    "editor.quickSuggestions": {
        "other": true,
        "comments": false,
        "strings": false
    },
    "workbench.tree.indent": 15,
    "workbench.startupEditor": "newUntitledFile",
    "workbench.editor.labelFormat": "short",
    "workbench.iconTheme": "symbols",
    "workbench.editor.empty.hint": "hidden",
    "terminal.integrated.fontSize": 14,
    "terminal.integrated.fontFamily": "Fira Code",
    "terminal.integrated.showExitAlert": false,
    "terminal.integrated.gpuAcceleration": "off",
    "terminal.integrated.defaultProfile.osx": "fish",
    "terminal.integrated.env.windows": {},
    "[python]": {
        "editor.tabSize": 4,
        "editor.defaultFormatter": "ms-python.autopep8",
    },
    "[java]": {
        "editor.defaultFormatter": "redhat.java",
        "editor.tabSize": 4
    },
    "[javascript]": {
        "editor.tabSize": 2,
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "[javascriptreact]": {
        "editor.tabSize": 2,
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "[typescript]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode",
        "editor.tabSize": 2
    },
    "[typescriptreact]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode",
        "editor.tabSize": 2
    },
    "[css]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "[prisma]": {
        "editor.defaultFormatter": "Prisma.prisma",
        "editor.tabSize": 4
    },
    "[sql]": {
        "editor.defaultFormatter": "ms-mssql.mssql"
    },
    "[json]": {
        "editor.defaultFormatter": "vscode.json-language-features"
    },
    "[jsonc]": {
        "editor.defaultFormatter": "vscode.json-language-features"
    },
    "[rust]": {
        "editor.defaultFormatter": "rust-lang.rust-analyzer",
        "editor.formatOnSave": true,
        "editor.tabSize": 4
    },
    "diffEditor.wordWrap": "on",
    "emmet.syntaxProfiles": {
        "javascript": "jsx"
    },
    "emmet.includeLanguages": {
        "javascript": "javascriptreact"
    },
    "javascript.suggest.autoImports": true,
    "javascript.updateImportsOnFileMove.enabled": "always",
    "typescript.tsserver.log": "off",
    "typescript.updateImportsOnFileMove.enabled": "always",
    "typescript.suggest.autoImports": true,
    "extensions.ignoreRecommendations": true,
    "files.associations": {
        ".sequelizerc": "javascript",
        ".stylelintrc": "json",
        "*.tsx": "typescriptreact",
        ".env.*": "dotenv",
        ".prettierrc": "json",
        "*.html": "html",
        "*.css": "css",
        "*.js": "javascript",
        "*.json": "json",
        "*.ts": "typescript",
        "*.md": "markdown",
        "*.jsx": "javascriptreact"
    },
    "explorer.confirmDelete": false,
    "liveshare.featureSet": "insiders",
    "git.enableSmartCommit": true,
    "explorer.confirmDragAndDrop": false,
    "eslint.validate": [
        "javascript",
        "javascriptreact",
        "graphql"
    ],
    "breadcrumbs.enabled": true,
    "security.workspace.trust.untrustedFiles": "newWindow",
    "tabnine.experimentalAutoImports": true,
    "update.mode": "start",
    "liveServer.settings.donotShowInfoMsg": true,
    "window.commandCenter": true,
    "git.openRepositoryInParentFolders": "always",
    "css.lint.unknownAtRules": "ignore",
    "console-ninja.featureSet": "Community",
    "prettier.useTabs": true,
    "files.autoSave": "afterDelay",
    "symbols.hidesExplorerArrows": false,
    "editor.unicodeHighlight.allowedLocales": {
        "es": true
    },
    "editor.codeActionsOnSave": {
        "source.fixAll.eslint": "explicit",
        "source.addMissingImports": "explicit"
    },
    "editor.rulers": [
        80,
        120
    ],
    "workbench.editorAssociations": {
        "*.db": "sqlite-viewer.option"
    },
    "terminal.integrated.env.osx": {
        "FIG_NEW_SESSION": "1"
    },
    "files.exclude": {
        "**\/CVS": true,
        "**\/.DS_Store": true,
        "**\/.hg": true,
        "**\/.svn": true,
        "**\/.git": true,
        // "node_modules": true
    },
    "tailwindCSS.classAttributes": [
        "class",
        "className",
        "ngClass",
        "containerStyle",
        "style"
    ],
    "diffEditor.ignoreTrimWhitespace": false,
    "git.confirmSync": false,
    "prisma.showPrismaDataPlatformNotification": false,
    "settingsSync.ignoredExtensions": [
        "graphql.vscode-graphql",
        "graphql.vscode-graphql-syntax",
        "icrawl.discord-vscode",
        "gitpod.gitpod-desktop",
        "vscjava.vscode-maven",
        "redhat.java",
        "redhat.fabric8-analytics",
        "vmware.vscode-boot-dev-pack",
        "ms-mssql.sql-bindings-vscode",
        "ms-mssql.sql-database-projects-vscode",
        "ms-mssql.mssql",
        "ms-python.python",
        "ms-python.autopep8",
        "formulahendry.code-runner",
        "vscjava.vscode-java-debug"
    ],
    "remote.SSH.remotePlatform": {
        "*.gitpod.io": "linux"
    },
    "git.autofetch": true
}
```

## Download Fira Code Font

<a href="https://github.com/tonsky/FiraCode/releases/download/6.2/Fira_Code_v6.2.zip"><img alt="Fira_Code_v6.2.zip - December 6, 2021 - 2.5 MB" src="https://raw.githubusercontent.com/tonsky/FiraCode/master/extras/download.png" width="520"></a>
