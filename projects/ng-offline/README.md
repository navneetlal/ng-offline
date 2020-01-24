# NgOffline
A simple angular directive which checks whether network connectivity is available or not.

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

### License
Published under the [MIT License](https://github.com/navneetlal/react-offline-component/blob/master/LICENSE).
