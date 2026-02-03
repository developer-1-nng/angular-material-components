# Angular Material Color Picker for @angular/material 16.x, 17.x, 18.x, 19.x, 20.x

## Description

An Angular Material Color Picker.

## DEMO

@see [DEMO stackblitz](https://stackblitz.com/edit/demo-ngx-mat-color-picker)

![Alt Text](demo_color_picker.png)

 Choose the version corresponding to your Angular version:

 Angular     | @nng-components/angular-material-color-picker
 ----------- | -------------------
 20          | 20.x+
 19          | 19.x+
 18          | 18.x+
 17          | 17.x+
 16          | 16.x+
 

## Getting started

```
npm install --save  @nng-components/angular-material-color-picker
```

## Setup

```
import { MAT_COLOR_FORMATS, NgxMatColorPickerModule, NGX_MAT_COLOR_FORMATS } from '@nng-components/angular-material-color-picker';

@NgModule({
   ...
   imports: [
        ...
        NgxMatColorPickerModule
   ],
   providers: [
    { provide: MAT_COLOR_FORMATS, useValue: NGX_MAT_COLOR_FORMATS }
   ],
   ...
})
export class AppModule { }
```
@see [src/app/demo-colorpicker/demo-colorpicker.module.ts](src/app/demo-colorpicker/demo-colorpicker.module.ts)

## Using the component

### Color Picker (ngx-mat-color-picker)

```
<mat-form-field>
    <input matInput [ngxMatColorPicker]="picker" [formControl]="colorCtr" [disabled]="disabled">
    <ngx-mat-color-toggle matSuffix [for]="picker"></ngx-mat-color-toggle>
    <ngx-mat-color-picker #picker [touchUi]="touchUi" [color]="color"></ngx-mat-color-picker>
</mat-form-field>
```

#### List of @Input

| @Input        	| Type     	| Default value 	| Description                                                          	|
|---------------	|----------	|---------------	|----------------------------------------------------------------------	|
| **disabled**      	| boolean  	| null          	| If true, the picker is readonly and can't be modified                	|
| **touchUi**    	   | boolean   | false           | Whether the calendar UI is in touch mode. In touch mode the calendar opens in a dialog rather than a popup and elements have more padding to allow for bigger touch targets. 	|

## Theming
- @see @angular/material [Using a pre-built theme](https://material.angular.io/guide/theming#using-a-pre-built-theme)
- Add the Material Design icon font to your index.html
```
<link href="https://fonts.googleapis.com/icon?family=Material+Icons&display=block" rel="stylesheet">
```

## License
MIT