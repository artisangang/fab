# fab
FAB for angular 5

Currently FAB Speed Dial ony. Some modification in styling may turn speed dial into toolbar.


**Declare Fab components in main module**
This is how your app.module.ts may look like after declaring FabComponents

```ts
import { BrowserModule } from '@angular/platform-browser';
import { NgModule } from '@angular/core';


import { AppComponent } from './app.component';

import { FabComponents } from '../directive/fab';


@NgModule({
  declarations: [
    AppComponent,
    FabComponents
  ],
  imports: [
    BrowserModule
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }
```

**In Template**
Avialable directions: up,down,left,right.

```html
<fab dir="up">
    <fab-toggle>+</fab-toggle>
    <fab-button>A</fab-button>
    <fab-button>B</fab-button>
    <fab-button>C</fab-button>
    <fab-button>D</fab-button>
</fab>
```  

**Note:** make sure to attach style.css

