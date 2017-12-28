# dx-locale-zh-cn

Chinese localization messages for DevExpress/DevExtreme

## Usage

1. Install it with npm:

   `npm install devextreme-intl dx-locale-zh-cn`

2. Add some code to the root component of your app, usually it is `AppComment`, like this:

   ```ts
   import { Component, OnInit } from '@angular/core';

   import { loadMessages, locale } from 'devextreme/localization';
   import { localeMessages, localeName } from 'dx-locale-zh-cn';

   @Component({
       moduleId: module.id,
       selector: 'app-root',
       templateUrl: './app.component.html',
       styleUrls: ['./app.component.scss']
   })
   export class AppComponent implements OnInit {
   
       public ngOnInit(): void {
           loadMessages(localeMessages);
           locale(localeName);
       }
   
   }
   ```

3. Ok, it's done!
