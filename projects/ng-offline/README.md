[![GitHub license](https://img.shields.io/github/license/navneetlal/ng-offline?style=flat-square)](https://github.com/navneetlal/ng-offline/blob/master/LICENSE)
![npm](https://img.shields.io/npm/v/ng-offline?color=blue&style=flat-square)

# NgOffline
A simple angular module which enables directives `ngOnline` and `ngOffline` to make conditional rendering of component based on network status.

### Installing

```bash
$ npm install ng-offline --save
```

### Basic usage
Import `NgOfflineModule` into your ngModule and start using directives `ngOnline` and `ngOffline` within your html component.

##### **`app.module.ts`**
```ts
import { BrowserModule } from '@angular/platform-browser';
import { NgModule } from '@angular/core';

import { NgOfflineModule } from 'ng-offline';

import { AppComponent } from './app.component';

@NgModule({
  declarations: [
    AppComponent
  ],
  imports: [
    BrowserModule,
    NgOfflineModule
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }
```

##### **`app.component.html`**
```html
<div ngOnline>Hey! You are online</div>
<div ngOffline>You're offline. Check your connection!</div>
```

First div container will only be visible when network status in online and second div will be visible after network status in offline.

### License
Published under the [MIT License](https://github.com/navneetlal/react-offline-component/blob/master/LICENSE).
