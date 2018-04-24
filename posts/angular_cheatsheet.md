[Main](/index.md)


__Installation__

- `npm i -g @angular/cli`


__Create new project__

- `ng new [name]`
- `ng new [name] --skip-test` (without tests)
- `ng new [name] --minimal` (without tests and with inline templates)
- `ng new [name] --inline-template` (with inline templates)
- `ng new [name] --inline-style` (with inline styles)
- `ng new [name] --style=scss` (with preprocessor scss / less / sass / styl)
- `ng new [name] --routing` (with a routing module)
- `ng new [name] --prefix=myapp` (prefix for selectors)
- `ng new [name] --skip-git`

Example: `ng new FETestApp --skip-test --style=scss --routing --prefix=u`


__Run the apllication__

- `ng serve --host 0.0.0.0 --port 4201`


__Change Package Manager__

- `ng set --global packageManager=yarn`


__Generate scaffolds__

- `ng g component my-new-component`
- `ng g directive my-new-directive`
- `ng g pipe my-new-pipe`
- `ng g service my-new-service`
- `ng g class my-new-class`
- `ng g guard my-new-guard`
- `ng g interface my-new-interface`
- `ng g enum my-new-enum`
- `ng g module my-module`


__Add Material__

- `npm i @angular/material`
- `npm i @angular/cdk`
- *index.html* - `<link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">`
- *styles.less* - `@import "~@angular/material/prebuilt-themes/indigo-pink.css";`
- *app.module.ts* - `imports: [BrowserAnimationsModule]`
