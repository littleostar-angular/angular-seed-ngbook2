
---
systemjs.config.js
```json
System.config({
    transpiler: 'typescript',
    typescriptOptions: {emitDecoratorMetadata: true},
    map: {
        '@angular'  : 'node_modules/@angular',
        'rxjs'      : 'node_modules/rxjs'
    },
    paths: {
        'node_modules/@angular/*': 'node_modules/@angular/*/bundles'
    },
    meta: {
        '@angular/*': {'format': 'cjs'}
    },
    packages: {
        'app'                               : {main: 'main', defaultExtension: 'ts'},
        'rxjs'                              : {main: 'Rx'},
        '@angular/core'                     : {main: 'core.umd.min.js'},
        '@angular/common'                   : {main: 'common.umd.min.js'},
        '@angular/compiler'                 : {main: 'compiler.umd.min.js'},
        '@angular/platform-browser'         : {main: 'platform-browser.umd.min.js'},
        '@angular/platform-browser-dynamic' : {main: 'platform-browser-dynamic.umd.min.js'},
    }
});
```

---
package.json
```json
{
  "name": "angular-seed-ngbook2",
  "description": "",
  "private": true,
  "scripts": {
    "start": "live-server"
  },
  "dependencies": {
    "@angular/common": "^2.4.0",
    "@angular/compiler": "^2.4.0",
    "@angular/core": "^2.4.0",
    "@angular/forms": "^2.4.0",
    "@angular/http": "^2.4.0",
    "@angular/platform-browser": "^2.4.0",
    "@angular/platform-browser-dynamic": "^2.4.0",
    "@angular/router": "^3.4.0",
    "core-js": "^2.4.1",
    "rxjs": "^5.1.0",
    "zone.js": "^0.7.6",
    "systemjs": "0.19.37"
  },
  "devDependencies": {
    "live-server": "0.8.2",
    "typescript": "~2.0.0"
  }
}

```

---

end
